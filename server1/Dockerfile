FROM golang

ENV GO111MODULE=on

WORKDIR /app

COPY . .

RUN go build ./cmd/api
RUN go build ./cmd/migrate


ENTRYPOINT ["/app/start.sh"]
