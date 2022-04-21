# Flash Claim FAQ

## Q: How can I claim my airdrops when my NFT is deposited in Bend?&#x20;

A: Flash Claim feature is designed for this scenario. Find the “Flash Claim” on the Dashboard, and borrowers can claim related airdrops. [https://www.benddao.xyz/app/flash-claim](https://www.benddao.xyz/app/flash-claim)

## Q: How can Bend know whether I’m eligible for the airdrop?&#x20;

A: Airdrops can be claimed if you’re holding related boundNFTs. All borrowers receive boundNFTs when they successfully deposit NFTs in Bend.

## Q: What kind of airdrop will be supported?&#x20;

A: Flash Claim supports 2 kinds of airdrops. 1) The project airdrops to holders’ addresses directly; 2) The airdrops need to be claimed by holders. More details: https://docs.benddao.xyz/portal/user-guides/flashclaim

## Q: If the project airdrops to holders’ addresses directly, how can Bend know which airdropped token belongs to which borrower?&#x20;

A: Bend DAO follows the airdrop rules set by the project. Both specific and random airdrops can be supported.

## Q: If it’s a random airdrop, how does Bend DAO distribute airdrops?&#x20;

A: The distribution process on Bend is also random. For fairness and safety, Bend random algorithm which is based on [Chainlink VRF infrastructure](https://vrf.chain.link/mainnet) to distribute tokens.&#x20;

The VRF subscription id is on Chainlink: [81](https://vrf.chain.link/mainnet/81).

The code for airdrop distribution is on[ ](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol)Github: [AirdropDistribution.sol](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol).&#x20;

The contract address on[ ](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD)Etherscan: [0x6D187449A5664DD87E58A9d3b982989AaeA469BD](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD).

## Q: What if I miss the claim period?&#x20;

A: You can always Flash Claim airdrops on Bend. Your airdrop never expires.

## Q: Can I Flash Claim if I have no knowledge of programming?&#x20;

A: You can simply click the Flash Claim button to claim your airdrops. There are no programming requirements.

## Q: What is boundNFT?&#x20;

A: For NFT-backed loans, when the borrower deposits an NFT in Bend DAO, a boundNFT will be minted as a Debt NFT. For Custody, when the NFT holder deposits an NFT in Bend DAO, a boundNFT will be minted as a receipt NFT.&#x20;

More details of boundNFT https://docs.benddao.xyz/portal/highlights/true-ownership

## Q: Is the Flash Claim open-sourced?&#x20;

A: Yes. Visit BoundNFT Github to find more details. https://github.com/BoundNFT/boundnft-protocol/tree/main/contracts

## Q: Can I realize the Flash Claim by myself if I have programming experience?&#x20;

A: Yes. Users also can write a contract to implement the Flash Claim. Please check the demo on Github. https://github.com/BendDAO/bend-flashclaim-demo

## Q: What kind of airdrops will be supported on Bend?&#x20;

A: Yuga Metaverse Land, of course. Technically, all airdrops that are related to the collaterals can be supported. Bend supported collaterals are BAYC, CryptoPunks, MAYC, Azuki, CloneX, and Doodles.

Feel free to find the team in Discord if you want us to support other great airdrops.
