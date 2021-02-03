# gRPC Calc Service
A simple gRPC calc service using Go.

## Compile
- Run,
```sh
protoc --proto_path=proto --proto_path=third_party --go_out=proto --go-grpc_out=proto service.proto
```

- To run server,
```sh
cd server
go run main.go
```


- To run client,
```sh
cd client
go run main.go
```

# Test
- Open browser/ or curl and navigate to test the Url
```sh
curl http://localhost:8080/add/152/120
{"result": "272"}
```
```sh
curl http://localhost:8080/mul/152/200
{"result": "30400"}
```

