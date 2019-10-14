# copy
- syntax:
  - `$$copy("name", $value)`
    - first argument
      - type: String
      - description: add property name to current context
    - second argument
      - type: Object, Array, Boolean, Number, Null or String
      - description: add value of deep copy of argument to property
- type:
  - String
- description:
  - deep copy property

## Example
```json
{
  "value": {
    "text": "world" 
  }
}
```

jfol:
```
$$copy("value2",$value)$$json
```

result:
```
{
    "value": {
        "text": "world"
    },
    "value2": {
        "text": "world"
    }
}
```