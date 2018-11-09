# HOWTO build docker image 

## Build
```
docker build --rm -f "postgres-Dockerfile" -t blockchain-explorer-db .

docker build --rm -f "Dockerfile" -t blockchain-explorer .
```
## Tag
```
docker tag blockchain-explorer-db dahoba/blockchain-explorer-db
docker tag blockchain-explorer-db dahoba/blockchain-explorer-db:<versoin>

docker tag blockchain-explorer dahoba/blockchain-explorer
docker tag blockchain-explorer dahoba/blockchain-explorer:<versoin>
```
## Push
```
docker push dahoba/blockchain-explorer-db

docker push dahoba/blockchain-explorer
```

## Verify if image had push

go to  `https://cloud.docker.com/repository/docker/dahoba/blockchain-explorer` and  `https://cloud.docker.com/repository/docker/dahoba/blockchain-explorer-db`