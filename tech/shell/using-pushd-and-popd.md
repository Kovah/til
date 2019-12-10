# Using pushd and popd for quick directory changes

[pushd and popd](https://en.wikipedia.org/wiki/Pushd_and_popd) can be used to quickly switch into a specific directory, execute commands and switch back to the previous directory.

## Example

```bash
$ pwd
/homes/kovah/work

$ pushd /tmp
/tmp ~/homes/kovah/work~

$ pwd
/tmp

$ popd
~/homes/kovah/work~

$ pwd
/homes/kovah/work
```
