## Lesson 1 - Containers e Docker

# Create, delete container
```
docker container run  -d -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=mongoadmin -e MONGO_INITDB_ROOT_PASSWORD=secret mongo

docker container ls

docker container rm -f [CONTAINER ID]
```

# Troubleshooting

```
docker container inspect [CONTAINER ID]

docker container exec -it [CONTAINER ID] /bin/bash

docker container logs [CONTAINER ID]
```

# Create, delete image
```
docker image build -t felipe/ubuntu:v1 .

docker image ls

docker image history [IMAGE ID]
```