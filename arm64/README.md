### Create the image

```
docker buildx build --platform linux/arm64 -t prnewsio/clickhouse:latest.arm --force-rm --no-cache .
docker login -u="\$DOCKER_USERNAME" -p="\$DOCKER_PASSWORD"
docker push prnewsio/clickhouse:latest.arm
```