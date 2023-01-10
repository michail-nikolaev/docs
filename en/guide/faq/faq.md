# All questions on one page

{% note tip %}

If you are looking for the answer to a specific question, use **Ctrl+F** to search the page (**Cmd+F** on MacOS).

{% endnote %}

## Registration and getting started {#register-and-start}

{% include [faq-change-account-type](../_includes/faq/register-and-start/change-account-type.md) %}

{% cut "How do I change the phone number in my account?" %}

To change your phone number, go to [Yandex ID]({{ phones }}) and change your main number.

{% note info %}

If you don't have access to the old number, it takes a month to replace it. For more information about changing the phone number, see [Yandex ID Help]({{ change-phone }}).

{% endnote %}

{% endcut %}

## Sandbox {#sandbox}

{% include [faq-work-with-sandbox](../_includes/faq/sandbox/work-with-sandbox.md) %}

{% include [faq-see-pool-as-toloker](../_includes/faq/sandbox/see-pool-as-toloker.md) %}

{% include [faq-check-mobile-version](../_includes/faq/sandbox/check-mobile-version.md) %}

{% include [faq-copy-from-sandbox](../_includes/faq/sandbox/copy-from-sandbox.md) %}

{% include [faq-move-control-tasks](../_includes/faq/sandbox/move-control-tasks.md) %}

{% include [faq-same-account](../_includes/faq/sandbox/same-account.md) %}

## Setting up a project {#project}

### Instructions {#instruction}

{% include [faq-show-instructions](../_includes/faq/project-settings/show-instructions.md) %}

{% include [faq-video-player](../_includes/faq/project-settings/video-player.md) %}

{% include [faq-different-instructions](../_includes/faq/project-settings/different-instructions.md) %}

### Configuring the task interface {#concept_gss_fkp_smb}

{% include [faq-image-expand](../_includes/faq/project-settings/image-expand.md) %}

{% include [faq-shortcut](../_includes/faq/project-settings/shortcut.md) %}

{% include [faq-loading-audio-files](../_includes/faq/project-settings/loading-audio-files.md) %}

{% include [faq-mobile-task-display](../_includes/faq/project-settings/mobile-task-display.md) %}

{% include [faq-different-numbers](../_includes/faq/project-settings/different-numbers.md) %}

{% include [faq-add-text](../_includes/faq/project-settings/add-text.md) %}

{% include [faq-hide-expandable](../_includes/faq/project-settings/hide-expandable.md) %}

{% include [faq-pass-value](../_includes/faq/project-settings/pass-value.md) %}

{% include [faq-link-not-required](../_includes/faq/project-settings/link-not-required.md) %}

{% include [faq-checkbox-selected](../_includes/faq/project-settings/checkbox-selected.md) %}

{% include [faq-calendar](../_includes/faq/project-settings/calendar.md) %}

{% include [faq-make-tasks](../_includes/faq/project-settings/make-tasks.md) %}

{% include [faq-deselect-radio](../_includes/faq/project-settings/deselect-radio.md) %}

{% include [faq-show-photo](../_includes/faq/project-settings/show-photo.md) %}

{% include [faq-prevent-adding-photos](../_includes/faq/project-settings/prevent-adding-photos.md) %}

{% include [faq-setsolution](../_includes/faq/project-settings/setsolution.md) %}

{% include [faq-different-areas](../_includes/faq/project-settings/different-areas.md) %}

{% include [faq-vue-markup](../_includes/faq/project-settings/vue-markup.md) %}

{% include [faq-side-by-side](../_includes/faq/project-settings/side-by-side.md) %}

{% include [faq-change-background](../_includes/faq/project-settings/change-background.md) %}

{% include [faq-validate-data](../_includes/faq/project-settings/validate-data.md) %}

{% include [faq-assigment-validation](../_includes/faq/project-settings/assigment-validation.md) %}

{% include [faq-line-by-line](../_includes/faq/project-settings/line-by-line.md) %}

{% include [faq-sliders](../_includes/faq/project-settings/sliders.md) %}

{% include [faq-expand-window](../_includes/faq/project-settings/expand-window.md) %}

{% include [faq-use-input-data](../_includes/faq/project-settings/use-input-data.md) %}

{% include [faq-display-formatted-text](../_includes/faq/project-settings/display-formatted-text.md) %}

{% include [faq-use-own-js](../_includes/faq/project-settings/use-own-js.md) %}

{% include [faq-variable-number](../_includes/faq/project-settings/variable-number.md) %}

{% include [faq-implement-prettifier](../_includes/faq/project-settings/implement-prettifier.md) %}

{% include [faq-display-text](../_includes/faq/project-settings/display-text.md) %}

{% include [faq-no-selectable-object](../_includes/faq/project-settings/no-selectable-object.md) %}

### Input and output data {#concept_cjj_gkp_smb}

{% include [faq-insert-function](../_includes/faq/project-settings/insert-function.md) %}

{% include [faq-add-mask](../_includes/faq/project-settings/add-mask.md) %}

{% include [faq-need-convert](../_includes/faq/project-settings/need-convert.md) %}

