# Introduction
JSON Formation Language(Jfol)

Note: Experimental syntax

## Surmary
Jfol is created to easy for JSON transforming to JSON or Text.

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

jfol:
```
Packages Total: $$(array.length)
$array[$$index: $(package.name)$$separator[\n]]
```

result:
```
Packages Total: 2
0: pack1
1: pack2
```

## Playground
Jfol online runner is prepared on [This](https://meilcli.github.io/Jfol.TS/index.html).

You can try JSON transforming by Jfol