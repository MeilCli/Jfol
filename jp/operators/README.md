# 演算子
Jfolは様々な演算子を持っています  

演算子は関数の引数でのみ計算され、他の場所では計算されません

## 演算子の一覧
- `==`, `!=`
  - 左辺と右辺の型(両方同じ必要あり): String, Boolean, NumberまたはNull
  - 戻る型: Boolean
- `+`
  - 左辺と右辺の型: Number
    - 戻る型: Number
  - 左辺と右辺の型(両辺ともNumberではない): String, Boolean, NumberまたはNull
    - 戻る型: String
- `-`, `%`, `*`, `/`
  - 左辺の型: Number
  - 右辺の型: Number
  - 戻る型: Number
- `&&`, `||`
  - 左辺の型: Boolean
  - 右辺の型: Boolean
  - 戻る型: Boolean
- `<`, `<=`, `>`, `>=`
  - 左辺の型: Number
  - 右辺の型: Number
  - 戻る型: Boolean

## 優先度
1. `*`, `/`, `%`
1. `+`, `-`
1. `<`, `<=`, `>`, `>=`
1. `==`, `!=`
1. `&&`
1. `||`