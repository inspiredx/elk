# filebeat

```
docker cp es01:/usr/share/elasticsearch/config/certs/http_ca.crt ./
docker run --rm --name fb01 --net elk -p 8080:8080 -v $(pwd)/filebeat.yml:/usr/share/filebeat/filebeat.yml -v $(pwd)/http_ca.crt:/usr/share/filebeat/http_ca.crt elastic/filebeat:8.7.0
```
