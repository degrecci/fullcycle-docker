FROM golang:1.21-alpine as build

WORKDIR /app

COPY main.go .
RUN go build -o hello ./main.go

FROM scratch

WORKDIR /

COPY --from=build /app/hello /app/hello

CMD ["/app/hello"]