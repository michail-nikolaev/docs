# Выделение объектов на картинке

{% include [deprecate](../../_includes/deprecate.md) %}

В этом разделе описано, как добавить к картинке редактор для выделения областей и как можно ускорить работу с ним с помощью горячих клавиш. Если вам нужно просто вставить картинку, читайте раздел [Вставка картинок](insert-images.md).


## Добавить редактор для выделения {#add-select}

Чтобы добавить возможность выделять на картинках области, используйте компонент [field.image-annotation](../reference/field.image-annotation.md).

```json
{
  "view": {
    "type": "field.image-annotation",
    "data": {
      "type": "data.output",
      "path": "path"
    },
    "image": "url"
  }
}
```

[![](../_images/buttons/view-example.svg)](https://ya.cc/t/HdPqNHC53ttFBy)


## Настроить режимы разметки {#shapes}

Компонент предлагает три режима разметки: прямоугольниками, многоугольниками и точками. По умолчанию исполнителю доступны все три режима. Вы можете оставить лишь определенные режимы: один или два из них.

{% list tabs %}

- Прямоугольниками

  Чтобы разрешить выделять области только прямоугольниками, в свойстве `shapes` добавьте ключ `rectangle` и передайте ему значение `true`.

  ```json
  {
    "shapes": {
      "rectangle": true
    }
  }
  ```

  [![](../_images/buttons/view-example.svg)](https://ya.cc/t/ZtJ6f56P3ttFCb)

- Многоугольниками

  Чтобы разрешить выделять области только многоугольниками, в свойстве `shapes` добавьте ключ `polygon` и передайте ему значение `true`.

  ```json
  {
    "shapes": {
      "polygon": true
    }
  }
  ```

  [![](../_images/buttons/view-example.svg)](https://ya.cc/t/frlb1AGg3ttFDC)

- Точками

  Чтобы разрешить выделять области только точками, в свойстве `shapes` добавьте ключ `point` и передайте ему значение `true`.

  ```json
  {
    "shapes": {
      "point": true
    }
  }
  ```

  [![](../_images/buttons/view-example.svg)](https://ya.cc/t/9ZNO1IDp3ttFE3)

{% endlist %}

## Классифицировать области {#labels}

Вы можете позволить исполнителю выделять объекты по типам. Например, если вам нужно, чтобы все выделенные на картинке машины попали в один тип, а дорожные знаки — в другой.

```json
{
  "labels": [{
      "label": "Вариант 1",
      "value": "value1"
    },
    {
      "label": "Вариант 2",
      "value": "value2"
    }
  ]
}
```

[![](../_images/buttons/view-example.svg)](https://ya.cc/t/3L2iMLDD3tvyLo)

Каждый новый объект свойства `labels` добавляет в редакторе кнопку для выбора типа области, а разное значение `value` дает возможность выделить область уникальным цветом.


## Добавить горячие клавиши {#hotkeys}

Чтобы помочь исполнителю работать быстрее, добавьте горячие клавиши с помощью компонента [plugin.field.image-annotation.hotkeys](../reference/plugin.field.image-annotation.hotkeys.md). Горячие клавиши можно назначить на стрелки вверх и вниз (`up`,`down`), цифры и латинские буквы.

Если вы добавите плагин для горячих клавиш без уточнения значений, то они будут проставлены по умолчанию.

[![](../_images/buttons/view-example.svg)](https://ya.cc/t/sn4WScBK3ttFEp)

Поменяйте их как описано ниже, если вам они не подходят. Если вам не нужен какой-то вид горячих клавиш, то передайте ему пустое значение.

{% list tabs %}

- Выбрать типы областей

  Если у вас доступны хотя бы два типа областей, то перечислите для них горячие клавиши через запятую в массиве свойства `labels`. Они добавятся на кнопки выбора разных областей в порядке их отображения.

  ```json
  {
    "type": "plugin.field.image-annotation.hotkeys",
    "labels": [
        "1",
        "2"
    ]
  }
  ```

  [![](../_images/buttons/view-example.svg)](https://ya.cc/t/HzTesKy63tvyxa)

- Выбрать режимы разметки

  Вы можете позволить исполнителю переключаться между разными режимами разметки с помощью горячих клавиш. Добавьте в свойстве `modes` нужный вам ключ и передайте ему значение горячей клавиши:
  - `select` — для режима выбора фигур и точек;
  - `point` — для режима разметки точками;
  - `rectangle` — для режима разметки прямоугольниками;
  - `polygon` — для режима разметки многоугольниками.

  ```json
  {
    "type": "plugin.field.image-annotation.hotkeys",
    "modes": {
      "select": "q",
      "point": "w",
      "rectangle": "e",
      "polygon": "r"
    }
  }
  ```

  [![](../_images/buttons/view-example.svg)](https://ya.cc/t/33szOrFP3tvzLF)

- Подтвердить или отменить создание области

  Настройте горячие клавиши, чтобы исполнитель мог подтверждать или отменять создание новой области. Передайте свойствам значения горячих клавиш:
  - `confirm` — подтвердить;
  - `cancel` — отменить.

  ```json
  {
    "type": "plugin.field.image-annotation.hotkeys",
    "confirm": "x",
    "cancel": "z"
  }
  ```

  [![](../_images/buttons/view-example.svg)](https://ya.cc/t/2girQif13tvzZF)

{% endlist %}

## Создать задание {#create-task}

Чтобы создать шаблон для задания по выделению областей, используйте следующие компоненты:

- [field.image-annotation](../reference/field.image-annotation.md) — чтобы добавить редактор для разметки;
- [plugin.field.image-annotation.hotkeys](../reference/plugin.field.image-annotation.hotkeys.md) — чтобы добавить горячие клавиши;
- [view.text](../reference/view.text.md) — чтобы добавить описание к заданию;
- [condition.required](../reference/condition.required.md) — чтобы убедиться, что исполнитель выделил хотя бы одну область;
- [plugin.toloka](../reference/plugin.toloka.md) — чтобы настроить внешний вид задания.

[![](../_images/buttons/view-example.svg)](https://ya.cc/t/grA2YJnS3tvztP)


[![](../_images/buttons/contact-support.svg)](../concepts/support.md)
