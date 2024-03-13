# Usefull commands for Docker

#Usefull commands for docker

## Copy files between container and host

<tabs>
<tab title="host 2 container">

~~~shell
docker cp containerName:/filePathInContainer FilePathOnHost
~~~
</tab>
<tab title="container 2 host">

~~~
docker cp FilePathOnHost containerName:/filePathInContainer
~~~
</tab>
</tabs>