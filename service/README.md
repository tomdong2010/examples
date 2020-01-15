# Service

This is an example of creating a micro service.

## Contents

- main.go - is the main definition of the service, handler and client
- proto - contains the protobuf definition of the API
```shell 
// $SRC_DIR: .proto 所在的源目录
// --cpp_out: 生成 c++ 代码
// $DST_DIR: 生成代码的目标目录
// xxx.proto: 要针对哪个 proto 文件生成接口代码

protoc -I=$SRC_DIR --cpp_out=$DST_DIR $SRC_DIR/xxx.proto
```

## Run the example

Run the service

```shell
go run main.go
```

Run the client

```shell
go run main.go --run_client
```

And that's all there is to it.
