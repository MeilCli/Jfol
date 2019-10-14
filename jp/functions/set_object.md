# setObject
- 構文:
  - `$$setObject("name",$value)`
    - 1つ目の引数:
      - 型: String
      - 説明: 追加するプロパティーの名前
    - 2つ目の引数:
      - 型: Object
      - 説明: コピーする値
- 型:
  - StringまたはObject
- 説明:
  - 値のコピーをプロパティーに追加する

**この関数のコピーは参照のコピーです。そのためもしディープコピーをしたいのであれば[copy関数](copy.md)を使います**

## 例
```json
{
  "value": {
    "text": "hello"
  }
}
```

jfol:
```
$$setObject("value2",$value)$$json
```

result:
```
{
    "value": {
        "text": "hello"
    },
    "value2": {
        "text": "hello"
    }
}
```