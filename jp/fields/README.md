# フィールド
- 構文:
  - `$(object.value)[子のコンテキストで実行/*ボディーはオプション*/]`
  - `$value[子のコンテキストで実行/*ボディーはオプション*/]`
- 型:
  - 解決されるときの動的な型
  - Object, Array, String, Boolean, NumberまたはNullになります
  - もしBooleanまたはNumberまたはNull型の場合はStringとの共用体型になります

## 基本型
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
または
```
$(value.text)
```

result:
```
world
```

Objectはボディーを持つことができますが、識別子をドットで繋げて利用することもできます

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