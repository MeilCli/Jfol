# eval
- syntax:
  - `$$eval($value)`
    - first argument:
      - type: Number, Boolean, Null or String
      - description: value that evaluate
- type:
  - String
- description:
  - evaluate argument

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
$$eval("hello "+$(value.text))
```

result:
```
hello world
```