# noText
- 構文:
  - `$$noText[body]`
    - ボディー:
      - 現在のコンテキスト
- 型:
  - String
- 説明:
  - ボディーを実行しますがなにも出力しません

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
$$noText[
$$setString("text","hello")
]$$json
```

result:
```
{
    "value": {
        "text": "world"
    },
    "text": "hello"
}
```