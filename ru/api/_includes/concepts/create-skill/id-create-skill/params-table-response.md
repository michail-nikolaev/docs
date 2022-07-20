#|
||**Параметр** | **Описание**||
||**id** | **string**

Идентификатор навыка.||
||**name** | **string**

Название навыка.||
||**private_comment** | **string**

Комментарий к навыку (доступен только заказчику).||
||**hidden** | **boolean**

Доступ к сведениям о навыке (название и значение) для исполнителей:

- `true` — закрыт;
- `false` — открыт.
По умолчанию значение `true`.||
||**skill_ttl_hours** | **integer**

Время жизни навыка после последнего обновления (в часах). Навык будет удален у исполнителя, если его значение не обновлялось в течение указанного срока.||
||**deprecated** | **boolean**

Прекращение поддержки навыка его создателем:

- `true` — поддержка прекращена, навык требует замены;
- `false` — поддержка ведется, навык актуальный.||
||**owner** | **object**

Параметры заказчика, который создал проект.||
||**owner.id** | **string**

Идентификатор заказчика.||
||**owner.myself** | **boolean**

Проверяет, кому принадлежит объект:

- `true` — исполнителю, чей OAuth-токен указан в запросе;
- `false` — другому аккаунту (сотруднику или владельцу).||
||**training** | **boolean**

Связь навыка с обучающим пулом:

- `true` — навык подсчитывается по заданиям обучающего пула;
- `false` — навык не связан с обучающим пулом.||
||**created** | **string**

Дата и время создания навыка по UTC в формате ISO 8601: `YYYY-MM-DDThh:mm:ss[.sss]`.||
||**global** | **boolean**

Признак глобального навыка:

- `true` — навык [глобальный]({{ requester-skills-global }}), показывает общие компетенции исполнителей, доступен всем исполнителям;
- `false` — навык создан заказчиком, может быть [назначен]({{ requester-assign-skills }}) исполнителям как вручную, так и автоматически: с помощью правил контроля качества или после прохождения обучения.||
|#