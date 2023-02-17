# golang-microservice-course
Code for Working with Microservices in Go course

run:
```
$ cd project
$ make up_build
```

Mongo DB connection string:
```
mongodb://admin:password@localhost:27017/logs?authSource=admin&readPreference=primary&appname=MongoDB%20Compass&directConnection=true&ssl=false
```

Install proto via: https://grpc.io/docs/languages/go/quickstart/

Compile Proto
```
$ cd ./logger-service/logs
$ protoc --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative logs.proto
```