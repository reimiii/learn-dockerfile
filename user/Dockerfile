FROM golang:1.18-alpine

RUN mkdir /app

RUN addgroup -S imigroup
RUN adduser -S -D -h /app imiuser imigroup
RUN chown -R imiuser:imigroup /app

USER imiuser

COPY main.go /app

EXPOSE 8080

CMD [ "go", "run", "/app/main.go" ]
