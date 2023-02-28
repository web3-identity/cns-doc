# 必须要知道关于正向解析和反向解析

### 什么是正向解析？

正向解析是指，通过一个 .web3 用户名可以查询到一个区块链地址

比如说，通过 `A.web3` 查询到 `cfx:abc...abcd` 这个区块链地址

具体的场景是，在 Fluent Wallet 中，输入 A.web3 即可向 `cfx:abc...abcd` 转账

**一个地址可以有多个正向解析**

可以将多个用户名的正向解析都设置为 `cfx:abc...abcd` 这个地址

比如说， `A.web3` , `B.web3` , `C.web3` 这三个用户名的正向解析都设置成 `cfx:abc...abcd`

那么通过以上任意一个用户名，都可以查询到 `cfx:abc...abcd` 这个地址



### 什么是反向解析

反向解析是指，通过一个区块链地址查询到其用于展示的用户名

比如说：通过 `cfx:abc...abcd` 查询到 `A.web3` 这个用户名



**一个地址只能有一个反向解析**

接着前文的描述，如果 `A.web3` , `B.web3` , `C.web3` 这三个用户名的正向解析都设置成了 `cfx:abc...abcd`&#x20;

那么，可以选择 `A.web3` , `B.web3` , `C.web3` 的其中一个作为展示域名