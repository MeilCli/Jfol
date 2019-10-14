# setBoolean
- syntax:
  - `$$setBoolean("name",$value)`
    - first argument:
      - type: String
      - description: set to property name
    - second argument:
      - type: Boolean
      - description: value that copy
- type:
  - String or Object
- description:
  - set property to copied value

## Example
```json
{
  "value": true
}
```

jfol:
```
$$setBoolean("value2",$value)$$json
```

result:
```
{
    "value": true,
    "value2": true
}
```