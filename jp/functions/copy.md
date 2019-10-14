# copy
- 構文:
  - `$$copy("name", $value)`
    - 1つ目の引数
      - 型: String
      - 説明: 現在のコンテキストに追加するプロパティーの名前
    - 2つ目の引数
      - 型: Object, Array, Boolean, Number, NullまたはString
      - 説明: プロパティにディープコピーで追加する値
- 型:
  - String
- 説明:
  - プロパティをディープコピーする

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
$$copy("value2",$value)$$json
```

result:
```
{
    "value": {
        "text": "world"
    },
    "value2": {
        "text": "world"
    }
}
```