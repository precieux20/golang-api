FROM golang:1.20.2

WORKDIR /usr/src/app

RUN go install github.com/cosmtrek/air@latest

COPY go.mod go.sum ./
RUN go mod download

COPY . .

RUN go mod tidy

CMD ["air", "-c", ".air.toml"]