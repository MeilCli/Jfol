# separator
- 構文:
  - `$$separator[body]`
    - ボディー:
      - 現在のコンテキスト(後ろの要素)
- 型:
  - String
- 説明:
  - 配列のテキストの区切り文字

**この関数は特別な関数で、配列のボディーでのみ使えます。また配列のボディーのどこで定義してもいいです**

## 例
```json
{
  "array": [
    {
      "value": 1
    },
    {
      "value": 2
    }
  ]
}
```

jfol:
```
$array[$value$$separator[\n]]
```

result:
```
1
2
```
