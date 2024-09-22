# Step 1: build golang binary
FROM golang:1.17 as builder
WORKDIR /opt/app
COPY tcp-server.go .
RUN go build -o tcp-server tcp-server.go

# Step 2: copy binary from step1
FROM ubuntu:latest
WORKDIR /opt/app
COPY --from=builder /opt/app/tcp-server ./tcp-server
EXPOSE 3333
ENTRYPOINT ["./tcp-server"]
