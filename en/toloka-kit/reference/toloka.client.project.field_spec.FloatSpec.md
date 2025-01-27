# FloatSpec
`toloka.client.project.field_spec.FloatSpec` | [Source code](https://github.com/Toloka/toloka-kit/blob/v1.1.0.post1/src/client/project/field_spec.py#L100)

```python
FloatSpec(
    self,
    *,
    required: Optional[bool] = True,
    hidden: Optional[bool] = False,
    min_value: Optional[float] = None,
    max_value: Optional[float] = None
)
```

An floating point field specification

## Parameters Description

| Parameters | Type | Description |
| :----------| :----| :-----------|
`required`|**Optional\[bool\]**|<p>Whether the object or input field is required.</p>
`hidden`|**Optional\[bool\]**|<p>Whether to hide the input field from Tolokers.</p>
`min_value`|**Optional\[float\]**|<p>Minimum value of the number</p>
`max_value`|**Optional\[float\]**|<p>Maximum value of the number</p>
