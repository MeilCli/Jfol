# Context
Function and field execute on current context, and, function body and field body execute on child context. 

```json
{
    "value": "hello",
    "child": {
        "value": "world"
    }
}
```
In example, `$value` is String of "hello" and `$child` is Object. `$child[/*here*/]`'s *here* is child context, so `$child[$value]`'s `$value` is String of "world"

**Not necessarily, all function body executes on child context.** some function's body executes on current context or parent context, need to remember see function document.