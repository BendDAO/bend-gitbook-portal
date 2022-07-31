# 预言机价格推送

Bend 协议使用来自 [OpenSea](http://opensea.io) 和 [LooksRare](https://looksrare.org/) 的 NFT 地板价作为 NFT 抵押品的价格推送数据。Bend 协议只支持蓝筹 NFT 资产的地板价，用于链上价格推送。蓝筹 NFT 的地板价不容易被操纵。此外，Bend 协议计算地板价的 TWAP（时间加权均价），以过滤来自 [OpenSea](http://opensea.io) 和 [LooksRare](https://looksrare.org/) 交易市场的价格波动。

Bend 的预言机设计和运行机制：

1. 链下节点从 OpenSea 和 Looksrare 交易市场获得 NFT 的原始地板价；
2. 过滤原始地板价数据，如 Opensea 和 Lookrare 之间的地板价差异太大；
3. 根据 Opensea 和 Looksrare 的交易量计算出地板价；
4. 比较链上价格和最新地板价之间的差异，以决定是否需要将地板价上传到链上；
5. 调用合约接口，将地板价上传至链上合约，并计算链上时间加权平均价格（TWAP）以对地板价进行加权，确保价格合理；
6. twap 的算法在链上合约上是开源的，每个人都可以验证数据的有效性；

{% hint style="info" %}
对于 CryptoPunks，我们从 [CryptoPunksMarket](https://etherscan.io/address/0xb47e3cd837ddf8e4c57f05d70ab865de6e193bbb#code) 合约直接获得地板价！
{% endhint %}

![预言机机制](<../.gitbook/assets/Bend NFT Oracle 0517.png>)

为了保证安全性和可靠性，我们将运行多个节点以确保有效的价格数据能够随时及时上传到链上预言机合约，并且链上合约限制了价格推送的频率，两个价格推送的差异不能超过一个阈值。

Bend 的开发人员正在与 Chainlink 团队合作，完成 NFT 预言机的价格推送。

## 预言机价格曲线

### CryptoPunks 6 个月内的价格曲线

如图所示，CryptoPunks 的预言机地板价与平均交易价格和 TWAP 价格一致。

![](<../.gitbook/assets/CryptoPunks Price Curve 0401.png>)

### Bored Ape YC 6 个月内的价格曲线

如图所示，BAYC 的预言机地板价与平均交易价格和 TWAP 价格一致。

![](<../.gitbook/assets/BAYC Price Curve 0401.png>)
