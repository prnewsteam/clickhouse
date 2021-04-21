### Create the image

```
docker build -t prnewsio/clickhouse:latest --force-rm --no-cache .
docker login -u="\$DOCKER_USERNAME" -p="\$DOCKER_PASSWORD"
docker push prnewsio/clickhouse:latest
```

### Run with docker-compose

```
...
    image: prnewsio/clickhouse:latest
...      
```