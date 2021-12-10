FROM golang:1.17 as builder
WORKDIR /go/src
COPY main.go .
RUN go build -o server main.go

FROM scratch
COPY --from=builder /go/src/server .
CMD ["./server"]