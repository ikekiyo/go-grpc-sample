# go-grpc-sample
golang × gRPC のサンプル

## 開発
### version管理
asdfで管理
```
# plugin install
asdf plugin-add golang

# python install
asdf install golang 1.18.0

# local setup
asdf local golang 1.18.0
```

### 起動
```bash
go run api/server/server.go
```
### リクエストサンプル
```bash
grpc_cli call localhost:50051 pancake.maker.PancakeBakerService.Bake 'menu: 2'
```

### protocol buffersの生成
```bash
make proto.build
```
