FROM golang:1.15

WORKDIR /go/src/microsservicos

COPY . .

RUN GOOS=linux go build

EXPOSE 9092

ENTRYPOINT [ "./microsservicos" ]