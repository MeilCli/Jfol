# Jfol
JSON Formation Language

Note: Experimental syntax

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
- `()`: some function argument
- `[]`: function or field body
- `.`: chain of function and field
  - such as `$(object.field)` or `$$(array.length)`
  
## Object
### if
conditional value, use `$$if`.

json:
```json
{
    "name": "meil"
}
```

format:
```
Hello World$$if($name=="meil")[, MeilCli].
```

output:
```
Hello World, MeilCli.
```

  
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

### separator
simple foreach cannot set separator, so use `$$separator` function.

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
$array[$value$$separator[\n]]
```

output:
```
1
2
```

`$$separator` can define anywhere array field body.

that is, `$array[$value$$separator[\n]]` equals to `$array[$$separator[\n]$value]`.

### index
can get index of array in array field, use `$$index`.

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
$array[index $$index value: $value$$separator[\n]]
```

output:
```
index 0 value: 1
index 1 value: 2
```

### number
can get number(`index + 1`) of array in array field, use `$$number`.

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
$array[number $$number value: $value$$separator[\n]]
```

output:
```
number 1 value: 1
number 2 value: 2
```

### length
can get length of array as function in array function or body.

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
Total: $$(array.length)\n$array[number $$number/$$length: $value$$separator[\n]]
```

output:
```
Total: 2
number 1/2: 1
number 2/2: 2
```

### where
filter element, use `$$where`.

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
$array[value: $value$$where($value==1)]
```

output:
```
value: 1
```
