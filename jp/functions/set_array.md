# setArray
- 構文:
  - `$$setArray("name",$value)`
    - 1つ目の引数:
      - 型: String
      - 説明: 追加するプロパティーの名前
    - 2つ目の引数:
      - 型: Array
      - 説明: コピーする値
- 型:
  - StringまたはArray
- 説明:
  - 値のコピーをプロパティーに追加する

**この関数のコピーは参照のコピーです。そのためもしディープコピーをしたいのであれば[copy関数](copy.md)を使います**

## 例
```json
{
  "value": [1, 2]
}
```

jfol:
```
$$setArray("value2",$value)$$json
```

result:
```
{
    "value": [
        1,
        2
    ],
    "value2": [
        1,
        2
    ]
}
```