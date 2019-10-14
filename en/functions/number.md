# number
- syntax:
  - `$$number`
- type:
  - Number or String
- description:
  - return current index+1

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
$array[number $$number value: $value$$separator[\n]]
```

result:
```
number 1 value: 1
number 2 value: 2
```