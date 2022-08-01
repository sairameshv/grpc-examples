# grpc-examples
This repository revolves around some of the stuff/examples related to the gRPC protocol, proto buffers, proto files etc.

## References
* https://grpc.io/docs/what-is-grpc/introduction/
* https://grpc.io/docs/languages/go/quickstart/
* https://grpc.io/docs/languages/go/basics/
* https://developers.google.com/protocol-buffers/docs/reference/go-generated

## What is gRPC?
* In gRPC, a client application can directly call a method on a server application on a different machine as if it were a local object, making it easier for you to create distributed applications and services. As in many RPC systems, gRPC is based around the idea of defining a service, specifying the methods that can be called remotely with their parameters and return types. On the server side, the server implements this interface and runs a gRPC server to handle client calls. On the client side, the client has a stub (referred to as just a client in some languages) that provides the same methods as the server.
* gRPC clients and servers can run and talk to each other in a variety of environments - from servers inside Google to your own desktop - and can be written in any of gRPC’s supported languages. So, for example, you can easily create a gRPC server in Java with clients in Go, Python, or Ruby. In addition, the latest Google APIs will have gRPC versions of their interfaces, letting you easily build Google functionality into your applications.

## Hands-On
* [Install](https://go.dev/doc/install) `go` as a prerequisite.
* [Install](https://grpc.io/docs/protoc-installation/) Protocol Buffer compiler `protoc`
* Go plugins for the protocol compiler as follows
```go
go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2
```
