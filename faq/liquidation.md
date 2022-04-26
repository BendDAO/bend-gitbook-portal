# Liquidation FAQ

## An example of liquidation

Assuming that the floor price of BAYC is 100 ETH when you borrow 40 ETH instantly in Bend DAO.

If the floor price drops to 44 ETH, the 48h liquidation protection will be triggered since the health factor of your NFT-backed loan is below 1.

Health Factor = (44 \* 90%) / (40 + interests) <1&#x20;

Health Factor = (Floor Price \* Liquidation Threshold) / Debt with Interests.

## What is the health factor?

The health factor is the numeric representation of the safety of your deposited NFT against the borrowed ETH and its underlying value. The higher the value is, the safer the state of your funds are against a liquidation scenario.

If the health factor reaches 1, the liquidation of your deposits will be triggered. A Health Factor below 1 can get liquidated. For a HF=2, the collateral value vs borrow can reduce by 1 out of 2: 50%.

The health factor depends on the liquidation threshold of your collateral against the value of your borrowed funds.

You can find all of the collateral parameters in the [risk parameters](../risk/nft-risk-parameters.md) section.

## What happens when my health factor is reduced?

Depending on the value fluctuation of your deposits, the health factor will increase or decrease. If your health factor increases, it will improve your borrow position by making the liquidation threshold more unlikely to be reached. In the case that the value of your collateralized assets against the borrowed assets decreases instead, the health factor is also reduced, causing the risk of liquidation to increase.

## **How does Bend calculate the value of the collateralized NFT?**

NFT floor prices are currently used as the price feeds for the collateralized NFTs. \*\*\*\* The original price data comes from OpenSea, the most well-known NFT marketplace. The collateral value is denominated in Ether instead of USDT on Bend.

## **Any plan to upgrade the NFT price feeds design?**

Since there is no sophisticated NFT price feed solution in the market now, using floor prices may be the safest choice. Bend will consider involving a new NFT Oracle when a better option arises.

## **Why does the market liquidation crisis NOT happen in Bend?**

48h Liquidation Protection and NFT Auction mean that the NFT will not be liquidated immediately. Meanwhile, the liquidator's bid must be equal to the floor price on OpenSea.

More details of [48h Liquidation Protection](../highlights/48h-liquidation-protection.md).

## **What will happen if liquidation occurs?**

A 48-hour liquidation protection mechanism is triggered by a smart contract when liquidation occurs. The borrower (user with the collateralized NFT) will be able to repay the loan within the 48-hour window.\
\
A Discord bot will be set up to update the loan status for borrowers.\
\
During the 48-hour liquidation protection period, an NFT auction will be activated.

## **What's the liquidation threshold on Bend?**

If collateral has a liquidation threshold of 90%, the loan will be liquidated when the debt value is worth 90% of the collateral value. The liquidation threshold is specified per collateral and expressed in percentage points.

## **Will my loan be liquidated if the price of Ether drops?**

All NFTs are denominated in Ether instead of USDT on Bend. The price of Ether and the price of NFT are not necessarily related.

## **Does the borrower need to keep paying interest while the 48-hour liquidation protection mechanism is active?**

Yes. Because the NFT-backed loan is still active during the 48-hour liquidation protection. For safety and fairness, borrowers need to pay a penalty (1% of the bid price in default) to the liquidator, even after NFT floor prices recover to the normal price.

## **What if no liquidator shows up?**

We believe that this will not happen. The liquidation mechanism is designed with a comprehensive incentive mechanism, such as discount purchase of NFT, redeeming fines, etc., and the liquidator participating in the auction can get a generous arbitrage.

## What if the floor price drops and the auction bid can’t cover it?

It will not happen, since the bid must be 1) more than 95% of the floor price; 2) bigger than the total accumulated debt; 3) higher than the previous bid.

If no liquidator shows up, for the safety of the protocol, the Bend DAO will participate in the NFT auction if no third-party liquidator is interested in the collateralized bluechip NFT. Security is always the first priority with Bend.

## What will happen if the floor price drops to 0?

Bluechip NFTs are fast-growing assets that appreciate faster than ETH and the whole market is still early.

Bend will only list high-quality bluechip NFTs that have been recognized by the market, and that have at least experienced multiple cycles of ups and downs.

Bend is continuously monitoring the market indicators of bluechip NFTs, and timely adjust risk parameters through community governance, such as collateral ratio and delisting NFTs.

