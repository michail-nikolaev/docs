# AppItemImport
`toloka.client.app.AppItemImport` | [Source code](https://github.com/Toloka/toloka-kit/blob/v1.1.0.post1/src/client/app/__init__.py#L184)

```python
AppItemImport(
    self,
    *,
    id: Optional[str] = None,
    records_count: Optional[int] = None,
    records_processed: Optional[int] = None,
    errors: Optional[Dict] = None
)
```

Meta-information on asynchronous loading operation (possible via UI).

## Parameters Description

| Parameters | Type | Description |
| :----------| :----| :-----------|
`id`|**Optional\[str\]**|
`records_count`|**Optional\[int\]**|<p>Number of items in the loading operation.</p>
`records_processed`|**Optional\[int\]**|<p>Number of successfully loaded items in the loading operation.</p>
`errors`|**Optional\[Dict\]**|<p>Errors during the loading operation.</p>
