# Hello Docker

## Login on Docker Hub
```bash
  docker login docker.io
```

## Build docker image
> Before build docker image, is needed build maven package to generate `.jar` file;
```bash
    mvn clean package
```

```bash
    docker build -t hello-docker:0.0.1-SNAPSHOT .
```

## Create `tag` compatible with Docker Hub
```bash
  docker tag hello-docker:0.0.1-SNAPSHOT douglasmatosdev/hello-docker:0.0.1-SNAPSHOT
```

## Push image to Docker Hub
```bash
    docker push douglasmatosdev/hello-docker:0.0.1-SNAPSHOT
```



