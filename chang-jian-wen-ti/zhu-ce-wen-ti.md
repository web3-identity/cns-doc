# 注册问题

### .web3用户名使用什么公链注册？

.web3用户名仅支持使用ConfluxCore地址进行注册。访问（网址），连接Fluent或支持的钱包，按流程指引进行注册。

### 注册过程中如何防止名称被抢注？

当一个用户注册.web3用户名，注册内容的交易在内存池中等待被打包进区块时，其他人可以看到用户要注册的内容，并立即发出一笔网络手续费更高的交易企图让矿工优先打包进行抢注，一旦抢注成功，真正想拥有这个用户名的用户将付出高价进行回购。因此，.web3合约会要求注册新的用户名时，必须经过两个阶段的注册模式，防止抢注行为发生。

1.注册申请：将用户的注册内容Hash、随机秘密值、公钥组合计算Hash，生成注册申请，提交到控制器。用户执行申请的过程，就是将注册申请记录到区块链的过程。在执行第1步后，需要等待一小段时间。

2.注册请求：用户真正的发起注册请求，携带上一步组合计算的Hash，执行注册验证。验证有效，用户进行支付并完成注册。

注册申请包含注册内容的hash和随机秘密值，不会泄露原始信息，即便恶意抢注者在用户执行第2步看到了明文的注册内容，也需要执行第一步并等待间隔时间才能完成注册，因此有效防止恶意抢注者通过观察区块链获取用户注册内容进行恶意抢注。

如果你执行第1步后，最后想注册的注册内容还是被注册了，这只能是冥冥中的巧合了。

### 注册费用如何支付？

.web3用户名的注册和续费支持法币支付，发起的注册时的网络手续费由Conflux基金会代付支持。

### .web3用户名为什么不能一次性购买永久使用？

.web3用户名是运行在区块链上分布式、去中心化的命名系统。拥有.web3用户名意味着你拥有这个账户完整的使用权和控制权，但如果私钥丢失，将导致.web3用户名永久性锁死。

.web3用户名是以.web3为后缀的全局唯一的命名系统，存在有限的优质名称资源。因此.web3用户名会在用户不进行续费后释放到公共资源中，提供给其他人使用资源的机会。

同时，作为公链的基础设施，.web3命名系统需要的持续改进和推广，开发者需要正向驱动的维护动力。

实际上，为了实现“永久使用”，你可以为.web3用户名续费数十年。

### 注册失败支付的费用会退还吗？

会退还。退还方式和退回时间取决于你所使用的注册商。

### 用户名过期会怎么样？

用户名过期后，会进入90天保护期。保护期内可以进行续费。

### 保留名称是什么？如何获取？

被判定用户名归属于某个组织或个人的，将会对名称进行保留。保留的用户名只能被其对应的组织和个人进行认领，认领方式即将开放。

### .web3用户名都有什么注册商？如何成为注册商？

官方注册渠道（网址），除此之外，目前接入智能合约的注册商还包括美匣和双镜，请访问：。不同的注册商提供的用户界面或法币支付方式会有所不同。任何人都可以和智能合约进行交互，任何人都可以成为注册商。成为注册商请访问：
