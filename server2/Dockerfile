FROM golang

ENV GO111MODULE=on

WORKDIR /app

COPY . .

RUN  go build ./cmd/api

ENTRYPOINT ["/app/api"]
