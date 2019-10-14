# value
- syntax:
  - `$$value`
- type:
  - if String value: String
  - if Number value: Number or String
  - if Boolean value: Boolean or String
  - if Null value: Null or String
- description:
  - get current context value

## Example
```json
{
  "array": [1, 2, 3]
}
```

jfol:
```
$array[$$value$$separator[\n]]
```

result:
```
1
2
3
```