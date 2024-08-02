FROM golang:1.18-alpine

# ARG hanya bisa dibaca padaa saat dockerfile dibuild
ARG app="main"

RUN mkdir app
COPY main.go app
RUN mv app/main.go app/${app}.go
EXPOSE 8080

# sedangkan jika env dia bisa dibaca pada saat image dijalankan
ENV app=${app}
CMD go run app/${app}.go

