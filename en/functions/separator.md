# separator

simple foreach cannot set separator, so use `$$separator` function.

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
$array[$value$$separator[\n]]
```

output:

```
1
2
```

`$$separator` can define anywhere array field body.

that is, `$array[$value$$separator[\n]]` equals to `$array[$$separator[\n]$value]`.
