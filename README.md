# memo-docker
A few useful commands for Docker

### Build container from Dockerfile
`docker build -t {desired_container_name} {path_to_dockerfile}`

### List available containers
`docker ps`

### Stop and delete all containers
```
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```

### Local dev
`docker run -p 80:80 -t -i -v /local/path:/container/path {container_name} /bin/bash`
