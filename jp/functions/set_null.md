# setNull
- 構文:
  - `$$setNull("name")`
    - 1つ目の引数:
      - 型: String
      - 説明: 追加するプロパティーの名前
- 型:
  - StringまたはObject
- 説明:
  - プロパティーにnullを追加する

## 例
```json
{
  "value": true
}
```

jfol:
```
$$setNull("value2")$$json
```

result:
```
{
    "value": true,
    "value2": null
}
```