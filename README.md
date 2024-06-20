Install protoc on Windows: https://www.geeksforgeeks.org/how-to-install-protocol-buffers-on-windows/
test
Linux:
```
protoc --plugin=./node_modules/.bin/protoc-gen-ts_proto --ts_proto_out=./ --ts_proto_opt=nestJs=true ./proto/auth.proto
```

Windows
```
protoc --plugin=protoc-gen-ts_proto=".\\node_modules\\.bin\\protoc-gen-ts_proto.cmd" --ts_proto_out=. --ts_proto_opt=nestJs=true ./proto/*.proto
protoc --plugin=protoc-gen-ts_proto=".\\node_modules\\.bin\\protoc-gen-ts_proto.cmd" --ts_proto_out=".\proto\test" --ts_proto_opt=nestJs=true ./proto/*.proto
```

ts-proto: https://github.com/stephenh/ts-proto
