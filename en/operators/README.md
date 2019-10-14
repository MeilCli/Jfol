# Operator
Jfol has some operators.

Operator can be calculate on function argument, but otherwhere does not calculate.

## Operators
- `==`, `!=`
  - left and right type(must same): String, Boolean, Number or Null
  - return type: Boolean
- `+`
  - left and right type: Number
    - return type: Number
  - left and right type(not both Number): String, Boolean, Number or Null
    - return type: String
- `-`, `%`, `*`, `/`
  - left type: Number
  - right type: Number
  - return type: Number
- `&&`, `||`
  - left type: Boolean
  - right type: Boolean
  - return type: Boolean
- `<`, `<=`, `>`, `>=`
  - left type: Number
  - right type: Number
  - return type: Boolean

## Priority
1. `*`, `/`, `%`
1. `+`, `-`
1. `<`, `<=`, `>`, `>=`
1. `==`, `!=`
1. `&&`
1. `||`