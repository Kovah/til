# Show the content of a shell alias

To easily show what a shell alias might do, use `type`:

```
type [alias]
```

Example output for aliases:

```
$ type gcmsg
gcmsg is an alias for git commit -m

$ type gloga
gloga is an alias for git log --oneline --decorate --graph --all
```

Example output for regular command:

```
$ type genact
genact is /usr/local/bin/genact
```

