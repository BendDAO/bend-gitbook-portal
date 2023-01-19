# Flash Claim FAQ

[Sewer Pass](flash-claim-faq.md#sewer-pass)

[General](flash-claim-faq.md#general)

## Sewer Pass

First, figure out which kind of situation you are in before Flash Claim.

1. Borrow and Stake (including solo staking)
2. Only Borrow
3. Only Stake

| BAYC/MAYC Holder | Flash Claim Start Time                                      | Remark                                                            |
| ---------------- | ----------------------------------------------------------- | ----------------------------------------------------------------- |
| Borrow and Stake | 7:30pm PST; 11:30am HKT, 20th Jan (because of the timelock) | If the user unstake, he/she can Flash Claim the pass on 17th Jan. |
| Only Borrow      | 17th Jan (same as the official site)                        |                                                                   |
| Only Stake       | 17th Jan (same as the official site)                        |                                                                   |

Users who only borrow or stake can Flash Claim directly via BendDAO to mint the Sewer Pass on 17th Jan.

Users who borrow and stake at the same time can Flash Claim directly via BendDAO to mint the Sewer Pass on 20th Jan. If the user unstake, he can Flash Claim the pass on 17th Jan as well.

{% hint style="info" %}
All details will be further confirmed when the official Sewer Pass Mint contract is released.&#x20;
{% endhint %}

### **Q: Why is the Flash Claim start time for users who both borrow and join the staking be 20th Jan, not 17th Jan?**

A: Because there is a 7-day timelock of Lending Pool contract. The new version of the Flash Claim Registry that supports users to Flash Claim when both borrowing and staking are deployed on 13th Jan and will be effective on 20th Jan. [Security ](../risk/security-and-audits.md)

### **Q: My BAYC and/or MAYC is deposited, can I plus a BAKC to mint a higher-tiered Sewer Pass?**

A: Yes. You can combine with a BAKC for a higher-tiered Sewer Pass with Flash Claim. The BAKC should be in your wallet address.

### **Q: Can I unstake right before the mint to Flash Claim at the first time, if I’m borrowing and staking?**

A: Yes, you can unstake anytime.

### **Q: Any preparation I need to do for Flash Claim?**

A: First-time users can deploy the **Airdrop Receiver Contract first** which is a one-time cost.&#x20;

[Refer to Q: Can I Flash Claim if I have no knowledge of programming? ](flash-claim-faq.md#q-can-i-flash-claim-if-i-have-no-knowledge-of-programming)



| BAKC Holder | Flash Claim | Remark                                        |
| ----------- | ----------- | --------------------------------------------- |
| Only Stake  | N.A.        | Users need to unstake first to join the mint. |

### **Q: I join the Ape Staking with my BAKC on BendDAO. How to Flash Claim with my BAKC?**

A: BAKC holders need to unstake first to mint a higher-tiered Sewer Pass.

## General

### Q: How can I claim my airdrops when my NFT is deposited in Bend?&#x20;

A: Flash Claim feature is designed for this scenario. Find the “Flash Claim” on the Dashboard, and borrowers can claim related airdrops. [https://www.benddao.xyz/app/flash-claim](https://www.benddao.xyz/app/flash-claim)

### Q: How can BendDAO know whether I’m eligible for the airdrop?&#x20;

A: Airdrops can be claimed if you’re holding related boundNFTs. All borrowers receive boundNFTs when they successfully deposit NFTs in Bend.

&#x20;[boundnft.md](../lending-protocol/boundnft.md "mention")

### Q: What kind of airdrop will be supported?&#x20;

A: Flash Claim supports 2 kinds of airdrops. 1) The project airdrops to holders’ addresses directly including contract addresses; 2) The airdrops need to be claimed by holders (no restriction of contract addresses). More details: [https://docs.benddao.xyz/portal/user-guides/flashclaim](https://docs.benddao.xyz/portal/user-guides/flashclaim)

### Q: If the project airdrops to holders’ addresses directly, how can BendDAO know which airdropped token belongs to which borrower?&#x20;

A: BendDAO follows the airdrop rules set by the project. Both specific and random airdrops can be supported.

### Q: If it’s a random airdrop, how does BendDAO distribute airdrops?&#x20;

A: The distribution process on BendDAO is also random. For fairness and safety, BendDAO random algorithm is based on [Chainlink VRF infrastructure](https://vrf.chain.link/mainnet) to distribute tokens.&#x20;

The VRF subscription id is on Chainlink: [81](https://vrf.chain.link/mainnet/81).

The code for airdrop distribution is on[ ](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol)Github: [AirdropDistribution.sol](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol).&#x20;

The contract address on[ ](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD)Etherscan: [0x6D187449A5664DD87E58A9d3b982989AaeA469BD](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD).

### Q: What if I miss the claim period?&#x20;

A: You can always Flash Claim airdrops on BendDAO if the project airdrops to holders’ addresses directly including contract addresses. Your airdrop never expires.

If the airdrops need to be claimed by holders (no restriction of contract addresses), the expiration date is decided by the project instead of BendDAO.

### Q: Can I Flash Claim if I have no knowledge of programming?&#x20;

A: Yes, you can. There are no programming requirements.&#x20;

You need to click the "Deploy Airdrop Receiver Contract" for the first Flash Claim. It's needed only once.&#x20;

![](<../.gitbook/assets/image (4) (2).png>)

### Q: What is boundNFT?&#x20;

A: For NFT-backed loans, when the borrower deposits an NFT in BendDAO, a boundNFT will be minted as a Debt NFT. For Custody, when the NFT holder deposits an NFT in BendDAO, a boundNFT will be minted as a receipt NFT.&#x20;

More details of boundNFT https://docs.benddao.xyz/portal/highlights/true-ownership

### Q: Is the Flash Claim open-sourced?&#x20;

A: Yes. Visit BoundNFT Github to find more details. https://github.com/BoundNFT/boundnft-protocol/tree/main/contracts

### Q: Can I realize the Flash Claim by myself if I have programming experience?&#x20;

A: Yes. Users also can write a contract to implement the Flash Claim. Please check the demo on Github. https://github.com/BendDAO/bend-flashclaim-demo

### Q: What kind of airdrops will be supported on BendDAO?&#x20;

A: Technically, all airdrops that are related to the collaterals can be supported. BendDAO-supported collaterals are BAYC, CryptoPunks, MAYC, Azuki, Moonbirds, CloneX, and Doodles.

Feel free to find the team in Discord if you want us to support other airdrops.
