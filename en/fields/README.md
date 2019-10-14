# Field
- syntax:
  - `$(object.value)[child context/*body is optional*/]`
  - `$value[child context/*body is optional*/]`
- type:
  - dynamic type when resolved.
  - can be Object, Array, String, Boolean, Number or Null type
  - if Boolean or Number or Null type, union of String and its type.

## Base type
```json
{
  "value": true
}
```

jfol:
```
$value
```

result:
```
true
```

## Object
```json
{
  "value": {
    "text": "world" 
  }
}
```

jfol:
```
$value[$text]
```
or
```
$(value.text)
```

result:
```
world
```

Object can have body, but can use dot connected identifiers.

## Array
```json
{
  "array": [
    {
      "value": 1
    },
    {
      "value": 2
    }
  ]
}
```

jfol:
```
$array[$value]
```

result:
```
12
```