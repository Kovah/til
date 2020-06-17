# Restore a MySQL database from a gzipped dump

```
gunzip < dump.sql.gz | mysql -u [uname] -p[pass] [dbname]
```
