## Content: MySQL
Once logged in mysql with credentials:
Command | Description
--- | --- 
`select * from <table> limit 3 \G` | List results in *(kinda)* vertical grid mode *(not table, the default one)*
`show columns from <table> like '%person%';` | Show columns that match the given criteria (i.e. partial column name includes 'person')
`show columns from <table> where type = 'varchar';` | Show columns that match the given criteria (i.e. columns of type 'varchar')
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjcxNzIxMjQzXX0=
-->