# action.notify

Компонент создает сообщение в левом нижнем углу экрана.

Можно задать: длительность активности сообщения, длительность задержки появления и цвет фона.

## Свойства компонента {#properties}

#|
|| **Название** | **Тип** | **Описание** ||
|| `type`<span style="color: red">\*</span> | "action.notify" | Задает тип компонента. ||
|| `payload`<span style="color: red">\*</span> | _object_ | Параметры для сообщения. ||
|| `payload.content`<span style="color: red">\*</span> | _string_ | Текст сообщения. ||
|| `payload.delay` | _number_ | Длительность задержки (в миллисекундах) до появления сообщения. ||
|| `payload.duration` | _number_ | Длительность активности сообщения (в миллисекундах), которое включает длительность задержки его показа.

Например, если `duration` — 1000, а `delay` — 400, то длительность показа сообщения будет 600 миллисекунд. ||
|| `payload.theme`<span style="color: red">\*</span> | _string_ | Цвет фона сообщения:

- `info` — синий.
- `success` — зеленый.
- `warning` — желтый.
- `danger` — красный.
  ||
  |#