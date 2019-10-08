# where

filter element, use `$$where`.

json:

```json
{
  "array": [
    {
      "value": 1
    },
    {
      "value": 2
    }
  ]
}
```

format:

```
$array[value: $value$$where($value==1)]
```

output:

```
value: 1
```