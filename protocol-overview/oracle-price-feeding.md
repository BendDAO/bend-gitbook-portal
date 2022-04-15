# Oracle Price Feeding

Bend protocol uses NFT floor price from [opensea.io](http://opensea.io) as data of price feeding for NFT collateral. Bend protocol only supports the bluechip NFT asset's floor price for price feeding on-chain. Bluechip NFT's floor price is not easily manipulated. Besides that bend protocol calculate TWAP of floor price to filter the price fluctuate from [opensea.io](http://opensea.io) marketplace.

Bend oracle design and running mechanism:

1. The off-chain node obtains the raw floor price of NFTs from OpenSea trading markets;
2. Filter the raw floor price data, such as unreasonable deviation from the average price in the recent period;
3. Use the time-weighted average price algorithm (TWAP) to weight the floor price, ensuring price is reasonable;
4. Compare the difference between the price on the chain and the latest floor price to determine whether the floor price needs to be upload on the chain;
5. Call the contract interface to upload the floor price to the on-chain contract;

![Oracle Mechanism](<../.gitbook/assets/Bend NFT Oralce 0320.jpg>)

For security and reliability, we will run multiple nodes to ensure that valid price data can be upload  to on-chian oracle contract in a timely manner at all times.

Bend devs are working with Chainlink team to complete the NFT oracle price feeding.

## Oracle Price Curves

### CryptoPunks Price Curve in 6 months

As shown in the figure, the floor price of the oracle for CryptoPunks is consistent with the average deal price and TWAP price.

![](<../.gitbook/assets/CryptoPunks Price Curve 0401.png>)

### Bored Ape YC Price Curve in 6 months

As shown in the figure, the floor price of the oracle for BAYC is consistent with the average deal price and TWAP price.

![](<../.gitbook/assets/BAYC Price Curve 0401.png>)
