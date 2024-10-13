FROM golang:1.23.2-alpine as base

WORKDIR /app

COPY go.mod .
COPY go.sum .

RUN go mod download

COPY . .

RUN go build -o app .

FROM alpine:latest as prod

WORKDIR /app
USER 1000

COPY --chown=1000:1000 --from=base /app/app .

CMD ["./app"]

EXPOSE 8080
