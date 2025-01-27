# Создание навыка

{% include [deprecate](../../_includes/deprecate.md) %}

Чтобы создать навык, нажмите кнопку {% if locale == "en-com" %}**+ Add skill**{% endif %}{% if locale == "ru-ru" %}**+Добавить навык**{% endif %} на странице [Навыки]({{ skills }}).

Если сделать навык публичным, исполнители смогут увидеть данные о присвоенном навыке: название и значение.

{% note tip %}

Чтобы заинтересовать исполнителя, сделайте навык публичным и используйте [динамическое ценообразование](../../glossary.md#dynamic-pricing) на основе этого навыка. В инструкции к заданию напишите, что влияет на значение навыка. Исполнители увидят информацию о том, как навык влияет на цену, и будут стремиться качественно выполнять задания.

{% endnote %}

## Что дальше {#what-next}

[Назначьте навык](nav-assign.md) вручную или автоматически.

## Решение проблем {#troubleshooting}

{% cut "Нужно ли создавать навык для каждого пула?" %}

Лучше использовать один [навык](../../glossary.md#skill) в проекте. Можно выбрать способ подсчета навыка:

- Подсчет навыка для каждого пула отдельно. Текущее значение навыка — это значение навыка в пуле, который выполнялся последним. Такой вариант удобен, если:

    - Пулы предназначены для разных групп исполнителей (например, настроены фильтры по городам, странам).

    - Пулы запускаются последовательно, и вы не хотите учитывать качество ответов в предыдущих пулах при подсчете навыка в выполняемом пуле.

    Этот способ подсчета действует по умолчанию при добавлении блока контроля качества в пул. Для блока по контрольным заданиям оставьте пустым поле **Учитывать последних ответов на контрольные и обучающие задания**.

- Подсчет навыка по всем выполненным заданиям в проекте. Такой вариант удобен, если пулы небольшие и вам не нужно рассчитывать навык для каждого пула.

    Этот способ подсчета доступен только для навыков по контрольным заданиям. Чтобы использовать его, заполните поле **Учитывать последних ответов на контрольные и обучающие задания** в блоках контроля качества в пулах.

{% endcut %}

{% cut "Можно ли использовать навык не только в пуле или в одном проекте, но и в разных проектах?" %}

Да, конечно, один и тот же навык можно назначать и использовать на различных проектах. Но чаще всего один навык используется в рамках одного проекта. Если исполнитель хорошо выполняет одно задание, это не значит, что он так же успешно справится с другим. Кроме того, используя фильтры по давно настроенным навыкам, вы ограничиваете количество доступных исполнителей.

{% endcut %}

{% cut "Обучение прошли более 500 исполнителей, но в тренировочном навыке отображается только 30" %}

В пуле отображается общее число исполнителей, которые выполнили там хотя бы одну страницу заданий. Тренировочный навык может со временем теряться из-за настройки повторного прохождения. Она позволяет заново выполнить тренировку по истечении указанного срока, если исполнитель так и не приступил к заданиям в привязанных пулах или сделал слишком большой перерыв в выполнении заданий (например, из-за [блокировки](../../glossary.md#banning-tolokers)). Поэтому в тренировочном навыке отображаются те исполнители, которые либо недавно завершили обучение, либо регулярно выполняют ваше задание и не дают навыку исчезнуть.

{% endcut %}

{% include [contact-support](../_includes/contact-support.md) %}