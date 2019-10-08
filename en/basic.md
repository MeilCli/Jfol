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
If write raw caracter, must escape it by `\`.

Escapable characters:
- `$`
- `(`
- `)`
- `[`
- `]`
- `\`
- `"`