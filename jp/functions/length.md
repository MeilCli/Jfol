# length
- 構文:
  - `$$length`
- 型:
  - NumberまたはString
- 説明:
  - 配列の長さまたはlengthプロパティーを返す

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
Total: $$(array.length)\n$array[number $$number/$$length: $value$$separator[\n]]
```

result:
```
Total: 2
number 1/2: 1
number 2/2: 2
```