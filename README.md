# Docker Hinemos

http://www.hinemos.info/

Hinemos docker image.

### Prerequirement
- Docker
- Docker Compose (Option)

## How to use

### docker run

```
docker run -d --privileged --name hinemos-manager -p 8080:8080 -p 8081:8081 -p 161:161/udp -p 162:162/udp -p 514:514 -p 10080:80 daichi703n/hinemos-manager /sbin/init
```

### docker-compose up

Or deploy with docker-compose.

```
git clone https://github.com/daichi703n/docker-hinemos
docker-compose up
```

## Access to Hinemos manager
Access to `http://<DockerHost IP>:10080`

Default User ID / Password is **hinemos / hinemos**.  
Manager URL `http://localhost:8080/HinemosWS/`

Let's start monitoring!!
