# jdl
JSON Domain Language

## Surmary
json:
```json
{
    "array": [
        {
            "package": {
                "name": "pack1"
            }
        },
        {
            "package": {
                "name": "pack2"
            }
        }
    ]
}
```

format:
```
Packages Total: $$(array.length)\n$array[$$index: $(package.name)$$separator[\n]]
```

output:
```
Packages Total: 2
0: pack1
1: pack2
```

## Basic
some `$` means special operand.

- `$`: field accessor
- `$$`: function accessor
- `[]`: function or field body
- `.`: chain of function and field
  - such as `$(object.field)` or `$$(array.length)`
  
## Array
### foreach
array field's value can flatten using `[]` body.

json:
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

format:
```
$array[$value]
```

output:
```
12
```

if raw value array, use `$$value` function.

json:
```json
{
    "array": [
        1,
        2
    ]
}
```

format:
```
$array[$$value]
```

output:
```
12
```
