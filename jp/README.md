# はじめに
JSON Formation Language(Jfol)

ノート: 実験的な構文です

## 概要
JfolはJSONを変換して簡単にJSONまたはTextを作成することができます

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

## 遊び場
[ここ](http://playground.jfol.meilcli.net/)でJfolのオンラインランナーが用意されています

JfolによるJSONの変換を試すことができます