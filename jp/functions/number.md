# number
- 構文:
  - `$$number`
- 型:
  - NumberまたはString
- 説明:
  - 現在のindex+1を返す

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
$array[number $$number value: $value$$separator[\n]]
```

result:
```
number 1 value: 1
number 2 value: 2
```