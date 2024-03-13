# Usefull commands for postgreSQL

## Create a database dump

<tabs>
<tab title="whole db">

~~~shell
pg_dump dbName -U userName > dumpFileName.sql
~~~
</tab>
<tab title="certain table">

~~~shell
pg_dump dbName -U userName -t tableName > dumpFileName.sql
~~~
</tab>
</tabs>
