# 清算和赎回

Bend 协议利用“健康系数”评分进行贷款。该公式概述如下。

当 NFT 贷款的“健康系数”低于 1 时，任何人都可以以 [**NFT拍卖**](auction.md) 的方式触发清算。清算人在 Bend 上被称为 Bidder（出价人）。出价人将偿还所有的债务，并获得抵押的 NFT 作为回报。

![](<../.gitbook/assets/image (3).png>)

请阅读[ 拍卖](auction.md) 中的清算细节。

## 健康系数的含义

健康系数的定义：(地板价 \* 清算阈值) / 含息债务。

健康系数（HF）的风险水平：

* 0.0 < HF < 1.0: <mark style="color:red;background-color:red;">危险</mark>，如果不及时偿还债务，借款人可能会失去抵押品。
* 1.0 <= HF <= 1.5: <mark style="color:orange;background-color:red;">有风险</mark>，借款人应及时偿还部分债务。
* 1.5 < HF < 2.0: <mark style="color:yellow;background-color:yellow;">请注意</mark>，借款人应注意并及时监控债务情况。
* 2.0 <= HF: <mark style="color:green;background-color:green;">安全</mark>，借款人不需要担心，可以保持债务。

如果 NFT 贷款的健康系数低于 1，将会触发清算。

## NFT 贷款状态

![](<../.gitbook/assets/NFT Loan State 0320.jpg>)
