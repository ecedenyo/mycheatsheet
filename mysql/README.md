## Content: MySQL
Once logged in mysql with credentials:

Command | Description
--- | --- 
`select * from <table> limit 3 \G` | List results in *(kinda)* vertical grid mode *(not table, the default one)*
`show columns from <table> like '%person%';` | Show columns that match the given criteria (i.e. partial column name includes 'person')
`show columns from <table> where type = 'varchar';` | Show columns that match the given criteria (i.e. columns of type 'varchar')
`select column_name from information_schema.columns where table_schema = '<db_name>' and table_name = '<table_name>' and is_nullable = 'no';` | Show all **not null** columns from the given table _(and yes!, such a long sentence for that!)_
