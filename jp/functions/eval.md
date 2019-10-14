# eval
- 構文:
  - `$$eval($value)`
    - 1つ目の引数:
      - 型: Number, Boolean, NullまたはString
      - 説明: 計算する値
- 型:
  - String
- 説明:
  - 引数を計算する

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
$$eval("hello "+$(value.text))
```

result:
```
hello world
```