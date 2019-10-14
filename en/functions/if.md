# if
- syntax:
  - `$$if($value)[body]`
    - first argument:
      - type: Boolean
      - description: conditional value, if true, execute body
    - body:
      - current context
- type:
  - String
- description: 
  - if control

## Example
```json
{
  "name": "meil"
}
```

jfol:
```
Hello World$$if($name=="meil")[, MeilCli].
```

result:
```
Hello World, MeilCli.
```