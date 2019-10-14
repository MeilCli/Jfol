# json
- syntax:
  - `$$json`
  - `$$json($value)`
    - first argument:
      - type: Array, Object, Number, Null, Boolean or String
      - description: output value
- type:
  - String
- description:
  - output json string of value or current context

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
$$json($value)
```

result:
```
{
    "text": "world"
}
```