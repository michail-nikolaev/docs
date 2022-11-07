# Финансы

{% include [troubleshooting-key-combination](../_includes/troubleshooting/troubleshooting/id-troubleshooting/key-combination.md) %}

## Пополнение счета {#concept-1}

{% cut "Как подключиться к биллингу из Москвы или Санкт-Петербурга?" %}

Если ваш адрес в самом Санкт-Петербурге, введите Санкт-Петербург в поле **Регион**, затем введите улицу, номер дома и индекс. Остальные поля заполнять не нужно.

Если ваш адрес в самой Москве, введите Москва в поле **Регион**, затем введите улицу, номер дома и индекс. [Подробнее](../concepts/refill-russia.md#step-by-step) о подключении к биллингу.

Если всё равно не получается [напишите](troubleshooting.md) полный адрес с индексом, который вы пытаетесь ввести, по форме обратной связи. Подскажем, как правильно заполнить поля.

{% endcut %}

{% cut "При пополнении счета вижу сумму, в 1000 раз большую, чем планировал — почему?" %}

Это нормально. Например, если вы вводили 25 $, а видите 25,000 — это все еще 25 долларов с десятичной запятой. На счет вы получите 25 $ по актуальному курсу. Сумма в рублях появится, когда вы перейдете к оплате.

{% endcut %}

{% cut "Почему мы пополняем счет не в российской валюте?" %}

Толока — международная платформа для исполнителей из разных стран. Ее предоставляет швейцарская компания Yandex Services AG.

{% endcut %}

{% cut "Почему мы платим НДС 20% в счете?" %}

Согласно налоговому законодательству РФ мы внесли п.3.8. в [Соглашение с заказчиком]({{ customeragreement-probki }}) — НДС начисляется дополнительно к стоимости услуг и включается в счет на оплату. Так же мы все платим НДС в любом магазине. На свой счет в Толоке вы получите сумму, которую указывали при пополнении.

{% endcut %}

{% cut "Сколько времени занимает оплата счета?" %}

Если вы оплачиваете банковской картой, средства обычно поступают на ваш счет в Толоке в течение нескольких минут. Если ваши средства не отображаются в счете, [напишите нам](../troubleshooting/support.md#help) — разберемся. Укажите логин заказчика и номер счета, а также отметьте тему **Пополнение счета**.

{% endcut %}

{% cut "Как узнать курс, по которому происходит валютный обмен при пополнении счета в Толоке?" %}

Вы указываете сумму пополнения в долларах США. В **Балансе** она переводится в рубли с учетом НДС. Конверсия производится по курсу ЦБ РФ на момент выставления счета по всемирному времени (UTC). [Подробнее](../concepts/refill-russia.md) о пополнении счета.

{% endcut %}

{% cut "Как добавить деньги в Толоку?" %}

Пополнить счет в Толоке можно с банковской карты или банковским переводом. На странице [Профиль]({{ profile }}) нажмите на кнопку Подключиться к биллингу, заполните форму, появится кнопка Пополнить счет. [Подробнее](../concepts/refill-russia.md#step-by-step) по шагам.

[Получить закрывающие документы и акты](support.md#feedback_g3b_vj3_qjb)

{% endcut %}

[Другой вопрос](support.md#new)

## Оплата заданий {#concept-2}

{% cut "Где установить цену задания?" %}

Установить цену за **страницу** заданий можно на странице редактирования пула. Минимальная цена для обычных пулов составляет 0,005 $.

{% endcut %}

{% cut "Как сформировать бюджет на свое первое задание в Толоке?" %}

Общее правило формирования цены: чем больше времени нужно на выполнение, тем выше цена.

Если задание простое , например, на оценку релевантности товара исполнитель потратит несколько секунд, то при 10 заданиях (товарах) на странице устанавливайте стоимость 0,01 $-0,02 $.

Если вы зарегистрируетесь в Толоке как исполнитель, то сможете проанализировать предложения других заказчиков.

Определите цену страницы, умножьте на перекрытие (например, в задании по классификации это обычно 3-5) и учтите НДС 20%. Попробуйте положить на счет первые 10 $, а затем пополняйте его с учетом выполнения.

{% endcut %}

{% cut "Как я могу платить больше исполнителям, которые заполняют необязательные поля?" %}

Вы можете выдавать бонусы после выполнения и описать условие получения повышенного вознаграждения в инструкции к заданию. Возможности изменять цену за страницу заданий динамически по результатам выполнения не предусмотрено.

{% endcut %}

{% cut "Где находится статистика по выплаченным бонусам?" %}

Отслеживайте списание денег на бонусы в {% if locale == "ru-ru" %}**Профиле** → вкладка **Затраты**{% endif %}{% if locale == "en-com" %}**Profile** → **Spent**{% endif %}.

{% endcut %}

{% cut "Могут ли быть в пуле задания с разными ценами?" %}

Нет, цена за страницу заданий общая для всех заданий в пуле. Вы можете создать несколько пулов с разными ценами или [изменять цену](../concepts/dynamic-pricing.md) в зависимости от навыка исполнителя с помощью **Динамического ценообразования**. Добросовестным исполнителям можно [выплачивать бонусы.](../concepts/bonus.md)

{% endcut %}

[Другой вопрос](support.md#new)

## Возврат средств {#concept-3}

[Вернуть средства, перечисленные на счет в Толоку](support.md#feedback_khw_wc3_qjb)

[Другой вопрос](support.md#new)

{% include [contact-support](../_includes/contact-support-help.md) %}