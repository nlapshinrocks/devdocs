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
