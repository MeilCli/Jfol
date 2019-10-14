# delete
- syntax:
  - `$$delete("name")`
    - first argument:
      - type: String or Number
      - description: delete property or element of array from current context
- type:
  - String
- description:
  - delete property

## Example
```json
{
  "value": {
    "text": "world" 
  },
  "text": "hello"
}
```

jfol:
```
$$delete("text")$$json
```

result:
```
{
    "value": {
        "text": "world"
    }
}
```