{% include [faq-output-data](../_includes/faq/project-settings/output-data.md) %}

## Setting up a pool {#pool-settings}

### Filters {#filters}

{% cut "Can I select Tolokers from a specific city of residence or is the only option “Region by IP”?" %}

Yes, you can do that. In the [filters](../concepts/filters.md), select {% if locale == "en-com" %}**Profile → City**{% endif %}. Please note that the profile data is entered by the Toloker when they register in Toloka. We recommended that you use the filters **Region by phone number** and **Region by IP**.

{% endcut %}

{% cut "Can I use a skill beyond a particular pool or project and apply it to other projects as well?" %}

Yes, of course — you can use the same skill for different projects. But most often, a skill is intended for a specific project. If the Toloker completes a certain task well, this doesn't mean that they will complete other ones successfully. Another disadvantage is that if you filter by skills that were set long ago, you will artificially limit the number of available Tolokers.

{% endcut %}

{% cut "I want to calculate a skill based on performance in multiple projects. Is that possible? If it is, can I use “Aggregation by skill”?" %}

If you mean multiple different projects, you can't do that.

You can merge all the projects into one and use **History size** in the quality control rules. See examples in the [Control tasks](../concepts/goldenset.md) post.

You can use **Aggregation by skill**, but you'll need to list all the possible values, which is probably not the best choice. Perhaps you'll find [another method of aggregation](../concepts/result-aggregation.md) helpful.

{% endcut %}

{% cut "Are there any easy ways to assign a certain user a skill in Toloka, even if the Toloker didn't do any tasks (like I can do in the Sandbox)?" %}

In the main Toloka version, you can only assign a skill to users who have completed at least one of your tasks. There is no option to assign a skill to an arbitrary user. To limit the audience of users who will see your project, use [filters](../concepts/filters.md). For example, specify the city, date of birth, gender, or some other parameters of your target Tolokers.

{% endcut %}

{% cut "Can I somehow limit the number of users that can take tasks from the pool at the same time?" %}

Tasks from an open pool are available to every user that matches your pool [filters](../concepts/filters.md). You can restrict access, like by using a skill.

{% endcut %}

{% cut "Which parameter affects skill expiration?" %}

The validity period of the training skills is controlled by the **Retry after** parameter. The skill is deleted after a period specified in days in the **Retry after** field, if the Toloker:

- Has a skill value lower than the one specified in the **Level required** field.

- Didn't complete any tasks linked to training during this period.

Your users will need to be trained again.

{% endcut %}

{% cut "Can I add an arbitrary user as a Toloker?" %}

If the Toloker mismatches your preset filter, they can't see the task. You can only remove the restricting filter from the pool. You can test the task in the [Sandbox](../concepts/sandbox.md) by adding the desired user to your trusted list.

{% endcut %}

{% cut "Can I set up a task to display it to users with certain demographic and geo parameters? For example, “Moscow only, 30–45 years old”." %}

You can do that. To select Tolokers for the pool, use [filters](../concepts/filters.md).

{% endcut %}

{% cut "How do I make the task available not only from desktops, but also from mobile devices?" %}

Tasks in pools are automatically available in the web version of Toloka and the mobile app. Check the pool settings. You might have the `Client = Mobile Toloka`[filter](../concepts/filters.md) on.

{% endcut %}

{% cut "Can I select specific Tolokers for my tasks because I liked their results in my previous pools?" %}

You can assign a skill to these people based on their performance in the previous pools. Use this skill as a [filter](../concepts/filters.md) in the new pool.

{% endcut %}

{% cut "How do I set up a filter so that the pool is available to users who don't have a specific skill (like a “spammer”)?" %}

Specify this skill as a [filter](../concepts/filters.md), but leave the value field empty (this is equivalent to absence of the skill).

{% endcut %}

{% cut "How can I raise the skill value for a user, if they already have the skill?" %}

If the Toloker already has a given skill, you can't add the same skill to them from the task review interface. You can open the Toloker's profile and edit the skill value.

{% endcut %}

{% cut "Can Toloka users see that they were assigned a skill?" %}

If it's a public or training skill, they see it and they get a message about it.

{% endcut %}

{% cut "Can I show a skill in the task interface?" %}

There is no such option. If the skill is public, the Toloker sees it in their profile.

{% endcut %}

{% cut "Why can't I find the Toloker's gender in the Toloker data, although I can filter people by this attribute in the pool settings?" %}

Requesters can't see the full details about specific Tolokers. So you can't see information like the date of birth, gender, last name, or first name. However, you can use filters by date of birth and gender (in the pool settings). This way you can select a group of Tolokers without accessing the personal information of individual Tolokers. This decreases the risk of user de-anonymization.

{% endcut %}

{% cut "How do I automatically assign skills based on user responses to my questions?" %}

You can do that using the [Control tasks](../concepts/goldenset.md) rule.

1. Upload the task file using **Smart mixing**.

1. Specify `student` as the correct answer to the question. Don't take other questions into account (leave the fields empty or unselected).

