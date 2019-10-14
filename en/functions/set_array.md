# setArray
- syntax:
  - `$$setArray("name",$value)`
    - first argument:
      - type: String
      - description: set to property name
    - second argument:
      - type: Array
      - description: value that copy
- type:
  - String or Array
- description:
  - set property to copied value

**This function's copy is reference copy, So if want to deep copy, use [copy function](copy.md).**

## Example
```json
{
  "value": [1, 2]
}
```

jfol:
```
$$setArray("value2",$value)$$json
```

result:
```
{
    "value": [
        1,
        2
    ],
    "value2": [
        1,
        2
    ]
}
```