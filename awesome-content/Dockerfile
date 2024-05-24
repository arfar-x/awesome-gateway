FROM golang:1.18-alpine
LABEL authors="Alireza"

WORKDIR /app

COPY . .

RUN go mod download

RUN go build -o /app/main_app main.go

RUN chmod +x /app/main_app

CMD ["./main_app"]
