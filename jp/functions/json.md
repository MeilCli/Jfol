# json
- 構文:
  - `$$json`
  - `$$json($value)`
    - 1つ目の引数:
      - 型: Array, Object, Number, Null, BooleanまたはString
      - 説明: JSONとして出力する値
- 型:
  - String
- 説明:
  - 値または現在のコンテキストをJSONで出力する

## 例
```json
{
  "value": {
    "text": "world" 
  }
}
```

jfol:
```
$$json($value)
```

result:
```
{
    "text": "world"
}
```