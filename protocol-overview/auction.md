# Auction

The NFT auction design ensure Bend remains both decentralized and sustainable. It is likely the best method to find real price of NFT assets.

## The Design of NFT Auction

An NFT auction will be initiated when the health factor is below 1.  More specifically, if the collateral has a liquidation threshold of 80%, the loan will be liquidated when the debt value is worth 80% of the collateral value. The liquidation threshold is specified per collateral and expressed in percentage points.

* An open-outcry ascending dynamic auction system
* The system opens the auction with a starting price. The starting price will be 1) more than 95% of the floor price; and 2) bigger than the total accumulated debt.
* If the borrowers repay the loan in 48 hours, he/she will pay penalty fine (1% bid price) to the latest bidder.

### Bidder

* Anyone can take part in an auction.
* The bid must be 1) no less than the starting price; and 2) higher than the previous bid.
* Bidder need to deposit ETH to bid.&#x20;
* Bidder can withdraw the deposited ETH when his/her bid is not the highest bid.

### Borrower

* The borrower will have a [48-hour liquidation protection](../highlights/48h-liquidation-protection.md) period to repay the loan.
* If borrower repay within 48 hours, he/she will pay a penalty fine (1% bid price) to the latest bidder.
* If the collateral is sold in auction for greater than the loan amount, the excess will belong to the borrower.&#x20;



{% hint style="info" %}
[Liquidation FAQ](../faq/liquidation.md)
{% endhint %}



