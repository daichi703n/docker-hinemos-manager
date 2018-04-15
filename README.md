# Docker Hinemos

http://www.hinemos.info/

Hinemos docker image.

### Prerequirement
- Docker
- Docker Compose

## How to use

```
git clone https://github.com/daichi703n/docker-hinemos
docker run -d --privileged --name hinemos-manager -p 8080:8080 -p 8081:8081 -p 161:161/udp -p 162:162/udp -p 514:514 -p 10080:80 daichi703n/hinemos-manager /sbin/init
```

Or deploy with docker-compose.

```
docker-compose up
```

access to `http://<DockerHost IP>:10080`

Default User ID / Password is **hinemos / hinemos**.  
Manager URL `http://localhost:8080/HinemosWS/`
