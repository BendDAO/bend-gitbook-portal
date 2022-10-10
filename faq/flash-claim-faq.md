# Flash Claim FAQ

## Q: How can I claim my airdrops when my NFT is deposited in Bend?&#x20;

A: Flash Claim feature is designed for this scenario. Find the “Flash Claim” on the Dashboard, and borrowers can claim related airdrops. [https://www.benddao.xyz/app/flash-claim](https://www.benddao.xyz/app/flash-claim)

## Q: How can BendDAO know whether I’m eligible for the airdrop?&#x20;

A: Airdrops can be claimed if you’re holding related boundNFTs. All borrowers receive boundNFTs when they successfully deposit NFTs in Bend.

&#x20;[boundnft.md](../lending-protocol/boundnft.md "mention")

## Q: What kind of airdrop will be supported?&#x20;

A: Flash Claim supports 2 kinds of airdrops. 1) The project airdrops to holders’ addresses directly including contract addresses; 2) The airdrops need to be claimed by holders (no restriction of contract addresses). More details: [https://docs.benddao.xyz/portal/user-guides/flashclaim](https://docs.benddao.xyz/portal/user-guides/flashclaim)

## Q: If the project airdrops to holders’ addresses directly, how can BendDAO know which airdropped token belongs to which borrower?&#x20;

A: BendDAO follows the airdrop rules set by the project. Both specific and random airdrops can be supported.

## Q: If it’s a random airdrop, how does BendDAO distribute airdrops?&#x20;

A: The distribution process on BendDAO is also random. For fairness and safety, BendDAO random algorithm is based on [Chainlink VRF infrastructure](https://vrf.chain.link/mainnet) to distribute tokens.&#x20;

The VRF subscription id is on Chainlink: [81](https://vrf.chain.link/mainnet/81).

The code for airdrop distribution is on[ ](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol)Github: [AirdropDistribution.sol](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol).&#x20;

The contract address on[ ](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD)Etherscan: [0x6D187449A5664DD87E58A9d3b982989AaeA469BD](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD).

## Q: What if I miss the claim period?&#x20;

A: You can always Flash Claim airdrops on BendDAO if the project airdrops to holders’ addresses directly including contract addresses. Your airdrop never expires.

If the airdrops need to be claimed by holders (no restriction of contract addresses), the expiration date is decided by the project instead of BendDAO.

## Q: Can I Flash Claim if I have no knowledge of programming?&#x20;

A: Yes, you can. There are no programming requirements.&#x20;

You need to click the "Deploy Airdrop Receiver Contract" for the first Flash Claim. It's needed only once.&#x20;

![](<../.gitbook/assets/image (4).png>)

## Q: What is boundNFT?&#x20;

A: For NFT-backed loans, when the borrower deposits an NFT in Bend DAO, a boundNFT will be minted as a Debt NFT. For Custody, when the NFT holder deposits an NFT in Bend DAO, a boundNFT will be minted as a receipt NFT.&#x20;

More details of boundNFT https://docs.benddao.xyz/portal/highlights/true-ownership

## Q: Is the Flash Claim open-sourced?&#x20;

A: Yes. Visit BoundNFT Github to find more details. https://github.com/BoundNFT/boundnft-protocol/tree/main/contracts

## Q: Can I realize the Flash Claim by myself if I have programming experience?&#x20;

A: Yes. Users also can write a contract to implement the Flash Claim. Please check the demo on Github. https://github.com/BendDAO/bend-flashclaim-demo

## Q: What kind of airdrops will be supported on BendDAO?&#x20;

A: Technically, all airdrops that are related to the collaterals can be supported. BendDAO-supported collaterals are BAYC, CryptoPunks, MAYC, Azuki, CloneX, and Doodles.

Feel free to find the team in Discord if you want us to support other great airdrops.
