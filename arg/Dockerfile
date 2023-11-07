FROM golang:1.18-alpine

ARG app=main

RUN mkdir app

COPY . app

RUN mv app/main.go app/${app}.go

EXPOSE 8080

ENV app=${app}

CMD go run app/${app}.go
