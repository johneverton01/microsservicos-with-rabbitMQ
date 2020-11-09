FROM golang:1.15

WORKDIR /go/src/microsservicos

COPY . .

RUN go get github.com/joho/godotenv
RUN go get github.com/wesleywillians/go-rabbitmq/queue

RUN GOOS=linux go build

EXPOSE 9090

ENTRYPOINT [ "./microsservicos" ]