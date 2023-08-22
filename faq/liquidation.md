# Liquidation FAQ

## An example of liquidation

Assuming that the floor price of BAYC is 100 ETH when you borrow 60 ETH instantly on BendDAO.

If the floor price drops to 75 ETH, the 24h liquidation protection can be triggered since the health factor of your NFT-backed loan is below 1.

Health Factor = (75 \* 80%) / (60 + interests) <1&#x20;

Health Factor = (Floor Price \* Liquidation Threshold) / Debt with Interests.

_\*The liquidation protection and liquidation threshold are adjusted based on_ [_BIP#9 & BIP#10._](../governance/benddao-improvement-proposals-bips.md) _Updated as of August 30th, 2022._

_\*The LTV of BAYC, CryptoPunks, and MAYC are adjusted based on_ [_BIP#15_](https://snapshot.org/#/benddao.eth/proposal/0x1bd2cb68f3577f97605b542a7094e0d350a427e516ff30503e8172cc89feb9e6)_. Updated as of December 20th, 2022._

## What is the health factor?

The health factor is the numeric representation of the safety of your deposited NFT against the borrowed ETH and its underlying value. The higher the value is, the safer the state of your funds are against a liquidation scenario.

If the health factor reaches 1, the liquidation of your deposits can be triggered. A Health Factor below 1 may get liquidated. For a HF=2, the collateral value vs borrow can reduce by 1 out of 2: 50%.

The health factor depends on the liquidation threshold of your collateral against the value of your borrowed funds.

You can find all of the collateral parameters in the [risk parameters](../risk/nft-risk-parameters.md) section.

## What happens when my health factor is reduced?

Depending on the value fluctuation of your deposits, the health factor will increase or decrease. If your health factor increases, it will improve your borrow position by making the liquidation threshold more unlikely to be reached. In the case that the value of your collateralized assets against the borrowed assets decreases instead, the health factor is also reduced, causing the risk of liquidation to increase.

## **How does Bend calculate the value of the collateralized NFT?**

NFT floor prices are currently used as the price feeds for the collateralized NFTs. The original price data comes from OpenSea and LooksRare, the most well-known NFT marketplaces. The collateral value is denominated in Ether instead of USDT on Bend.&#x20;

More details: [https://docs.benddao.xyz/portal/protocol-overview/oracle-price-feeding](https://docs.benddao.xyz/portal/protocol-overview/oracle-price-feeding)

## **Any plan to upgrade the NFT price feeds design?**

Since there is no sophisticated NFT price feed solution in the market now, using floor prices may be the safest choice. Bend will consider involving a new NFT Oracle when a better option arises.

## **Why does the market liquidation crisis NOT happen in Bend?**

24h Liquidation Protection and NFT Auction mean that the NFT will not be liquidated immediately.

More details of [Liquidation Protection](../highlights/48h-liquidation-protection.md).

## **What will happen if liquidation occurs?**

When the 'health factor' of an NFT loan is below 1, a bidder can trigger a liquidation in terms of an [**NFT Auction**](../lending-protocol/auction.md) and the 24h liquidation protection**.**&#x20;

The borrower (user with the collateralized NFT) will be able to repay the loan within the 24-hour window.

## **What's the liquidation threshold on Bend?**

The liquidation threshold is the maximum loan to value (LTV) which means debt plus interest to collateral value. If collateral has a liquidation threshold, the loan will be liquidated when the debt value is worth the liquidation threshold of the collateral value. The liquidation threshold is specified per collateral and expressed in percentage points.

_\*More details of the adjustment of the_ [_Liquidation Threshold_](../governance/benddao-improvement-proposals-bips.md)_._&#x20;

## **Will my loan be liquidated if the price of Ether drops?**

All NFTs are denominated in Ether instead of USDT on Bend. The price of Ether and the price of NFT are not necessarily related.

## **Does the borrower need to keep paying interest while the liquidation protection mechanism is active?**

Yes. Because the NFT-backed loan is still active during the 24-hour liquidation protection. For safety and fairness, borrowers need to pay a penalty of a maximum(5% of the debt, 0.2 ETH) to the first bidder, even after NFT floor prices recover to the normal price.

We believe that this will not happen. The liquidation mechanism is designed with a comprehensive incentive mechanism, such as the discount purchase of NFT, redeeming fines, etc., and the liquidator participating in the auction can get a generous arbitrage.

## What if the floor price drops and the auction bid can’t cover it?

It will not happen, since the bid must be:

1. bigger than the total accumulated debt.
2. higher than the previous bid plus 1% debt.

## What will happen if the floor price drops and there is no liquidator involved in the auction?

First, we should define whether it is short-term fluctuations. The short-term fluctuations in NFT floor price are normal. Consensus on bluechip NFTs wasn't built in a day, and it will not be collapsed in a short period of time.

In this case, the platform only has a temporary floating loss and no actual losses. Either the borrower will repay the debt at some point in the future, or after the market price recovers, some liquidators emerge to take part in auctioning off the debt. Liquidation records: [Dune](https://dune.com/cgq0123/Bend-DAO)

The delisting may happen when the collection is not considered bluechip NFTs anymore.

Delisting reference: [https://governance.benddao.xyz/t/nft-delisting-reference/53](https://governance.benddao.xyz/t/nft-delisting-reference/53)

## What will happen if the floor price drops to 0?

BendDAO will only list high-quality bluechip NFTs that have been recognized by the market, and that have at least experienced multiple cycles of ups and downs. Here are the bluechip NFT eligibility requirements decided through governance.  [https://docs.benddao.xyz/portal/risk/bluechip-nft-eligibility-requirements](https://docs.benddao.xyz/portal/risk/bluechip-nft-eligibility-requirements)

BendDAO is continuously monitoring the market indicators of bluechip NFTs, and timely adjust risk parameters through community governance, such as collateral ratio and delisting NFTs.

The delisting may happen when the collection is not considered bluechip NFTs anymore.

Delisting reference: [https://governance.benddao.xyz/t/nft-delisting-reference/53](https://governance.benddao.xyz/t/nft-delisting-reference/53)

## Any royalty for the auction?

No. There is no royalty for the auction on BendDAO.

## If I'm the highest bidder, how can I get the NFT?

There will be a "Liquidate" button on the auction page for the highest bidder after the auction. The liquidated NFT will be transferred to your wallet after you click the button.

## If I use batch borrow, how many loans will be created?

One NFT one loan. Each loan has its own health factor.

## If my bid is not the highest one, do I need to claim my bid?

No. Your bid will automatically be refunded to your wallet in WETH.

## If the bid exceeds the debt, who will receive the difference?&#x20;

The borrower. If the collateral is sold in an auction for greater than the loan amount, the excess will belong to the borrower.

