# Build docker image
```sh
docker build -t helloworld_node .
```

# Run docker container
```sh
docker run -v ./app:/app -w /app -it -p 3000:3000 --name helloworld_node_container helloworld_node
```

# Enter docker container
```sh
docker exec -it helloworld_node_container bash  # starts with bash
docker exec -it helloworld_node_container sh  # starts with sh
```