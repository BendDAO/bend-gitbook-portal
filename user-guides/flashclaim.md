# 闪电领取（Flash Claim）

闪电领取是建立在 BoundNFT 的闪电贷（Flash Loan）之上。通过闪电领取，您可以使用您的 NFT 来领取第三方的空投，而不需要偿还给贷款池。

对于知名空投项目，Bend 将正式进行适配。用户不需要开发合约代码和了解基础的技术细节。他们只需要在网页上选择空投项目和自己的 NFT 就可以快速完成领取。

对于那些没有得到官方支持的空投项目，如果您认为它是好项目，请在 Discord 社区反馈。如果有足够的人力和时间，Bend 会尽量优先支持。

Bend 支持两类空投项目，第一类是用户主动发起交易领取空投，第二类是项目方主动空投给用户。

对于第一种类型，Bend 使用 boundNFT 的闪电贷来支持用户领取空投，空投闪电贷的代码在[Github](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropFlashLoanReceiver.sol)，以及合约地址在 [Etherscan](https://etherscan.io/address/0xa8Ae91Dd8CD8f410BA59626caef160925A033734)。

![](<../.gitbook/assets/Flash claim 04191810.jpg>)

对于第二种类型，Bend 将做快照和空投分发，以支持用户领取空投。如果空投项目方使用一些随机算法来分发代币，为了公平和安全，我们也使用基于 [Chainlink VRF infrastructure](https://vrf.chain.link/mainnet) 的随机算法来分发代币。

[Chainlink VRF 订阅 ID](https://vrf.chain.link/mainnet/81) 是  81，空投分发的代码在 [Github](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol)，以及合约地址在 [Etherscan](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD)。

![](<../.gitbook/assets/Airdrop Distribution 04191825.jpg>)

## 使用闪电领取 UI

第1步：进入面板，点击 Claim your airdrop（领取您的空投）。

第2步：选择空投项目并点击 Claim（领取）。

第3步：领取交易成功后，您将在钱包中获得空投代币。

![](<../.gitbook/assets/Flashclaim Page 04201331.jpg>)

![](<../.gitbook/assets/Dashboard Flashclaim 02401330.jpg>)

![](<../.gitbook/assets/Flashclaim Page 04201331.jpg>)

## 闪电领取代码 Demo

对于高级用户，您可以写一个合约来实现领取，请在 [Github](https://github.com/BendDAO/bend-flashclaim-demo) 中查看演示。
