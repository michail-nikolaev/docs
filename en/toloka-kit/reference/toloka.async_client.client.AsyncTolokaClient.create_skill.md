# create_skill
`toloka.async_client.client.AsyncTolokaClient.create_skill` | [Source code](https://github.com/Toloka/toloka-kit/blob/v1.1.0.post1/src/client/__init__.py#L0)

Creates a new Skill


You can send a maximum of 10 requests of this kind per minute and 100 requests per day.

## Parameters Description

| Parameters | Type | Description |
| :----------| :----| :-----------|
`name`|**Optional\[str\]**|<p>Skill name.</p>
`private_comment`|**Optional\[str\]**|<p>Comments on the skill (only visible to the requester).</p>
`hidden`|**Optional\[bool\]**|<p>Access to information about the skill (the name and value) for Tolokers:</p> <ul> <li>True - Closed. Default behavior.</li> <li>False - Opened.</li> </ul>
`skill_ttl_hours`|**Optional\[int\]**|<p>The skill&#x27;s &quot;time to live&quot; after the last update (in hours). The skill is removed from the Toloker&#x27;s profile if the skill level hasn&#x27;t been updated for the specified length of time.</p>
`training`|**Optional\[bool\]**|<p>Whether the skill is related to a training pool:</p> <ul> <li>True - The skill level is calculated from training pool tasks.</li> <li>False - The skill isn&#x27;t related to a training pool.</li> </ul>
`public_name`|**Optional\[Dict\[str, str\]\]**|<p>Skill name for other Tolokers. You can provide a name in several languages (the message will come in the Toloker&#x27;s language).</p>
`public_requester_description`|**Optional\[Dict\[str, str\]\]**|<p>Skill description text for other Tolokers. You can provide text in several languages (the message will come in the Toloker&#x27;s language).</p>
`owner`|**Optional\[[Owner](toloka.client.owner.Owner.md)\]**|<p>Skill owner.</p>
`id`|**-**|<p>Skill ID. Read only field.</p>
`created`|**-**|<p>The UTC date and time when the skill was created. Read only field.</p>

* **Returns:**

  Created skill. With read-only fields.

* **Return type:**

  [Skill](toloka.client.skill.Skill.md)

**Examples:**

How to create a new skill.

```python
new_skill = toloka_client.create_skill(
    name='Area selection of road signs',
    public_requester_description={
        'EN': 'Tolokers annotate road signs',
        'FR': "Les Tolokers annotent les signaux routier",
    },
)
print(new_skill.id)
```