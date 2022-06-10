# layout.bars

Компонент, добавляющий к контенту верхнюю и нижнюю панели.

Внутри каждой части компонента вы можете использовать другие компоненты, например картинки, текст или переключатели.

Верхняя панель располагается у верхней границы компонента, а нижняя — у нижней. Контент располагается между панелями, занимая все доступное пространство.

## Свойства компонента {#properties}

#|
|| **Название** | **Тип** | **Описание** ||
|| `type`<span style="color: red">\*</span> | "layout.bars" | Задает тип компонента. ||
|| `barAfter` | _view_ | Панель, которая отображается у нижней границы компонента. ||
|| `barBefore` | _view_ | Панель, которая отображается у верхней границы компонента. ||
|| `content`<span style="color: red">\*</span> | _view_ | Основной контент. ||
|| `validation` | _condition_ | Валидация на основе условия _(condition)_. ||
|#