# Field

## Array

array field's value can flatten using `[]` body.

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
$array[$value]
```

output:

```
12
```

if raw value array, use `$$value` function.

json:

```json
{
  "array": [1, 2]
}
```

format:

```
$array[$$value]
```

output:

```
12
```
