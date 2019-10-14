# index
- 構文:
  - `$$index`
- 型:
  - NumberまたはString
- 説明:
  - 現在のindexを返します

**この関数は特別な関数で、配列のボディーでのみ使えます**

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
$array[index $$index value: $value$$separator[\n]]
```

return:
```
index 0 value: 1
index 1 value: 2
```