1. Add the [Control tasks](../concepts/goldenset.md) rule to the pool: `if the percentage of correct control answers = 100, then set the skill value Student = 1`.

{% endcut %}

{% cut "See the screenshot" %}

![](../_images/troubleshooting/set-questionnaire-skill-student.png)

{% endcut %}

### Quality control {#quality-control}

{% cut "How do I set quality control in a pool correctly?" %}

The settings for [quality control](../../glossary.md#quality-control) rules depend on the type of tasks. General recommendations:

- Always use one or more ways to control quality of answers.

- Counting [fast responses](../concepts/quick-answers.md) makes sense for most tasks.

- If the Toloker has to choose between options (for example, by selecting checkboxes), check the answers using [majority vote](../concepts/mvote.md) or [control tasks](../concepts/goldenset.md).

- If the Toloker has to provide a response as a text or link or upload a photo, the best way to control quality is by [reviewing assignments](../concepts/accept.md). You can outsource task acceptance to Tolokers. Create a task with a question (for example, “Is this phrase translated correctly?”) and possible responses (for example, “yes”/“no”). Set up [overlap](../concepts/dynamic-overlap.md) and [majority vote](../concepts/mvote.md) check.

- If a task is more like an opinion poll (for example, choosing nice pictures from a set), [majority vote](../../glossary.md#majority-vote) is not a good way to control quality. Make [control tasks](../../glossary.md#control-task) with artificial examples where the choice is evident.

{% endcut %}

{% cut "How many control tasks do I need to add?" %}

We recommend adding at least 1% of control tasks in the pool. And for small pools — 5–10%.

{% cut "Why's that?" %}

Each control task is shown to the Toloker only once. If you use smart mixing, you determine how many control tasks should be in a suite. If each suite contains one control task, then the maximum number of suites the Toloker can complete is equal to the number of control tasks in the pool. If you increase the number of control tasks in a suite, the number of suites available to the Toloker decreases by the same number.

There shouldn't be too few pages available. Otherwise:

- You won't be able to correctly evaluate the quality of the Toloker's responses.

- The Toloker won't be interested in completing such tasks because they'll spend a lot of time studying instructions but won't earn much.

{% cut "Example" %}

#### A large pool with 1% of control tasks (good)

There are 10,000 tasks in the pool, and 100 of them are control tasks (1%). Each suite contains 10 tasks, and 1 of them is a control task. Hence, a user can complete up to 100 suites.

#### A small pool with 1% control tasks (bad)

There are 100 tasks in the pool, and 1 of them is a control task (1%). Each suite contains 10 tasks, and 1 of them is a control task. Hence, each user can only complete 1 suite.

#### A small pool with 10% control tasks (good)

There are 100 tasks in the pool, and 10 of them are control tasks (10%). Each suite contains 10 tasks, and 1 of them is a control task. Hence, each user can complete up to 100 suites

{% endcut %}

{% endcut %}

If there are few control tasks in the open pool, [add new control tasks](pool-setup.md#add-gs).

{% cut "What for" %}

In a large pool with few control tasks, a situation might occur when users who have completed a lot of tasks in the project stop getting new task suites. This happens when the Toloker completes all control tasks in the pool.

{% endcut %}

{% note info %}

To filter out Tolokers, use the [Control tasks](../concepts/control.md) quality control rule. To rank Tolokers by the quality of responses in control tasks, use a [skill](../concepts/nav.md).

{% endnote %}

{% endcut %}

{% cut "How do I add new control tasks to an open pool?" %}

To make new task suites available to all users, including those who have already completed tasks in this pool:

1. Stop the pool.

1. [Upload the file](../concepts/task_upload.md) with new control tasks.

1. Start the pool.

For open pools, we don't recommend creating control tasks from other types of tasks that have already been completed. This is because users who have already given their responses to them won't be able to re-complete such tasks as control tasks. In order for these users to continue completing task suites, the control tasks in the pool must be new.

{% endcut %}

{% cut "How are the correct responses to control questions counted?" %}

The Control tasks rule starts working after the Toloker completes the number of control tasks you specified. If your pool contains both [training](../../glossary.md#training-task) and control tasks, you can take into account the responses in both of them (the **Number of responses** parameter) or only in control tasks (the **Number of control responses** parameter).

As soon as the needed number of responses is collected, Toloka calculates the percentage of correct and incorrect responses and performs an action (assigns a skill, or blocks the Toloker in the pool or in the project). Then this percentage is updated as the tasks are completed by the Toloker. The number of the Toloker's recent responses that's used in the calculation is set in the **Recent control task responses to use** field. If you leave it empty, all the responses from the Toloker in the pool are counted.

{% endcut %}

{% cut "Should I create a skill for every pool?" %}

It is better to use one [skill](../../glossary.md#skill) in a project. You can choose the way to calculate the skill:

- Calculate the skill for each pool separately. The current skill value is the value of the skill in the pool the Toloker completed last. This option is convenient if:

    - The pools are intended for different groups of Tolokers (for example, there are filters by city or country).

    - Pools are started one by one and you don't want to take into account the responses in the previous pools to calculate the skill in the current pool.

    This calculation method is used by default when adding a quality control rule to a pool. For the control tasks block, leave the **Recent control task responses to use** field empty.

- Calculate skill based on all tasks in a project This option is good if the pools are small and you don't need to have skill calculated for each pool.

    This option is available only for skills on control tasks. To use it, fill in the **Recent control task responses to use** field in pool quality control rules.

{% endcut %}

{% cut "Can I make my training or control tasks totally different from the general tasks?" %}

Your [training](../concepts/train.md) and control tasks have the same project specification. However, you can create a separate project with the tasks and assign a skill based on user responses. Then you can admit Tolokers to the main project based on their skill.

{% endcut %}

{% cut "Isn't the exam a regular pool that I pay for? How does it differ from a regular pool?" %}

An exam pool contains only control tasks. It's usually small and used for checking how well users learned to do your tasks after they read the instructions and completed the [training](../concepts/additionals-q.md#selection). Unlike your main pool, you already know the correct responses for every task in this pool. You can set the price to zero.

Based on the results of responses to control tasks, you can assign a skill to the Tolokers and then specify it in the main pool as a filter. For example, `MySkill = 80 or = Is missing`. You don't have to create an exam. For simple tasks, the training pool provides enough practice, but many requesters also use exams.

{% endcut %}

{% cut "Is the time specified per task suite in the fast response settings?" %}

Yes, the [fast response](../concepts/quick-answers.md) settings specify the time per task suite.

{% endcut %}

{% cut "I set up a rule to ban users after the first incorrect captcha. This is to eliminate any bots. Is this too strict? What rule do most projects use?" %}

Indeed, this rule is probably too strict. Even the most careful user can make a mistake, so you probably want to relax the rule. Besides the requester-specific bans, we have system processes that ban users who regularly fail captcha checks in Toloka.

{% endcut %}

{% cut "The pool has an overlap and majority vote set up, but some fraudulent user opens the task suites, does nothing, and submits empty assignments. Could this cheater get more tasks from the pool before the results of other Tolokers are known? Could a user quickly click through a lot of task suites before the majority vote is accumulated to ban the cheater?" %}

Yes, unfortunately, this can happen. This is why we recommend that you offer a training task or exam before the general task. In this case, only those people who showed good performance at the previous stage are selected for the main pool.

{% endcut %}

{% cut "How do I set up an exam so that different people can take it without running out of tasks?" %}

When you load tasks, use smart mixing. In this case, you'll have infinite overlap in your exam.

However, this poses the risk that you might spend a lot of money on the exam. You might want to open this pool only when the main pool opens, and close it when labeling of the main pool ends.

{% endcut %}

{% cut "How do I test users to determine which kinds of tasks they do better and assign them relevant tasks?" %}

You can add a [training pool](../concepts/train.md) to test your Tolokers. Based on the test results, assign skills to the Tolokers for the tasks they do best.

Then open your pools only to the Tolokers that have a certain skill: use [filters](../concepts/filters.md) for this.

{% endcut %}

{% include [faq-using-smart-mixing](../_includes/faq/adding-tasks-to-the-pool/using-smart-mixing.md) %}

{% cut "If a cheating Toloker gives a lot of incorrect responses, and the system eventually bans them for errors in control tasks, do I have to pay for the bad responses anyway?" %}

If the Toloker already got paid for the tasks, the money can't be refunded to you.

{% endcut %}

{% cut "Can I control the frequency of showing captchas to the Tolokers? Some Tolokers get a bit demotivated by that." %}

The frequency of issuing [captchas](../concepts/captcha.md) is set up in the pool.

No

: Don't show captchas.

Low

: Show a captcha after every 20 assignments.

Average/High

: Show a captcha after every 10 assignments.

{% endcut %}

{% cut "Can one Toloker get access to two pools in the same project? Can I avoid that?" %}

Yes, if they can access both pools, they can do both of them. To restrict access to subsequent tasks for a Toloker, use the [Completed tasks](../concepts/submitted-answers.md) rule and select a ban at the project level.

{% endcut %}

{% cut "If I ban a Toloker for doing my tasks too fast, will all their responses be deleted and given to other Tolokers for labeling?" %}

No. The responses of these Tolokers aren't automatically excluded from the final results file.

But you can do it yourself if you want. When downloading the results, select the option **Exclude assignments by banned users** to delete the responses of Tolokers who were banned at the moment of downloading. You can also forward all the assignments from banned users to other Tolokers using the [Re-completion of assignments from banned users](../concepts/restore-task-overlap.md) rule.

{% endcut %}

{% cut "Can I create two active training pools, one for practice and the other for admitting users to the main pool? In other words, one pool is for users to practice and the other pool tests them." %}

Yes, you can do that. In this case, create the first pool based on the [training pool](../../glossary.md#training-pool) and the exam pool based on your main pool. If a pool contains only control and/or training tasks, the price can be set to zero.

In the exam pool, you can create a skill reflecting the exam result and granting admission to the main pool. For example, `if the number of responses is ≥ 10, set the skill value in the <exam skill> as % of correct responses`. In your exam pool user requirements, specify: `<exam skill> < 80 or = Is missing>`. In the main pool, set up a filter: `<exam skill> >= 80 and (<main skill> >= 70 or = Is missing)`. You can choose the skill values depending on how well the Tolokers handle your task.

{% endcut %}

{% cut "Can I get more details on the best practices for using captchas? For which projects is it better to use captchas and how often?" %}

[Captcha](../concepts/captcha.md) is usually used in simple projects with automatic acceptance, like classification, categorization, or information search. These are cases where there are few response options and users don't need to upload files or write texts. It helps you filter out bots and sloppy Tolokers.

The frequency of issuing captchas is configured in the pool.

No

: Don't show captchas.

Low

: Show a captcha after every 20 assignments.

Average/High

: Show a captcha after every 10 assignments.

{% endcut %}

{% cut "I found the following terms related to captcha in Help: “Percentage of correct responses” and “Percentage of incorrect responses”. Are they determined from the control sample?" %}

The percentage of correct responses is based on the total number of captchas processed by the Toloker within the “range” specified in the **Recent control task responses to use** field. If the value is empty, the percentage is calculated using all the captchas that are shown for the tasks in the pool which uses the captcha rule.

{% endcut %}

{% cut "My task uses a form with multiple fields. When there is an overlap and “Majority vote” is used for quality control, is each field taken into account, or if one field mismatches the majority vote, are the task results considered incorrect?" %}

All responses to the task are taken into account. If one response differs from the majority vote, the whole task is counted as mismatching the responses of other Tolokers.

{% endcut %}

{% cut "Have I understood correctly that if I use `set the the skill value = 1` with the `percentage of accepted responses >= 75` and `10 recent values to use`, for every 8 correctly completed tasks out of 10 the Toloker is given 1 skill point?" %}

No, this is incorrect. With these settings, each time a rule condition is met, the Toloker gets `skill = 1`. To change the skill value in the process of task review, you need a “multi-step” rule, which has multiple identical rules with different values of **Total reviewed responses**.

{% endcut %}

{% cut "Can I use non-automatic acceptance in the training pool?" %}

No. But you can create a pool of the **Training** type based on your main pool and enable non-automatic acceptance there.

{% endcut %}

{% cut "Can the Tolokers see which questions are control tasks?" %}

No, they can't.

{% endcut %}

{% cut "I have two text versions that I want to show to my respondents: one version to half of the audience, and another version to the other half (like in A/B testing). Is this possible in Toloka, or do I need to create two separate projects?" %}

If you pass texts to the input data, you can load 2 different tasks in the pool. In one task, pass Text 1 in the `INPUT: <input field name>` field, and in the other task, use this field to pass Text 2. But if the text is in the HTML block of the task template, you need to clone the project. To let a Toloker do only one task in your project, use the [Submitted responses](../concepts/submitted-answers.md) rule. You can assign a skill or ban the Toloker after they submit one response.

{% endcut %}

{% cut "If I ban users from my project so that everyone can complete a maximum of one task, are the Tolokers notified of the ban?" %}

No, the Tolokers are unaware of the ban.

{% endcut %}

{% cut "What output format do I use for the review results to filter out mismatching users based on the “Majority vote”?" %}

To perform actions with users (assign a skill or ban them) based on the majority vote, add a relevant [rule](../concepts/mvote.md) to the pool.

Don't forget to enable **Keep task order** in the pool parameters. Majority vote is used in the projects with preset options (radio buttons or checkboxes). This rule won't apply to the text entry or file upload fields.

{% endcut %}

{% cut "In the section about control questions, does "Number of control responses" mean the total number of responses to control questions (including incorrect responses) or the number of correct responses to my control questions?" %}

This is the total number of responses to the control questions.

{% endcut %}

{% cut "How do I classify users as good Tolokers and poor Tolokers as they complete tasks, and ban the poor Tolokers?" %}

You can create a task pool for all your Tolokers and create Toloker skills in it. In this case, you can open your tasks only to the Tolokers with the necessary skills.

{% endcut %}

{% cut "How can I speed up the pool completion?" %}

- To motivate Tolokers, assign a [public skill](../concepts/nav-create.md#public) and use [dynamic pricing](../concepts/dynamic-pricing.md).

- Try to [increase the project rating](../concepts/project_rating_stat.md), so that your task is higher in the list of tasks for Tolokers.

- Adjust the [quality-speed ratio](../concepts/adjust.md).

- Set a higher [priority](../concepts/pool_poolparams.md#priority) for the pool among other project pools.

{% endcut %}

### Overlap {#overlap}

{% cut "What overlap should I set?" %}

Overlap defines how many Tolokers complete the same pool task.

The best overlap is an overlap that provides satisfying quality of results. For most tasks that are not [reviewed](../../glossary.md#assignment-review), overlap from “3” to “5” is enough. If the tasks are simple, overlap of “3” is likely to be enough. For tasks that are reviewed, set overlap to “1”.

{% endcut %}

{% cut "Can I change overlap after the pool is started?" %}

Yes. [Open edit mode for the pool](../concepts/pool-edit.md) and set a new overlap value. You don't need to restart the pool. Updating the settings is usually fast, but if there are many tasks, it may take several minutes.

{% endcut %}

{% cut "With dynamic overlap, is it possible that the pool will close before the tasks for minimal overlap run out? The overlap increased, but the pool is closed, and I need to start it manually." %}

Yes, this might happen. You must set an adequate pool closing interval.

{% endcut %}

{% cut "How does counting work if I set `overlap = 3` in the pool and `response threshold = 3` in the majority vote?" %}

In this case, if you don't have 3 identical responses for your task (response threshold), no user would be considered a good or poor Toloker, because the system can't see which of the Tolokers made an error.

But if you set `response threshold = 2` with `overlap = 3`, then two users with the same responses are considered good Tolokers, but the third user, who gives a different response, is a poor Toloker.

{% endcut %}

{% cut "Can I do it like this: set a basic overlap of 2 users, then, if both Tolokers select the same response, close the pool, but if they give different responses, show the task to one more user?" %}

Yes, you can do that. Set up [dynamic overlap](../concepts/dynamic-overlap.md) (incremental relabeling, IRL).

{% endcut %}

{% cut "Is there a cross-check feature for tasks?" %}

You can use overlap to let multiple Tolokers do the same task. The overlap value is set up in the [pool settings](../concepts/pool-edit.md).

{% endcut %}

{% cut "Why is the maximum number of submitted assignments in the progress bar less than the total number of uploaded tasks?" %}

The progress bar shows the number of task suites including the overlap. If the overlap is greater than one, the number of task suites is different from the total number of tasks.

{% endcut %}

## Adding tasks to a pool {#add-task-to-pool}

### Uploading tasks {#concept_iy1_3kh_5mb}

{% include [faq-how-many-tasks-in-suite](../_includes/faq/adding-tasks-to-the-pool/how-many-tasks-in-suite.md) %}

{% include [faq-right-time-limit](../_includes/faq/adding-tasks-to-the-pool/right-time-limit.md) %}

{% include [faq-how-many-tasks-toloker-will-see](../_includes/faq/adding-tasks-to-the-pool/how-many-tasks-toloker-will-see.md) %}

{% include [faq-upload-accepted-assignments](../_includes/faq/adding-tasks-to-the-pool/upload-accepted-assignments.md) %}

{% include [faq-how-hint-displayed](../_includes/faq/adding-tasks-to-the-pool/how-hint-displayed.md) %}

{% include [faq-add-your-text-here](../_includes/faq/adding-tasks-to-the-pool/add-your-text-here.md) %}

{% include [faq-create-task-file-properly](../_includes/faq/adding-tasks-to-the-pool/create-task-file-properly.md) %}

{% include [faq-max-number-per-suite](../_includes/faq/adding-tasks-to-the-pool/max-number-per-suite.md) %}

{% include [faq-tasks-sensitive-to-order](../_includes/faq/adding-tasks-to-the-pool/tasks-sensitive-to-order.md) %}

{% include [faq-multiple-known-solutions](../_includes/faq/adding-tasks-to-the-pool/multiple-known-solutions.md) %}

{% include [faq-where-is-file-added](../_includes/faq/adding-tasks-to-the-pool/where-is-file-added.md) %}

{% include [faq-array-input-file](../_includes/faq/adding-tasks-to-the-pool/array-input-file.md) %}

{% cut "How do I properly structure my file used for data upload if there is JSON data among the input?" %}

All the values are written to the same column. Make sure to escape quotes. For more information about escaping quotes in JSON format, see the [Guide](../concepts/pool_csv.md#json).

{% endcut %}

{% include [faq-missing-headers](../_includes/faq/adding-tasks-to-the-pool/missing-headers.md) %}

{% include [faq-link-golden-field](../_includes/faq/adding-tasks-to-the-pool/link-golden-field.md) %}

{% include [faq-smart-mixing](../_includes/faq/adding-tasks-to-the-pool/smart-mixing.md) %}

{% include [faq-task-suite-difference](../_includes/faq/adding-tasks-to-the-pool/task-suite-difference.md) %}

{% cut "How do I view the processing log?" %}

To view the processing log, click **More on uploading errors**. The processing log is written in JSON format. Objects inside `result` match the line number of the uploaded file. Lines that were processed with an error have the status `"success": false`.

{% note info %}

To work with a large log conveniently, copy it to the text editor.

{% endnote %}

{% endcut %}

{% include [faq-two-versions-text](../_includes/faq/adding-tasks-to-the-pool/two-versions-text.md) %}

### Training-exam-retry {#concept_i2g_kkh_5mb}

{% include [faq-precede-with-control-questions](../_includes/faq/adding-tasks-to-the-pool/precede-with-control-questions.md) %}

{% include [faq-exam-main-pool](../_includes/faq/adding-tasks-to-the-pool/exam-main-pool.md) %}

{% include [faq-skill-expiration](../_includes/faq/adding-tasks-to-the-pool/skill-expiration.md) %}

{% include [faq-optional-parameters](../_includes/faq/adding-tasks-to-the-pool/optional-parameters.md) %}

{% include [faq-particular-toloker-got-skill](../_includes/faq/adding-tasks-to-the-pool/particular-toloker-got-skill.md) %}

{% cut "How do I insert a link in the GOLDEN field?" %}

Text in the GOLDEN field must match the control text exactly.

Usually, if you copy site links from the browser, the copied links have the same format. But this is not the case when the link is trimmed or typed manually.

Check the links that you use. There are several ways to unify links:

- Add requirements for the link format in your instructions and hints in your training pool.

- Use RegExp in your JS to trim the received links and write the result to the new output field, and then match the received value against the control value.

{% endcut %}

{% include [faq-using-smart-mixing](../_includes/faq/adding-tasks-to-the-pool/using-smart-mixing.md) %}

{% include [faq-pause-accepting](../_includes/faq/adding-tasks-to-the-pool/pause-accepting.md) %}

{% include [faq-check-during-training](../_includes/faq/adding-tasks-to-the-pool/check-during-training.md) %}

{% include [faq-two-training-pools](../_includes/faq/adding-tasks-to-the-pool/two-training-pools.md) %}

{% include [faq-admitted-to-general-task](../_includes/faq/adding-tasks-to-the-pool/admitted-to-general-task.md) %}

{% include [faq-all-tasks-training-pool](../_includes/faq/adding-tasks-to-the-pool/all-tasks-training-pool.md) %}

{% include [faq-retry](../_includes/faq/adding-tasks-to-the-pool/retry.md) %}

{% include [faq-optional-training](../_includes/faq/adding-tasks-to-the-pool/optional-training.md) %}

{% include [faq-manual-review-training](../_includes/faq/adding-tasks-to-the-pool/manual-review-training.md) %}

{% include [faq-training-without-correct-responses](../_includes/faq/adding-tasks-to-the-pool/training-without-correct-responses.md) %}

{% include [faq-exam-preset](../_includes/faq/adding-tasks-to-the-pool/exam-preset.md) %}

{% include [faq-training-with-exam](../_includes/faq/adding-tasks-to-the-pool/training-with-exam.md) %}

{% include [faq-file-with-training-tasks](../_includes/faq/adding-tasks-to-the-pool/file-with-training-tasks.md) %}

### Changing a running pool {#concept_olz_kkh_5mb}

{% include [faq-change-time-for-task](../_includes/faq/adding-tasks-to-the-pool/change-time-for-task.md) %}

{% include [faq-edit-uploaded-tasks](../_includes/faq/adding-tasks-to-the-pool/edit-uploaded-tasks.md) %}

{% include [faq-delete-one-of-file](../_includes/faq/adding-tasks-to-the-pool/delete-one-of-file.md) %}

## Working with results {#result-questions}

### Aggregation {#results}

{% include [faq-confidence-difference](../_includes/faq/result-questions/confidence-difference.md) %}

{% include [faq-how-dawid-skene-work](../_includes/faq/result-questions/how-dawid-skene-work.md) %}

{% include [faq-aggregation-progress](../_includes/faq/result-questions/aggregation-progress.md) %}

{% cut "Can I get notifications when results aggregation finishes?" %}

{% include [faq-notifications-results](../_includes/faq/result-questions/notifications-results.md) %}

{% endcut %}

### Processing the results file {#results_1}

{% include [faq-empty-text-field](../_includes/faq/result-questions/empty-text-field.md) %}

### Assignment review {#results_2}

{% include [faq-send-back](../_includes/faq/result-questions/send-back.md) %}

{% include [faq-disable-tasks](../_includes/faq/result-questions/disable-tasks.md) %}

{% include [faq-fix-myself](../_includes/faq/result-questions/fix-myself.md) %}

{% include [troubleshooting-pool-archived](../_includes/troubleshooting/result-questions/pool-archived.md) %}

{% include [troubleshooting-rejected-task](../_includes/troubleshooting/result-questions/rejected-task.md) %}

{% include [faq-reject-part](../_includes/faq/result-questions/reject-part.md) %}

{% include [faq-notify](../_includes/faq/result-questions/notify.md) %}

{% include [faq-increase-rating](../_includes/faq/result-questions/increase-rating.md) %}

### Statistics {#results_3}

{% include [faq-formula-for-calculation](../_includes/faq/result-questions/formula-for-calculation.md) %}

{% include [faq-expired-skipped](../_includes/faq/result-questions/expired-skipped.md) %}

{% include [faq-quality-stat](../_includes/faq/result-questions/quality-stat.md) %}

{% include [faq-get-time](../_includes/faq/result-questions/get-time.md) %}

## Archiving pools and projects {#pool-n-project-archive}

{% include [faq-delete-pool](../_includes/faq/pool-n-project-archive/delete-pool.md) %}

{% include [faq-pool-storage-time](../_includes/faq/pool-n-project-archive/pool-storage-time.md) %}

{% include [faq-where-closed-pool](../_includes/faq/pool-n-project-archive/where-closed-pool.md) %}

{% include [faq-pool-archiving-parameters](../_includes/faq/pool-n-project-archive/pool-archiving-parameters.md) %}

{% include [faq-accept-tasks-from-archived-pool](../_includes/faq/pool-n-project-archive/accept-tasks-from-archived-pool.md) %}

## Payments {#finance}

### Adding funds to your account {#concept-1}

{% include [faq-how-long-paying-invoice-take](../_includes/faq/finance/how-long-paying-invoice-take.md) %}

{% include [faq-currency-exchange-rate](../_includes/faq/finance/currency-exchange-rate.md) %}

{% include [faq-add-money](../_includes/faq/finance/add-money.md) %}

[Get closing documents and invoices](../troubleshooting/support.md)

[Refund money transferred to the Toloka account](../troubleshooting/support.md)

### Payment for tasks {#concept-2}

{% include [faq-set-task-price](../_includes/faq/finance/set-task-price.md) %}

{% include [faq-set-up-budget](../_includes/faq/finance/set-up-budget.md) %}

{% include [faq-pay-more-optional-fields](../_includes/faq/finance/pay-more-optional-fields.md) %}

{% include [faq-awards-statistics](../_includes/faq/finance/awards-statistics.md) %}

{% include [faq-tasks-with-different-prices](../_includes/faq/finance/tasks-with-different-prices.md) %}

## Tolokers {#annotators}

### Data about Tolokers {#user-info}

{% include [faq-information-about-tolokers](../_includes/faq/users/information-about-tolokers.md) %}

{% include [faq-verify-information](../_includes/faq/users/verify-information.md) %}

{% include [faq-know-id](../_includes/faq/users/know-id.md) %}

{% include [faq-filter-by-gender](../_includes/faq/users/filter-by-gender.md) %}

### Rewards {#bonuses}

{% include [faq-reward](../_includes/faq/users/reward.md) %}

{% include [faq-stat-rewards](../_includes/faq/users/stat-rewards.md) %}

### Cheaters {#cheaters}

{% include [faq-disable-tasks](../_includes/faq/result-questions/disable-tasks.md) %}

{% include [faq-redo-task](../_includes/faq/users/redo-task.md) %}

{% include [faq-fix-myself](../_includes/faq/result-questions/fix-myself.md) %}

{% include [faq-empty-response](../_includes/faq/users/empty-response.md) %}

{% include [faq-cheaters-paid](../_includes/faq/users/cheaters-paid.md) %}

{% include [troubleshooting-include-responses](../_includes/troubleshooting/users/include-responses.md) %}

{% include [faq-ban-and-reject](../_includes/faq/users/ban-and-reject.md) %}

## Questions about presets {#question-about-templates}

### Selecting a preset {#concept_tfh_pgd_rmb}

{% include [faq-complex-task](../_includes/faq/questions-about-templates/complex-task.md) %}

{% include [faq-input-output-text-fields](../_includes/faq/questions-about-templates/input-output-text-fields.md) %}

{% include [faq-text-classification](../_includes/faq/questions-about-templates/text-classification.md) %}

{% include [faq-irrelevant-products](../_includes/faq/questions-about-templates/irrelevant-products.md) %}

{% include [faq-elements-web-pages](../_includes/faq/questions-about-templates/elements-web-pages.md) %}

{% include [faq-validation-depending-checkbox](../_includes/faq/questions-about-templates/validation-depending-checkbox.md) %}

### Area selection {#concept_bdk_qgd_rmb}

{% include [faq-shortcut-adding-polygon](../_includes/faq/questions-about-templates/shortcut-adding-polygon.md) %}

{% include [faq-mark-triangles](../_includes/faq/questions-about-templates/mark-triangles.md) %}

{% include [faq-selecting-objects](../_includes/faq/questions-about-templates/selecting-objects.md) %}

{% include [faq-large-number-objects](../_includes/faq/questions-about-templates/large-number-objects.md) %}

{% include [faq-different-areas](../_includes/faq/questions-about-templates/different-areas.md) %}

{% include [faq-input-data-labeling-image](../_includes/faq/questions-about-templates/input-data-labeling-image.md) %}

{% include [faq-control-area-selection](../_includes/faq/questions-about-templates/control-area-selection.md) %}

### Field task {#concept_k1m_rgd_rmb}

{% include [faq-limit-source-photo](../_includes/faq/questions-about-templates/limit-source-photo.md) %}

### Side-by-side image comparison {#side-by-side}

{% include [faq-paired-images-comparison](../_includes/faq/questions-about-templates/paired-images-comparison.md) %}

## Survey {#interview}

{% include [faq-simple-survey](../_includes/faq/questions-about-templates/simple-survey.md) %}

{% include [faq-survey-single-question](../_includes/faq/questions-about-templates/survey-single-question.md) %}

### Field task {#concept_k1m_rgd_rmb}

{% include [faq-limit-source-photo](../_includes/faq/questions-about-templates/limit-source-photo.md) %}

{% include [contact-support](../_includes/contact-support.md) %}