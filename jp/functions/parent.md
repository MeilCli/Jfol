# parent
- 構文:
  - `$$parent[body]`
    - ボディー:
      - 親のコンテキスト
- 型:
  - String
- 説明:
  - ボディーを親のコンテキストで実行します

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
$value[$$parent[$text]]
```

result:
```
hello
```