#This is a learning project.
There are some comments that can be a note. but this may be incorrect. 😁 
use gRPC documentation and check with it if something feels incorrect.

gRPC uses an special file written in protocol buffers
the .proto file sits between the consumer and the gRPC API ( Server )
gPRPC use HTTP2

##What is gRPC?

 High-performance remote procedure call (RPC) framework
 Uses binary serialization
 Designed for HTTP/2
 Contract-first

 Can define and expose APIs in a language-agnostic way
 Perfect for Service - to - Service communication

 Can provide sync and async communication


##What is gRPC?

 It uses an special file written in Protocol Buffers

 The .proto file sits between the consumer and the gRPC API(server)

Service A -proto file Service B


| Feature				| grpc						|RESTful 
|--|--|--|
| Contract				| Required (.proto)	 		| Optional 
| Protocol	 			| HTTP/2					| HTTP/2 & 1 
| Payload	 			| Protobuf (small, binary) 	| JSON (large) 
| Strong-Typing 		| yes	 					| No 
|Streaming				|Client, server, bi-directional| Client, server
|Client code-generation	|yes						| OpenAPI + third-part
|Security				|Transport (TLS)			| Transport (TLS)
		


##When to use gRPC?

Microservices

Point-to-point real-time communication

Polyglot environments/wannabe

Mobile devices and networks with bandwidth restrictions

Inter-process communication (IPC)

Background jobs (Windows service, CRON, etc.)

To replace older technologies


##Introduction to Protocol Buffers

Language and platform-neutral data serialization format developed by Google.
Used for defining structure of our types and operations using a simple language
Strongly typed
Binary encoded
Backward and forward compatibility
Extensible
Multiple language Support


##Scalar Value Types
A scalar message field can have one of the following types – the table shows the type specified in the .proto file, and the corresponding type in the automatically generated class:

https://protobuf.dev/programming-guides/proto3/#scalar

double, float, int32, int64, uint32, uint64, sint32, sint64, fixed32, fixed64, sfixed32, sfixed64, bool, string, bytes