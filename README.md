以太坊中继 (ETH-Relay)
书籍《区块链以太坊DApp开发实战》跟学源码

## 启动
`eth-relay/block_scanner_test.go` 的 `TestBlockScanner_Start` 函数是区块遍历入口函数

## 功能列表
- 创建以太坊钱包
- 解锁以太坊钱包，传入钱包地址和对应的 keystore密码
- 签名交易数据结构体
- 构建符合“ERC20”标准的“transfer”合约函数的“data”入参
- 根据交易的 hash 值获取对应交易的信息
- 根据交易 hash 字符串数组批量获取对应的交易信息
- 单条查询：根据以太坊地址，查询以太坊 eth 的余额
- 单条查询：根据以太坊地址，查询以太坊 ERC20 代币的余额
- 批量查询：根据以太坊地址数组，查询以太坊 eth 的余额
- 批量查询：根据以太坊地址数组，查询 ERC20 代币的余额
- 发送交易，根据入参 transaction 的不同变量设置，达到发送不同种类的交易
- 获取地址的 nonce 值
- 直接发送 ERC20 代币交易，或称转账 ERC20 代币
- 获取以太坊最新生成区块的区块号
- 根据区块号，获取区块信息
- 根据区块 hash，获取区块信息
- 自定义扫描以太坊区块