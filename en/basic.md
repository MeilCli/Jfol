# Basic
Jfol interpret some character to symbol.
- `$`
- `$$`
- `(`, `)`
- `[`, `]`
- `.`
- `\`

## Syntax
### Literal
Jfol has 4 literal type.
- String Literal
  - alike some programming language, enclosed by `""`
- Number Literal
  - alike some programming language number, but Numerical range is implementation-dependent
- Boolean Literal
  - `true` or `false`
- Null Literal
  - `null`

### Field
$(*identifiers*)[*fieldBodies*]  
$*identifier*[*fieldBodies*]

- identifiers are to connect with `.`
  - example:
  - $(*identifier1*.*identifier2*)[*fieldBodies*]
- fieldBodies can omit
  - example:
  - $(*identifiers*)
  - $*identifier*

### Function
$$(*identifiers.functionName*)(*functionArguments*)[*functionBodies*]  
$$*functionName*(*functionArguments*)[*functionBodies*]

- identifiers are to connect with `.`
- functionArguments are to separate by `,` and can omit
  - example:
  - $$*functionName*(*functionArgument1*,*functionArgument2*)[*functionBodies*]
  - $$*functionName*[*functionBodies*]
- functionBodies can omit
  - example:
  - $$*functionName*(*functionArguments*)

## Escape
If write raw character, must escape it by `\`.

Escapable characters:
- `$`
- `(`
- `)`
- `[`
- `]`
- `\`
- `"`

## Escape Sequence
If use special character, you can use escaping sequence.

- `\0`: Null
- `\b`: Backslash
- `\f`: Form feed
- `\n`: New line
- `\r`: Carriage return
- `\t`: Horizontal tab
- `\v`: Vertical tab