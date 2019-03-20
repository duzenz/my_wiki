# Docker commands

##  List all containers (only IDs)

```bash
docker ps -aq
```

##  Stop all running containers

```bash
docker stop $(docker ps -aq)
```
## Remove all containers

```bash
docker rm $(docker ps -aq)
```

##  Remove all images

```bash
docker rmi $(docker images -q)
```

##  Remove images from registry

```bash
rm -r <root>/v2/repositories/${name}/_manifests/tags/${tag}/index/sha256/${hash}
rm -r <root>/v2/repositories/${name}/_manifests/revisions/sha256/${hash}
```

##  How to Update a Single Running docker-compose Container

```bash
docker-compose stop <service_name>
docker-compose kill <service_name>
docker-compose up -d --no-deps <service_name>
```

```bash
docker-compose up -d --no-deps --build <service_name> 
```

## **Configure logback log level via environment variables**

Declare a new variable inside your logback.xml file and provide a default value for logging level.

```xml
<variable name="SERVICE_LOG_LEVEL" value="${SERVICE_LOG_LEVEL:-DEBUG}" />
<logger name="com.duzenz" level="${SERVICE_LOG_LEVEL}"/>
```

Run docker container with environment variable

```-e SERVICE_LOG_LEVEL=INFO ```
