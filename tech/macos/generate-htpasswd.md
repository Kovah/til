# Generate htpasswd credentials on macOS

You can easily generate the user-password combination for a htpasswd file on macOS using the `htpasswd -nb [user] [password]` command, whih is actually built-in.

```
$ htpasswd -nb user password
user:$apr1$6w/uVSDH$0KU12480Tv421ZMwtFK5K1
```
