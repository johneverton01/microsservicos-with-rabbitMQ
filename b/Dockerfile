FROM golang:1.15

WORKDIR /go/src/microsservicos

COPY . .

RUN go get github.com/joho/godotenv
RUN go get github.com/satori/go.uuid
RUN go get github.com/streadway/amqp
RUN go get github.com/wesleywillians/go-rabbitmq/queue

RUN GOOS=linux go build

ENTRYPOINT [ "./microsservicos" ]