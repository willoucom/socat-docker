# socat-docker

Basic usage of socat for DooD (Docker out of Docker)

## Usage

Run container

```docker run -d -v /var/run/docker.sock -p 2375:2375 --name=socat_docker willoucom/socat-docker```

Link another container

```docker run -l socat_docker:socat myimage```
