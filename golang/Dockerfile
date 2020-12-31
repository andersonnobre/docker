FROM golang:1.14 AS StageOne 

WORKDIR /usr/src/myapp
COPY ./hello.go .
RUN go build hello.go

FROM scratch
WORKDIR /usr/src/myapp
COPY --from=StageOne /usr/src/myapp .
CMD ["./hello"]