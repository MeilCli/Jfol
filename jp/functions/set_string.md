# setString
- 構文:
  - `$$setString("name",$value)`
    - 1つ目の引数:
      - 型: String
      - 説明: 追加するプロパティーの名前
    - 2つ目の引数:
      - 型: String
      - 説明: コピーする値
- 型:
  - StringまたはObject
- 説明:
  - 値のコピーをプロパティーに追加する

## 例
```json
{
  "value": "hello"
}
```

jfol:
```
$$setString("value2",$value)$$json
```

result:
```
{
    "value": "hello",
    "value2": "hello"
}
```