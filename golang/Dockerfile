FROM golang:alpine AS builder 
WORKDIR /usr/src/myapp
COPY ./hello.go .
RUN go build hello.go 

FROM scratch
WORKDIR /usr/src/myapp
COPY --from=builder /usr/src/myapp .
CMD ["./hello"]