# supergold-adapter

supergold-adapter继承了litecoin-adapter，主要修改了如下内容：

- 重写了Symbol = "SPG"。

## 如何测试

openwtester包下的测试用例已经集成了openwallet钱包体系，创建conf文件，新建SPG.ini文件，编辑如下内容：

```ini

# switch of scan block  true:scan false:disable
isScan = true
# RPC Server Type，0: CoreWallet RPC; 1: Explorer API
rpcServerType = 0
# node api url, if RPC Server Type = 0, use supergold core full node
serverAPI = "http://127.0.0.1:18445/"
# RPC Authentication Username
rpcUser = "user"
# RPC Authentication Password
rpcPassword = "password"
# Is network test?
isTestNet = false
# minimum transaction fees
minFees = "0.004"
# Cache data file directory, default = "", current directory: ./data
dataDir = ""

```

