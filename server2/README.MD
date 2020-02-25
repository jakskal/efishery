# Endoint documantation

you can see the Endoint documentation in [Endoint documentation](https://server21.docs.apiary.io/#) or file Endpoint_documentation.MD

# manual instalation

## Requirement
please make sure you already have:

* Golang installed

*  golang wire

    ```go get github.com/google/wire/cmd/wire```

    and ensuring that $GOPATH/bin is added to your $PATH.

## Setup environtment variable 
you can see the example from .env.example


## Run Application 
```go run cmd/api/main.go cmd/api/wire_gen.go```


# Run using docker

## Requirement
*  docker
see [docker documentation](https://docs.docker.com/) 

## Build application
```cd to/app/directory```

```docker build it server2 .```

## Run application
```docker run -it --rm -p 8081:8081 --env-file ./.env --name server2 server2```