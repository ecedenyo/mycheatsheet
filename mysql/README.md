## Content: MySQL
Once logged in mysql with credentials:

Command | Description
--- | --- 
`select * from <table> limit 3 \G` | List results in *(kinda)* vertical grid mode *(not table, the default one)*
`show columns from <table> like '%person%';` | Show columns that match the given criteria (i.e. partial column name includes 'person')
`show columns from <table> where type = 'varchar';` | Show columns that match the given criteria (i.e. columns of type 'varchar')
`select column_name from information_schema.columns where table_schema = '<db_name>' and table_name = '<table_name>' and is_nullable = 'no';` | Show all **not null** columns from the given table _(and yes!, such a long sentence for that!)_
`show tables where tables_in_<databasename> not like '<condition>';` | Show only tables that match the given condition based on tables name
`show full tables where table_type = 'base table';` | Show only table objects from database (not views, etc).
`show full tables where table_type != 'view';` | Show only table objects from database (not views).
`select name from mysql.proc where db = database() and type = 'procedure';`| Show only stored procedures from database, replace 'procedure' for 'function' accordingly ...
`SELECT DISTINCT TABLE_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE COLUMN_NAME IN ('columnA','ColumnB') AND TABLE_SCHEMA='YourDatabase';` | Get all tables within a specify database with given columns.
`SELECT * INTO OUTFILE '/tmp/data.csv' FIELDS TERMINATED BY ',' OPTIONALLY ENCLOSED BY '"' LINES TERMINATED BY '\n' FROM <table>` | Export the results of a given query to a file.

### Other combo-commands:

**Import** _(some)_ sql to the selected database keeping the **encoding**.
```
mysql -uroot -p --default-character-set=utf8 database
mysql> SET names 'utf8';
mysql> SOURCE utf8.dump
```

**Exporting** including SP.
```mysqldump <other mysqldump options> --routines outputfile.sql```
