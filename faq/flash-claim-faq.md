# 闪电领取（Flash Claim）FAQ

## Q: 当我的 NFT 存入 Bend 时，我如何能领取我的空投？&#x20;

A: 闪电领取功能就是为这种情况设计的。在网页面板上找到 “Flash Claim”，借款人即可领取相关空投。 [https://www.benddao.xyz/app/flash-claim](https://www.benddao.xyz/app/flash-claim)

## Q: Bend 如何知道我是否有资格获得空投？&#x20;

A: 如果您持有相关的 boundNFT，您可以领取空投。所有借款人在 Bend 成功存入 NFT 时都会收到 boundNFT。

&#x20;[boundnft.md](../lending-protocol/boundnft.md "mention")

## Q: 闪电领取将支持哪种空投方式？&#x20;

A: 闪电领取支持两种空投方式：1）项目直接空投到持有者地址，包括合约地址；2）空投需要持有人领取（无合约地址限制）。更多细节，见：[https://docs.benddao.xyz/portal/user-guides/flashclaim](https://docs.benddao.xyz/portal/user-guides/flashclaim)

## Q: 如果项目直接空投到持有人的地址，Bend 怎么能知道哪个空投的代币属于哪个借款人？&#x20;

A: Bend DAO 遵循项目设定的空投规则。可以支持指定空投和随机空投。

## Q: 如果是随机空投，Bend DAO 是如何分配空投的？&#x20;

A: Bend 上的分配过程也是随机的。为了公平和安全，Bend 的随机算法是基于 [Chainlink VRF 架构](https://vrf.chain.link/mainnet) 来分发代币。&#x20;

Chainlink 上的 VRF 的订阅 id：[81](https://vrf.chain.link/mainnet/81)。

空投代币分配的代码在[ ](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol)Github: [AirdropDistribution.sol](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol)。&#x20;

合约地址在[ ](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD)Etherscan: [0x6D187449A5664DD87E58A9d3b982989AaeA469BD](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD)。

## Q: 如果我错过了领取期怎么办？&#x20;

A: 如果项目直接空投到持有人地址，包括合约地址，您永远可以在 BendDAO 上面闪电领取您的空投。您的空投永不过期。

如果空投需要被持有者认领（无合约地址限制），到期日由项目而不是 BendDAO 决定。

## Q: 如果我没有编程知识，也可以使用闪电领取吗？&#x20;

A: 是的，您可以。闪电领取没有任何编程要求。&#x20;

您需要在第一次闪电领取时点击 "Deploy Airdrop Receiver Contract"（部署空投接收合约）。该操作只需要做一次。&#x20;

![](<../.gitbook/assets/image (4).png>)

## Q: 什么是 boundNFT?&#x20;

A: 对于 NFT 支持的贷款，当借款人在 Bend DAO 存入 NFT 时，一个 boundNFT 将被铸造成债务 NFT。对于托管，当 NFT 持有人在 Bend DAO 存入 NFT 时，一个 boundNFT 将被铸造一个 NFT 收据。&#x20;

更多 boundNFT 的细节，见：https://docs.benddao.xyz/portal/highlights/true-ownership

## Q: 闪电领取是开源的吗？&#x20;

A: 是的。详情见 BoundNFT Github：https://github.com/BoundNFT/boundnft-protocol/tree/main/contracts

## Q: 如果我有编程经验，我可以自己实现闪电领取吗？&#x20;

A: 是的。用户也可以自己写合约来实现闪电领取。见 Github 上的 demo：https://github.com/BendDAO/bend-flashclaim-demo

## Q: BendDAO 上面支持什么样的空投？&#x20;

A: 从技术上讲，所有与抵押品有关的空投都可以得到支持。BendDAO-支持的抵押品包括 BAYC、CryptoPunks、MAYC、Azuki、CloneX 以及 Doodles。

如果您希望团队支持其它更多很棒的空投，请随时通过 Discord 联系团队。
