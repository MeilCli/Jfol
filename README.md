# jdl
JSON Domain Language

## Surmary
Json:
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

Format:
```
Packages Total: $$(array.length)\n$array[$$index: $(package.name)$$separator[\n]]
```

Output:
```
Packages Total: 2
0: pack1
1: pack2
```
