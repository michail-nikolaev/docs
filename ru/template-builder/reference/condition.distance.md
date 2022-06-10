# @yandex-toloka/condition.distance

Компонент проверяет, соответствуют ли переданные координаты заданным.

Например, вы хотите, чтобы исполнитель сфотографировал конкретное место. Компонент `condition.distance` проверит, сделана ли фотография в том месте, координаты которого вы указали.

За передачу координат устройства отвечает компонент [data.location](data.location.md). Вы можете использовать его без `condition.distance`, если вам нужно считать координаты устройства исполнителя без сравнения с заданными.

[Посмотреть пример в песочнице](https://clck.ru/TpUxX).

## Свойства компонента {#properties}

#|
|| **Название** | **Тип** | **Описание** ||
|| `type`<span style="color: red">\*</span> | "@yandex-toloka/condition.distance" | Задает тип компонента. ||
|| `from` | _string_ | Координаты, которые будут сравниваться с координатами из свойства `to`. ||
|| `hint` | _string_ | Сообщение об ошибке валидации, которое увидит исполнитель ||
|| `max` | _number_ | Расстояние в метрах, на которое могут отличаться заданные и переданные координаты. ||
|| `to` | _string_ | Координаты, которые будут сравниваться с координатами из свойства `from`. ||
|#