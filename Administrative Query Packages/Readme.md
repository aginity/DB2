# DB2 Package Summary

|Package Name| Package Description| Number of Queries in Package|
|------------|--------------------|-----------------------------|
|Aginity-Pro-DB2-Admin-Set1.aginitypkg|Contains administrative queries to do common tasks in DB2   | 10  |


### The table below details all queries within the Aginity-Pro-DB2-Admin-Set1 package.


|Catalog Item Name               |Catalog Item Description            | Required Table     |
|--------------------------|------------------------------------|--------------------|
|Active Queries|This query allows you to see active queries running|sysibmadm.mon_current_sql|
|BLU Compression Ratios|Calculates the compression ratio for BLU tables|SYSCAT.TABLES|
|Column Selectivity by Table (BLU)|Reports how selective at the column level queries are that run against a specific table|EXECUTE privilege on the routine, DATAACCESS authority, DBADM authority, SQLADM authority|
|Columns of a Table in a Comma Separated List|Lists the columns of a table in a comma separated list|syscat.columns|
|Dependent MQTs and Views for a Table in a Schema|Lists all MQTs and views dependent on a single table, MQT, or view.|syscat.tabdep|
|List of users in current database with few of their authorities|Returns users list with permissions|sysibmadm.authorizationids, syscat.dbauth|
|Listing Tables and Current Size|Returns a list of tables and their current sizes in descending order by size.|syscat.tables, sysibmadm.admintabinfo|
|top 20 queries by Number of Executions|SQL for top 20 SQL by Number of Executions|SYSIBMADM.TOP_DYNAMIC_SQL|
|top 20 SQL by Execution Time|SQL for top 20 SQL by Execution Time|SYSIBMADM.TOP_DYNAMIC_SQL|
|Unused Indexes|Generate a list of unused or not recently used indexes.|syscat.indexes, syscat.tables, syscat.references, syscat.keycoluse|
