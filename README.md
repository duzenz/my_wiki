# Docker commands

# List all containers (only IDs)

```docker
docker ps -aq
```

# Stop all running containers
```docker
docker stop $(docker ps -aq)
```
# Remove all containers

```docker
docker rm $(docker ps -aq)
```

# Remove all images

```docker
docker rmi $(docker images -q)
```


## **Configure logback log level via environment variables**

Declare a new variable inside your logback.xml file and provide a default value for logging level.

```xml
<variable name="SERVICE_LOG_LEVEL" value="${SERVICE_LOG_LEVEL:-DEBUG}" />
<logger name="com.duzenz" level="${SERVICE_LOG_LEVEL}"/>
```

Run docker container with environment variable

```-e SERVICE_LOG_LEVEL=INFO ```
