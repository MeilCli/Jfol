# setString
- syntax:
  - `$$setString("name",$value)`
    - first argument:
      - type: String
      - description: set to property name
    - second argunmet:
      - type: String
      - description: value that copy
- type:
  - String or Object
- description:
  - set property to copied value

## Example
```json
{
  "value": "hello"
}
```

jfol:
```
$$setString("value2",$value)$$json
```

result:
```
{
    "value": "hello",
    "value2": "hello"
}
```