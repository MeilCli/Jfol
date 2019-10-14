# setObject
- syntax:
  - `$$setObject("name",$value)`
    - first argument:
      - type: String
      - description: set to property name
    - second argunmet:
      - type: Object
      - description: value that copy
- type:
  - String or Object
- description:
  - set property to copied value

**This function's copy is reference copy, So if want to deep copy, use [copy function](copy.md).**

## Example
```json
{
  "value": {
    "text": "hello"
  }
}
```

jfol:
```
$$setObject("value2",$value)$$json
```

result:
```
{
    "value": {
        "text": "hello"
    },
    "value2": {
        "text": "hello"
    }
}
```