# Pool-based Ape Staking (V2) Intro & FAQs

## What is Bend Pool-based Ape Staking (V2)?

Bend Pool-based Ape Staking (V2) is a **pure staking** protocol with NO liquidation risk or bank run risk. It is designed to maximize users' rewards with minimal GAS costs. With V2, holders of BAYC, MAYC, BAKC, and ApeCoin can stake their assets and instantly begin earning and auto-compounding yield.

### Why Pool-based Ape Staking (V2)?

#### **No Liquidation Risk & No Bank Run Risk**

Bend Pool-based Ape Staking is a pure staking solution. Therefore, no liquidation risk and no bank run risk for stakers thereby safeguarding user assets. It allows users to withdraw their stakes at any time during the staking period, providing both asset flexibility and liquidity.

#### **0 GAS Auto-compounding**

Upon depositing assets into the pool, users can immediately start earning auto-compounding yields without incurring any additional GAS costs for reinvestments, ensuring maximum yields.

#### Proposing $BEND Incentives

The community is proposing $**BEND Incentives** for even Higher APY for users. Details[https://discord.com/channels/897709643948761148/1105834496122703892](https://discord.com/channels/897709643948761148/1105834496122703892)

### **BendApeStaking V2 vs. V1**

| Bend Ape Staking                | V2        | V1                                                 |
| ------------------------------- | --------- | -------------------------------------------------- |
| Model                           | Pool2Pool | Peer2Peer                                          |
| Time of yield earning           | Instantly | Waiting for co-stakers to pair                     |
| Flexibility                     | Anytime   | Anytime                                            |
| Users’ Cost of Auto-compounding | 0 GAS     | Need to claim rewards to the auto-compounding pool |

## FAQ

[Security of Staking V2](pool-based-ape-staking-v2-intro-and-faqs.md#security-of-staking-v2)

[Auto-pairing Service Fee](pool-based-ape-staking-v2-intro-and-faqs.md#auto-pairing-service-fee)

[Auto-compounding](pool-based-ape-staking-v2-intro-and-faqs.md#auto-compounding)

[Staking, Withdraw, and Claim](pool-based-ape-staking-v2-intro-and-faqs.md#staking-withdraw-and-claim)

[Share Ratio](pool-based-ape-staking-v2-intro-and-faqs.md#share-ratio)

[StakedNFT (stNFT)](pool-based-ape-staking-v2-intro-and-faqs.md#stakednft)

### Security of Staking V2

#### **Q: What makes BendDAO's Pool-based Ape Staking safe?**

A: BendDAO's Pool-based Ape Staking implements several safety measures.

* Architecture Design V2 is constructed independently from Lending, maintaining a unique coupling yet isolating their respective functionalities. This architecture design achieves risk isolation.
* Pure Staking Solution No liquidation risk and no bank run risk for stakers thereby safeguarding user assets.
* Third-party Audit All smart contracts are audited by Verilog Solution, Report:[https://www.verilog.solutions/audits/benddao\_ape\_staking\_v2/](https://www.verilog.solutions/audits/benddao\_ape\_staking\_v2/).
* Testcase Coverage Whole code coverage is beyond 90%, all the core logic is covered by test cases, Repo:[https://github.com/BendDAO/bend-apestaking-v2](https://github.com/BendDAO/bend-apestaking-v2).

#### **Q: Is there a scenario for a flash loan attack?**

A: NO. V2 is a pure staking solution. With NO liquidation or bank run risks, it assures investments are safeguarded.

### Auto-pairing Service Fee

#### **Q: How does BendApeStaking V2 charge the pairing service fee?**

A: The pairing service fee is charged at the time of staking rewards claim, and calculated based on time since the previous claim. All the service fees are used to cover the expenditure of staking v2, eg. Security Audit, Auto Compounding Gas Cost.

#### **Q: Any chance to change the pairing service fee?**

A: Yes. The current charge is 4%. BendDAO is a DAO owned by the community. Anyone can propose a related proposal to adjust the setting.

#### **Q: If I deposit both ApeCoin and NFT, any Service Fee?**

A: For users who have both NFT and enough ApeCoin, they can use solo staking which does not charge any service fee, but without the zero gas auto compounding feature.

### Auto-compounding

#### **Q: What is auto-compounding?**

A: Auto-compounding is a feature that automatically reinvests earned ApeCoin into the official ApeCoin pool, which leads to compounding returns.

#### **Q: Do I need to pay GAS for the auto-compounding?**

A: It’s zero Gas for users. All cost is covered by the DAO.

#### **Q: What’s the frequency of the auto-compounding?**

A: It depends on the amount of the pending rewards of each NFT. The general principle is that the charged service fee from the pending rewards can cover the auto compound gas cost.

### Staking, Withdraw, and Claim

#### **Q: Can I withdraw my staked assets at any time?**

A: Yes, it offers complete asset flexibility, allowing users to withdraw their stakes at any point during the staking period.

#### **Q: If I stake my rare NFT to the pool, will I receive the same NFT when I withdraw?**

A: YES! The user will receive the stNFT when depositing. Each stNFT represents the value of the initially deposited NFT and is issued 1:1 with the original NFT. When the original NFT is withdrawn, the corresponding stNFT is burned. [More details of stNFT](pool-based-ape-staking-v2-intro-and-faqs.md#stakednft)

#### **Q: What is the main difference between V1 and V2?**

A: Please refer to the docs.

#### **Q: How does auto-compounding work?**

A: Auto-compounding in V2 works by automatically reinvesting the staking rewards generated from the staking. These rewards are directly deposited into the official ApeCoin pool without any additional GAS transactions, maximizing user profits.

#### **Q: Can I withdraw my staked assets at any time?**

A: Yes, Pool-base Ape Staking offers complete asset flexibility, allowing users to withdraw their stakes at any point during the staking period.

#### **Q: Any liquidation risk on V2?**

A: NO. V2 is a pure staking solution. It’s a Pool2Pool-based auto-paring and staking protocol,

### Share Ratio

#### **Q: What’s the share ratio?**

A: The share ratio will be adjusted periodically according to market rates, ensuring all parties achieve the optimal APY in the market.

#### **Q: What’s the frequency of the ratio adjustment?**

A: This mainly depends on the supply and demand of both ApeCoin and NFT on the staking pool, maybe every two weeks or a month.

### StakedNFT

#### **Q: What is stNFT?**

A: stNFT stands for Staked Non-Fungible Token. It represents an NFT that has been staked in BendDAO's Pool-based Ape Staking (V2). Each stNFT represents the value of the initially deposited NFT and is issued 1:1 with the original NFT. When the original NFT is withdrawn, the corresponding stNFT is burned.

#### **Q: Why do we need stNFT?**

A: The new pool-based Ape Staking is designed to maximize users' rewards with minimal GAS costs. To achieve this goal, a design like stNFT is necessary for the architecture. As soon as assets are staked in the protocol, users start enjoying auto-compounding staking rewards. In addition, users can also achieve more utilities based on stNFT, such as lending, and trading.

#### **Q: Can I trade my stNFTs?**

A: Yes, stNFTs are approvable and transferable, they can be tradable on the NFT marketplace.

#### **Q: What happens to the stNFT when I unstake my NFT?**

A: When you unstake your NFT, the corresponding stNFT is instantly burned. This means it will be removed from the blockchain and no longer exist.

#### **Q: How is the value of stNFTs determined?**

A: The value of stNFTs is consistent with the value of the original NFTs that are staked. Therefore, the value can fluctuate based on the market value of the original NFTs.

#### **Q: Why can't two NFTs with the same ID circulate at the same time?**

A: This is to avoid potential misuse of the system. Each stNFT is tied to a specific staked NFT, ensuring the system maintains the integrity of the 1:1 ratio between staked NFTs and stNFTs.

#### **Q: What are the parameters for stNFTs?**

A: stNFT parameters are set in accordance with their corresponding NFTs. For example, stBAYC follows the parameters of BAYC, and stMAYC follows the parameters of MAYC.

#### **Q: How to use delegate.cash to delegate ownership to hotwallet?**

A: Go to the etherscan [stakedBAYC](https://etherscan.io/token/0x08f5f0126af89b4fd5499e942891d904a027624b#writeProxyContract), [stakedMAYC](https://etherscan.io/token/0xc1ed28e4b4d8e284a41e7474ca5522b010f3a64f#writeProxyContract), [stakedBAKC](https://etherscan.io/address/0xf6d3B8098967dd349d0477F01C16E8864a832ac2#writeProxyContract), and then select `setDelegateCash` method.&#x20;

* The first parameter is your hotwallet address
* The second is your NFT tokenID
* The third is `true`.
