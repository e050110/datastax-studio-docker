# datastax-studio-docker

DataStax Studio on a Docker Container.

## Start DataStax Studio

#### Basic

```
docker run -p 9091:9091 jeremievallee/datastax-studio-docker
```

#### With shared data volume

With this solution, if you stop your container and them start it again, you won't loose the data you created in DataStax Studio.

```
mkdir /localpath/to/studio-data
docker run -p 9091:9091 -v /localpath/to/studio-data:/var/lib/datastax-studio jeremievallee/datastax-studio-docker
```
