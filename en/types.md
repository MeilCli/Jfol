# Types
Jfol has 6 types in internal.

## Object
Object is basic type in Jfol.

Object is alike reference type in some programming language, and usually use pass to function argument or passed from function-return.

## Array
Array is alike array of reference types in some programming language, same as Object, and usually use pass to function argument or passed from function-return.

## String
String is base type in Jfol.

Most usually use in Jfol, Jfol-result can be said String.

## Boolean
Boolean is base type in Jfol.

Boolean value are only true or false, usually use in pass to function argument.

## Number
Number is base type in Jfol.

Number value are integer or floating point number, but Numerical range is implementation-dependent. So need to remenber that cannot calculate accurately.

## Null
Null value is only null. Null means nothing, need to remember what is different from undefined in JavaScript.

## Union
Some type maybe union type.

In example, value of String or Number type can pass to function String argument and function Number argument. If pass to value and passed from value both are union type, resolve by priority higher type.