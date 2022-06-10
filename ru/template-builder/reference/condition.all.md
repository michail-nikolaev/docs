# condition.all

Проверяет, что **все** дочерние условия выполняются. Если хотя бы одно условие не выполнено, компонент возвращает `false`.

[Посмотреть пример в песочнице](https://clck.ru/RFUkZ).

Если вам достаточно выполнения одного из нескольких условий, используйте компонент [condition.any](condition.any.md). Вы также можете комбинировать эти компоненты.

## Свойства компонента {#properties}

#|
|| **Название** | **Тип** | **Описание** ||
|| `type`<span style="color: red">\*</span> | "condition.all" | Задает тип компонента. ||
|| `conditions` | _array_ | Набор условий, которые должны быть выполнены. ||
|| `conditions[]` | _condition_ | Необходимое условие. ||
|| `hint` | _string_ | Сообщение об ошибке валидации, которое увидит исполнитель ||
|#