# where
- syntax: 
  - `$$where(condition)`
    - first argument:
      - type: Boolean
      - description: condition of execute array body
- type:
  - Boolean
- description:
  - control of where on array body

**This function is special function, available in array body. And enabled on anywhere on array body.**

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
$array[value: $value$$where($value==1)]
```

result:
```
value: 1
```