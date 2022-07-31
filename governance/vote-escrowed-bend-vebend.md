# BEND 托管选票（veBEND）

用户需要质押他们的 [BEND](https://etherscan.io/token/0x0d02755a5700414b26ff040e1de35d337df56218) 代币以获得 [veBEND](https://etherscan.io/address/0xd7e97172C2419566839Bf80DeeA46D22B1B2E06E) 代币来赚取协议收入或在 Bend DAO 上投票。

BEND 持有者可以参与投票，决定 Bend 协议可以支持哪些 NFT 作为抵押品以借出 ETH 并提供流动性。只要支持的 NFT 的流动性得到改善，所有 NFT 持有者都会受益。

社区投票选出 7 个蓝筹 NFT 中的 4 个：
[https://snapshot.org/#/benddao.eth/proposal/QmVgsdtx6PAqKLyAMSnvXAoLrEJc1s6VVKLtWtEdqb4zPC](https://snapshot.org/#/benddao.eth/proposal/QmVgsdtx6PAqKLyAMSnvXAoLrEJc1s6VVKLtWtEdqb4zPC)

参与 BEND DAO 治理需要一个账户有 BEND 托管选票（veBEND）的余额。veBEND 是一种非标准的 ERC20 协议（non-standard ERC20 implementation），在 Snapshot 中用来确定每个账户的投票权。

veBEND 由 VotingEscrow 合约代表，部署在 Ethereum 主网上的：待确认。

veBEND 不能被转移。获得 veBEND 的唯一方法是锁定 BEND。最大的锁定时间为四年。一个锁定四年的 BEND 可以提供一个 veBEND 的初始余额。

一个用户的 veBEND 余额会随着 BEND 解锁前剩余时间的减少而线性衰减。例如，锁定一年的 4000 BEND 的余额提供的 veBEND 数量与锁定两年的 2000 BEND 或锁定四年的 1000 BEND 相同。

最高锁定期为四年时间。公式概述如下：

MAXTIME = 4 \* 365 \* 86400\
unlock\_time < (block\_time + MAXTIME) veBEND\_amount = BEND\_locked\_amount / MAXTIME \* (unlock\_time - block\_time)
