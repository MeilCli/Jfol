# index
- syntax:
  - `$$index`
- type:
  - Number or String
- description:
  - return current index

**This function is special function, available in array body.**

## Example
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

jfol:
```
$array[index $$index value: $value$$separator[\n]]
```

return:
```
index 0 value: 1
index 1 value: 2
```