# delete_user_restriction
`toloka.client.TolokaClient.delete_user_restriction` | [Source code](https://github.com/Toloka/toloka-kit/blob/v1.1.0.post1/src/client/__init__.py#L3110)

```python
delete_user_restriction(self, user_restriction_id: str)
```

Unlocks existing restriction

## Parameters Description

| Parameters | Type | Description |
| :----------| :----| :-----------|
`user_restriction_id`|**str**|<p>Restriction that should be removed.</p>

**Examples:**


```python
toloka_client.delete_user_restriction(user_restriction_id='1')
```
