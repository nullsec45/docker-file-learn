FROM golang:1.18-alpine

RUN mkdir /app

RUN addgroup -S fajar_group
RUN adduser -S -D -h /app fajar fajar_group
RUN chown -R fajar:fajar_group /app

USER fajar
COPY main.go /app

EXPOSE 8080
CMD go run /app/main.go
