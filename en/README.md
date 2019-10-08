# Introduction

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