indexify
========

Create an sqlite3 database out of your csv / dsv files for quick querying. Assumes headers in the CSV

Usage
-----

```sh
$ indexify my-cool-database.db table_name /path/to/csv-file.csv index1 index2
$ SEPARATOR=" " indexify my-cool-database.db another_table_name /path/to/ssv-file.ssv
$ sqlite3 my-cool-database.db
sqlite> select * from table_name left outer join another_table name on column1 = another_table.another_column
```
