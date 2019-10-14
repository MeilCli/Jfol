# separator
- syntax:
  - `$$separator[body]`
    - body:
      - current context(behind element)
- type:
  - String
- description:
  - array text's separator

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
$array[$value$$separator[\n]]
```

result:
```
1
2
```
