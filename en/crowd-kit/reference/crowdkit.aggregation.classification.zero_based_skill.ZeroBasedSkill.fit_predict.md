# fit_predict
`crowdkit.aggregation.classification.zero_based_skill.ZeroBasedSkill.fit_predict` | [Source code](https://github.com/Toloka/crowd-kit/blob/v1.1.0/crowdkit/aggregation/classification/zero_based_skill.py#L126)

```python
fit_predict(self, data: DataFrame)
```

Fit the model and return aggregated results.

## Parameters Description

| Parameters | Type | Description |
| :----------| :----| :-----------|
`data`|**DataFrame**|<p>Workers&#x27; labeling results. A pandas.DataFrame containing `task`, `worker` and `label` columns.</p>

* **Returns:**

  Tasks' labels.
A pandas.Series indexed by `task` such that `labels.loc[task]`
is the tasks's most likely true label.

* **Return type:**

  Series
