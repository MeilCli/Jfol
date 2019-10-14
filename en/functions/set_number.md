# setNumber
- syntax:
  - `$$setNumber("name",$value)`
    - first argument:
      - type: String
      - description: set to property name
    - second argument:
      - type: Number
      - description: value that copy
- type:
  - String or Object
- description:
  - set property to copied value

## Example
```json
{
  "value": 1
}
```

jfol:
```
$$setNumber("value2",$value)$$json
```

result:
```
{
    "value": 1,
    "value2": 1
}
```