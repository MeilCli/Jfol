# if

conditional value, use `$$if`.

json:

```json
{
  "name": "meil"
}
```

format:

```
Hello World$$if($name=="meil")[, MeilCli].
```

output:

```
Hello World, MeilCli.
```