# setNull
- syntax:
  - `$$setNull("name")`
    - first argument:
      - type: String
      - description: set to property name
- type:
  - String or Object
- description:
  - set property to null

## Example
```json
{
  "value": true
}
```

jfol:
```
$$setNull("value2")$$json
```

result:
```
{
    "value": true,
    "value2": null
}
```