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
cd api
go run api/server/server.go
```

### インストール
[evans](https://github.com/ktr0731/evans)
```bash
brew tap ktr0731/evans
brew install evans
```

### リクエストサンプル
```bash
echo '{ "menu": 1}' | evans -r -p 50051 cli call pancake.maker.PancakeBakerService.Report
```

### protocol buffersの生成
```bash
make proto.build
```
