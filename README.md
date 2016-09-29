# socat-docker
[![](https://images.microbadger.com/badges/image/willoucom/socat-docker.svg)](https://microbadger.com/images/willoucom/socat-docker "Get your own image badge on microbadger.com")

Basic usage of socat for DooD (Docker out of Docker)

## Usage

Run container

```docker run -d -v /var/run/docker.sock -p 2375:2375 --name=socat_docker willoucom/socat-docker```

Link another container

```docker run -l socat_docker:socat myimage```

