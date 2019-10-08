# index

can get index of array in array field, use `$$index`.

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
$array[index $$index value: $value$$separator[\n]]
```

output:

```
index 0 value: 1
index 1 value: 2
```