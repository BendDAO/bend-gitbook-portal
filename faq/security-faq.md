# 安全 FAQ

## Q: BendDAO 如何保持安全？&#x20;

A: BendDAO 团队已经花费了所有必要的资源，以确保该协议符合最高的安全标准。



* 提供的第二份审计报告。[https://www.verilog.solutions/audits/BendDAO](https://www.verilog.solutions/audits/BendDAO)
* 在 BendDAO 主网上线前，Certik 发布了一份 BendDAO 的审计报告。[https://www.certik.com/projects/bend-dao ](https://www.certik.com/projects/bend-dao)
* 高达 $1m 的 BendDAO 漏洞（Bug）赏金 [https://immunefi.com/bounty/benddao/](https://immunefi.com/bounty/benddao/)&#x20;
* 所有 boundNFT 协议合约都有 7 天的时间锁。
* 所有 BendDAO 借贷协议合约都有 24 小时的时间锁。

https://docs.benddao.xyz/portal/risk/security-and-audits

## Q: 时间锁如何保护用户？&#x20;

A: 时间锁被用来增加关键操作的延迟，如合约升级和代币转移，使用户能够在协议操作真正生效之前知道这些操作并采取行动。这种时间延迟使用户有机会在团队变得恶意或受攻击时退出协议。

* 所有 boundNFT 协议合约——7 天时间锁&#x20;
* 所有 BendDAO 借贷协议合约——24 小时时间锁&#x20;

更多时间锁的细节，见：[https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller](https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller)

## Q: 用户如何监控时间锁？&#x20;

A: 用户可以使用 Etherscan 设置提醒。一旦合约地址上的任何合约更改得到确认，包括资金交易和协议升级，就会发送电子邮件。以下是关于如何设置电子邮件通知的指南：[https://info.etherscan.com/watch-list/](https://info.etherscan.com/watch-list/)

所有 boundNFT 协议合约——7 天时间锁：[https://etherscan.io/address/0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e ](https://etherscan.io/address/0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e)

所有 BendDAO 借贷协议合约——24 小时时间锁：[https://etherscan.io/address/0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214](https://etherscan.io/address/0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214)&#x20;

## Q: 为什么 BendDAO 使用可升级的代理合约（upgradeable proxy contracts）？&#x20;

A: 我们为 BendDAO 合约使用可升级代理的原因是为了确保资金的安全。如果发现一些漏洞，团队可以用可升级的代理来改进功能。

为了避免信任问题，所有合约都有时间锁。时间锁是一种智能合约的功能，它规定只有在一定时间后才会进行升级，而不是立即进行。在升级真正生效之前，所有用户都有一个时间窗口来采取行动。

* 所有 boundNFT 协议合约——7 天时间锁&#x20;
* 所有 BendDAO 借贷协议合约——24 小时时间锁&#x20;

更多时间锁的细节，见：[https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller](https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller)

## Q: 我担心团队跑路（rug pull）看，要是 BendDAO 跑路怎么办？&#x20;

A: 在加密货币中的跑路是指团队突然放弃一个项目，并出售或从去中心化交易平台（Dex）中移除其所有流动资金。

DAO 成员而非团队在 Uniswap 上提供所有 BEND/ETH 的流动性。第一个团队代币的释放将在 2023 年 5 月 9 日 14:29 UTC 发生。团队现在没有任何 BEND 代币。

团队代币合约细节：[https://mirror.xyz/benddaoteam.eth/VLTqI6yPC\_YojeUreU1YvJfHT27KFEkHFW5BN1CH48M](https://mirror.xyz/benddaoteam.eth/VLTqI6yPC\_YojeUreU1YvJfHT27KFEkHFW5BN1CH48M)

## Q: 如果 BendDAO 团队将所有蓝筹 NFT 和 ETH 从借贷池中拿走怎么办？&#x20;

A: 从技术上讲，只有借款人/贷款人的地址可以调用提款功能。更多 BendDAO 协议的细节：https://github.com/BendDAO

## Q: 如果 BendDAO 团队将他们的地址列入白名单，将所有蓝筹 NFT 和 ETH 从借贷池中撤出怎么办？&#x20;

A: 从技术上讲，团队无法做到这一点。但是即使该团队能够做到，由于时间锁的存在，实施起来也会有延迟。时间锁使用户能够在协议升级真正生效之前知道更新并采取行动。这种时间延迟使用户有机会撤出所有资产，并在团队变得恶意或受攻击时退出协议。

更多 BendDAO 协议的细节：[https://github.com/BendDAO ](https://github.com/BendDAO)

更多时间锁的细节：[https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller](https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller)

## Q: BendDAO 智能合约是否有保险？&#x20;

A: 无。因为保险对可扩展协议（scalable protocol）不起作用。而且以前没有保险真正覆盖了 DeFi 漏洞的损失。安全操作和审计是减少安全漏洞风险的关键，而不是保险。
