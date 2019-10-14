# value
- 構文:
  - `$$value`
- 型:
  - Stringの値の場合: String
  - Numberの値の場合: NumberまたはString
  - Booleanの値の場合: BooleanまたはString
  - Nullの値の場合: NullまたはString
- 説明:
  - 現在のコンテキストの値を取得する

## 例
```json
{
  "array": [1, 2, 3]
}
```

jfol:
```
$array[$$value$$separator[\n]]
```

result:
```
1
2
3
```