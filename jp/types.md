# 様々な型
Jfolは内部的に6つの型があります

## Object
ObjectはJfolの基礎的な型です

Objectは様々なプログラミング言語の参照型のようなもので、関数の引数や返り値によく使われます

## Array
Arrayは様々なプログラミング言語の参照型の配列のようなもので、Objectと同じように関数の引数や返り値によく使われます

## String
StringはJfolの基本型です

Jfolで最もよく使われ、Jfolの結果はStringとも言えます

## Boolean
BooleanはJfolの基本型です

Booleanの値はtrueまたはfalseしかなく、関数の引数でよく使われます

## Number
NumberはJfolの基本型です

Numberの値は整数値または小数点の数値です。しかし数値の範囲は実装依存となります。そのため正確な計算ができないということを覚えておく必要があります

## Null
Nullの値はnullしかありません。Nullは何もないことを意味していますが、JavaScriptのundefinedとは違うことを覚えておく必要があります

## 共用体
いくつかの型は共用体型になります

たとえば、StringまたはNumberの値は関数のString引数と関数のNumber引数に渡すことができます。もし、渡す型と受け取る型が両方共用体であれば優先度の高い型で解決されます