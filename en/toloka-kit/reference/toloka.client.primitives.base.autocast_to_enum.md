# autocast_to_enum
`toloka.client.primitives.base.autocast_to_enum` | [Source code](https://github.com/Toloka/toloka-kit/blob/v1.1.0.post1/src/client/primitives/base.py#L306)

```python
autocast_to_enum(func: Callable)
```

Function decorator that performs str -> Enum conversion when decorated function is called


This decorator modifies function so that every argument annotated with any subclass of Enum type (including Enum
itself) can be passed a value of str (or any )

