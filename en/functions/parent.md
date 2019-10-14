# parent
- syntax:
  - `$$parent[body]`
    - body:
      - parent context
- type:
  - String
- description:
  - execute body on parent context

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
$value[$$parent[$text]]
```

result:
```
hello
```