# length

can get length of array as function in array function or body.

json:

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

format:

```
Total: $$(array.length)\n$array[number $$number/$$length: $value$$separator[\n]]
```

output:

```
Total: 2
number 1/2: 1
number 2/2: 2
```