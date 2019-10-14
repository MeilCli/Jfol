# where
- 構文: 
  - `$$where(condition)`
    - 1つ目の引数:
      - 型: Boolean
      - 説明: 配列のボディーを実行する条件
- 型:
  - Boolean
- 説明:
  - 配列ボディーのwhereコントロール

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
$array[value: $value$$where($value==1)]
```

result:
```
value: 1
```