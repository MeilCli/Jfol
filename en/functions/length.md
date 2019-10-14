# length
- syntax:
  - `$$length`
- type:
  - Number or String
- description:
  - return array length or length property's value

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
Total: $$(array.length)\n$array[number $$number/$$length: $value$$separator[\n]]
```

result:
```
Total: 2
number 1/2: 1
number 2/2: 2
```