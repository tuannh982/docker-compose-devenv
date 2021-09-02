The first time we run 

```sh
docker-compose up -d
```

to bootstrap elasticsearch and kibana containers,

`AccessDeniedException[/usr/share/elasticsearch/data/nodes]` will be thrown in the elasticsearch container

Simply run 

```sh
./fix-access-denied-exception.sh /path/to/elasticsearch/persistent/dir
```