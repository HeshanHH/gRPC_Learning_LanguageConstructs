This is a learning project.
There are some comments that can be a note. but this may be incorrect. 😁 
use gRPC documentation and check with it if something feels incorrect.

gRPC uses an special file written in protocol buffers
the .proto file sits between the consumer and the gRPC API ( Server )
gPRPC use HTTP2

What is gRPC?

 High-performance remote procedure call (RPC) framework
 Uses binary serialization
 Designed for HTTP/2
 Contract-first

 Can define and expose APIs in a language-agnostic way
 Perfect for Service - to - Service communication

 Can provide sync and async communication


What is gRPC?

 It uses an special file written in Protocol Buffers

 The .proto file sits between the consumer and the gRPC API(server)

Service A -proto file Service B


Feature						grpc								RESTful API
		
Contract					Required (.proto)					Optional
		
Protocol					HTTP/2								HTTP/2 & 1
		
Payload						Protobuf (small, binary)			JSON (large)
		
Strong-Typing				yes									No
		
Streaming					Client, server, bi-directional		Client, server
		
Client code-generation		yes									OpenAPI + third-part
		
Security					Transport (TLS)						Transport (TLS)


