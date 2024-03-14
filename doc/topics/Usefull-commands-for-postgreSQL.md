# Useful commands for PostgreSQL

## Create a database dump

<tabs>
<tab title="whole db">

~~~shell
pg_dump dbName -U userName > dumpFileName.sql
~~~

</tab>
<tab title="certain table">

~~~shell
pg_dump dbName -U dbUser -t tableName > dumpFileName.sql
~~~

</tab>
<tab title="in docker container">

~~~shell
docker exec containerName bash -c "pg_dump dbName -U dbUser -t tableName > dumpFileName.sql"
~~~

</tab>
</tabs>

## Restore database from dump
<tabs>
<tab title="whole db or table">
Works same for db or table - just runs sql-script

~~~shell
psql dbName -U dbUser < dumpFile.sql
~~~
</tab>
<tab title="in docker container">

~~~shell
docker exec london_back-pgsql-1 bash -c "psql dbName -U dbUser < dumpFile.sql"
~~~
</tab>
</tabs>