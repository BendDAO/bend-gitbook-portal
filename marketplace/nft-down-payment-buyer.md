# NFT 首付（买家）

The buyer can pay a minimum down payment of 60%, depending on the actual price, to buy a bluechip NFT while initiating a flash loan from AAVE to cover the remainder. If the total price of the NFT is much higher than the collection floor price, the percentage of the down payment will increase. The borrowed amount of the flash loan will be repaid through the instant NFT-backed loan on BendDAO.

To be specific, the workflow of BendDAO NFT down payment is as follows.&#x20;

1. The buyer pays a minimum down payment of 60%;&#x20;
2. A flash loan is initiated to borrow the remainder from a third-party platform, e.g. AAVE;&#x20;
3. The newly purchased NFT will be used as collateral on BendDAO to get instant liquidity;&#x20;
4. The flash loan will be repaid with the borrowed ETH from BendDAO.

The buyers will automatically become borrowers with the down payment. And borrowers can list their mortgaged NFT for sale on the BendDAO marketplace as well.

The supported NFT collections are BAYC, CryptoPunks, MAYC, Doodles, Space Doodles, CloneX and Azuki. The percentage of the down payment is determined by [the LTV on BendDAO](https://docs.benddao.xyz/portal/highlights/instant-lending-and-repayments).&#x20;
