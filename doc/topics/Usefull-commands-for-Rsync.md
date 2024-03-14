# Usefull commands for Rsync


### Copy file from remote server

~~~shell
rsync -chavzP -e 'ssh -p 2722' userName@remoteHostName:remotePath -avP targetPath
~~~