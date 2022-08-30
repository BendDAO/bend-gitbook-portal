# Auction

The NFT auction design ensures Bend remains both decentralized and sustainable. It is likely the best method to find the real price of NFT assets.

## The Design of NFT Auction

An NFT auction will be initiated when the health factor is below 1. More specifically, if the collateral has a liquidation threshold of 90%, the loan will be liquidated when the debt value is worth 90% of the collateral value. The liquidation threshold is specified per collateral and expressed in percentage points.

* An open-outcry ascending dynamic auction system
* The system opens the auction with a starting price. The starting price will be 1) bigger than the total accumulated debt.
* If the borrowers repay the loan in 24 hours, he/she will pay a fine to the first bidder.
* The fine will take the larger of 5% debt or 0.2 ETH. Fine = maximum (5% of the debt, 0.2 ETH)

### Bidder

* Anyone can take part in an auction.
* The bid must be:1) no less than the starting price;  2) higher than the previous bid plus 1% debt.
* The first bidder will receive at least 0.2 ETH paid by the borrower as the penalty if the borrower repays within 24 hours.&#x20;
* The highest bidder will get the collateral if the borrower doesn't repay the loan.
* The bidder needs to deposit ETH to bid.
* The deposited ETH will automatically be refunded in wETH when his/her bid is not the highest bid.

### Borrower

* The borrower will have a[ liquidation protection](../highlights/48h-liquidation-protection.md) period to repay the loan.
* If the borrower repays within 24 hours, he/she will pay a fine of a maximum(5% of the debt, 0.2 ETH) to the first bidder.
* If the collateral is sold in auction for greater than the loan amount, the excess will belong to the borrower.

{% hint style="info" %}
[Liquidation FAQ](../faq/liquidation.md)
{% endhint %}
