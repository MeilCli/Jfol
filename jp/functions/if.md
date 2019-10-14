# if
- 構文:
  - `$$if($value)[body]`
    - 1つ目の引数:
      - 型: Boolean
      - 説明: 条件値、もしtrueであればボディーを実行
    - ボディー:
      - 現在のコンテキスト
- 型:
  - String
- 説明: 
  - ifコントロール

## 例
```json
{
  "name": "meil"
}
```

jfol:
```
Hello World$$if($name=="meil")[, MeilCli].
```

result:
```
Hello World, MeilCli.
```