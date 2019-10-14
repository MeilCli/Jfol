# delete
- 構文:
  - `$$delete("name")`
    - 1つ目の引数:
      - 型: StringまたはNumber
      - 説明: 現在のコンテキストから削除するプロパティーまたは配列の要素
- 型:
  - String
- 説明:
  - プロパティーを削除する

## 例
```json
{
  "value": {
    "text": "world" 
  },
  "text": "hello"
}
```

jfol:
```
$$delete("text")$$json
```

result:
```
{
    "value": {
        "text": "world"
    }
}
```