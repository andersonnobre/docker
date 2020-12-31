FROM golang:1.14 AS Builder 

WORKDIR /usr/src/myapp
COPY ./hello.go .
RUN go build hello.go

FROM scratch
WORKDIR /usr/src/myapp
COPY --from=Builder /usr/src/myapp .
CMD ["./hello"]