wonjinsin/go-grpc-boilerplate(phantom)
============================
Simple rest api server with [GO-GRPC](https://github.com/grpc/grpc-go)

[![License MIT](https://img.shields.io/badge/License-MIT-green.svg)](http://opensource.org/licenses/MIT)
[![DB Version](https://img.shields.io/badge/DB-Redis-red)](https://redis.io/)
[![DB Version](https://img.shields.io/badge/DB-Mysql-blue)](https://www.mysql.com/)
[![Go Report Card](https://goreportcard.com/badge/github.com/StarpTech/go-web)](https://goreportcard.com/report/github.com/wonjinsin/go-web-boilerplate)

## Features
- [Gorm](https://github.com/go-gorm/gorm) : For mysql ORM
- [Go-redis](https://github.com/go-redis/redis/v8) : Go redis client
- [Zap](https://github.com/uber-go/zap) : Go leveled Logging
- [Viper](https://github.com/spf13/viper) : Config Setting
- [Ginko](https://onsi.github.io/ginkgo) : BDD Testing Framework with [Gomega](https://onsi.github.io/gomega)
- [Makefile]() : go build, test, vendor using Make

## Project structure
DDD(Domain Driven Design) pattern with grpc-controller, model, service, repository

## dependency
```
$ go install google.golang.org/protobuf/cmd/protoc-gen-go
$ go install github.com/favadi/protoc-go-inject-tag@latest
```

## Getting started

### Initial action
```
$ make all && make build && make start
```

### Build vendors
```
$ make vendor
```

### Build and start
```
$ make build && bin/phantom
```

### Test
```
$ make vet && make lint && make test
// or
$ make test-all
```

### Clean
```
$ make clean
```

### reference
- [Go-clean-arch-grpc](https://github.com/bxcodec/go-clean-arch-grpc)
- [hexArchGoGRPC](https://github.com/selikapro/hexArchGoGRPC)