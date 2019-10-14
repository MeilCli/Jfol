# noText
- syntax:
  - `$$noText[body]`
    - body:
      - current context
- type:
  - String
- description:
  - execute body, but no-output

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
$$noText[
$$setString("text","hello")
]$$json
```

result:
```
{
    "value": {
        "text": "world"
    },
    "text": "hello"
}
```