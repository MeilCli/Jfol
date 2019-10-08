# number

can get number(`index + 1`) of array in array field, use `$$number`.

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
$array[number $$number value: $value$$separator[\n]]
```

output:

```
number 1 value: 1
number 2 value: 2
```