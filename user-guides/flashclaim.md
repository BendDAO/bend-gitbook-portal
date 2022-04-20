# Flash Claim

Flash Claim is build on BoundNFT's Flash Loan. Through Flash Claim, you can use your NFT to claim third parties airdrop without repaying to lending pool.

For well-known airdrop projects, Bend will officially make adaptations. Users do not need to develop contract codes and understand the underlying technical details. They only need to select the airdrop project and their own NFT on the webpage to quickly complete the claim.

For those airdrop projects that have not officially supported, if you think it is good project, please give feedback in the Discord community. Bend will try to give priority to support if there is sufficient manpower and time.

Bend supports two types of airdrop projects, the first type is that the user actively initiates the transaction to claim airdrop, the second is that the project party actively airdrops to the user.

For the first type, Bend use boundNFT's Flash Loan to support user claim airdrop, the code for airdrop flash loan is on [Github](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropFlashLoanReceiver.sol), and contract address on [Etherscan](https://etherscan.io/address/0xa8Ae91Dd8CD8f410BA59626caef160925A033734).

![](<../.gitbook/assets/Flash claim 04191810.jpg>)

For the second type, Bend will do snapshot and airdrop distribution to support user claim airdrop. If   airdrop project party use some random algorithm to distribute tokens, we also use random algorithm which is based on [Chainlink VRF infrastructure](https://vrf.chain.link/mainnet) to distribute tokens, for fairness and safety, the code for airdrop distribution is on [Github](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol), and contract address on [Etherscan](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD).

![](<../.gitbook/assets/Airdrop Distribution 04191825.jpg>)

## Using Flash Claim UI

Step 1: Go to Dashboard and click Claim your airdrop.

Step 2: Choose airdrop project and click Claim.

Step 3: Your will get airdrop tokens in wallet after claim transaction is succeeded.

![](<../.gitbook/assets/Flashclaim Page 04201331.jpg>)

![](<../.gitbook/assets/Dashboard Flashclaim 02401330.jpg>)

![](<../.gitbook/assets/Flashclaim Page 04201331.jpg>)

## Flash Claim Code Demo

For advance users, you can write contract to implement claim, please check demo at [Github](https://github.com/BendDAO/bend-flashclaim-demo).
