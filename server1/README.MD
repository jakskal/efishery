# Endpoint documantation
you can see the Endpoint documentation in [Endpoint documentation](https://anglingz.docs.apiary.io/#reference/0/authentication) or file API_documentation.MD 

# Manual instalation

## Requirement
please make sure you already have:

* Golang installed

*  golang wire

    ```go get github.com/google/wire/cmd/wire```

    and ensuring that $GOPATH/bin is added to your $PATH.

*  docker
see [docker documentation](https://docs.docker.com/) 

* postgres database

## Run Containerized Postgres if have no postgres installed
docker run --name postgres -p 5432:5432 -d postgres

inspect the postgres container ip addres and set it to DB_HOST in .env file

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

```docker build it server1 .```

## Run application

⋅⋅⋅ note: make sure set your .env properly

```docker run -it --rm -p 8080:8080 --env-file ./.env --name server1 server1```