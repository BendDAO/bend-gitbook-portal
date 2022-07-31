# 安全和审计

## 审计

BendDAO 协议的实施以安全为首要考虑。该系统的设计是安全的，我们已经花费了所有必要的资源以确保该协议符合最高的安全标准。

以下是 BendDAO 的所有审计报告的链接。

| 审计方             | 日期       | 报告                                                                                   |
| ----------------- | ---------- | ------------------------------------------------------------------------------------ |
| Verilog Solutions | 2022-05-26 | [https://www.verilog.solutions/audits/benddao/](https://www.verilog.solutions/audits/benddao/) |
| Certik            | 2022-04-01 | [https://www.certik.com/projects/bend-dao](https://www.certik.com/projects/bend-dao)   |

{% hint style="info" %}
关于 Certik 报告中未解决的主要问题（Unresolved Major issues）：

1. 对于中心化的风险，BendDAO 已经部署了 **Timelock Controller**（时间锁控制器）和 **Multi-Signature Wallet**（多签钱包），请[在此](security-and-audits.md#timelock-controller)阅读细节。
2. 对于 NFT 预言机，BendDAO 采取了各种解决方案，如节点备份、时间加权和阈值检查，请[在此](../lending-protocol/oracle-price-feeding.md)阅读细节。
{% endhint %}

## 时间锁控制器（Timelock Controller）

BendDAO 已将所有 bend 借贷协议合约的所有者设置为 24 小时时间锁控制器地址。

BendDAO 已将 bound NFT 协议合约的所有者设置为 7 天时间锁控制器地址。

![](<../.gitbook/assets/Bend MultiSig Wallet & TimeLock 0526.png>)

| 名称              | 时长 | 地址                                                                                                               |
| ----------------- | -------- | --------------------------------------------------------------------------------------------------------------------- |
| BendDAO 时间锁  | 24 小时 | [0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214](https://etherscan.io/address/0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214) |
| BoundNFT 时间锁 | 7 天   | [0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e](https://etherscan.io/address/0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e) |

## 多签钱包（Multi-signature Wallet）

BendDAO 在合约升级和金库基金中使用了多个 Gnosis Safe 多签名钱包。

BenDAO 将在多签选举后将多签钱包转让给社区。

| 钱包名称             | 钱包类型 | 地址                                                                                                               |
| ----------------------- | ----------- | --------------------------------------------------------------------------------------------------------------------- |
| 初始代币分配 | Gnosis Safe | [0x16729FaD4DfD9F7c50f3b52a5deaF842D2c609B7](https://etherscan.io/address/0x16729FaD4DfD9F7c50f3b52a5deaF842D2c609B7) |
| 储备金库        | Gnosis Safe | [0x472FcC65Fab565f75B1e0E861864A86FE5bcEd7B](https://etherscan.io/address/0x472FcC65Fab565f75B1e0E861864A86FE5bcEd7B) |
| 时间锁提案者 1     | Gnosis Safe | [0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C](https://etherscan.io/address/0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C) |
| 时间锁提案者 2     | Gnosis Safe | [0xF1465c7Ea04765853Facc2D1ea68bc6e47bE90e1](https://etherscan.io/address/0xF1465c7Ea04765853Facc2D1ea68bc6e47bE90e1) |
| 时间锁管理员       | Gnosis Safe | [0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C](https://etherscan.io/address/0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C) |
