FROM golang:latest

RUN go install github.com/air-verse/air@latest

WORKDIR /app

COPY /app /app

COPY /app/.air.toml /app/.air.toml

EXPOSE 8080

CMD ["air", "-c", ".air.toml"]
