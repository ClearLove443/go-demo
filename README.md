# go demo

## 环境

```sh
go env -w GO111MODULE=on
go env -w GOPROXY=https://mirrors.aliyun.com/goproxy/,direct

# vscode
"go.goroot": "D:/Program Files/go",
"gopls": {
  "ui.semanticTokens": true
}
go mod init demo
```

## 正向代理 (类似vpn)

[正向代理 vs 反向代理](https://cloud.tencent.com/developer/article/1418457)

### 测试

```sh
curl --proxy 127.0.0.1:18080 http://www.baidu.com
curl --proxy 127.0.0.1:18080 https://www.baidu.com
```
