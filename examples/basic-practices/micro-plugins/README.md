# micro plugins

## 跨域

实现跨域，只需要在 micro api（micro API 网关）注册相关插件，并且通过命令行指定跨域相关信息即可。

```go
plugin.Register(cors.NewPlugin())
```

```bash
go run main.go api 
--cors-allowed-headers=X-Custom-Header,X-Header 
--cors-allowed-origins=someotherdomain.com,xx.com 
--cors-allowed-methods=POST
```
