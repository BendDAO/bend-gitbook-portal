# Liquidation and Redeem

The Bend Protocol utilizes a scored 'health factor' for loans. The formula is outlined below.

When the 'health factor' of an NFT loan is below 1, anyone can trigger a liquidation in terms of an [**NFT Auction**](auction.md). The liquidator is called Bidder on BendDAO. The bidder will pay back all of the debt and receive the collateralized NFT in return. The borrower can redeem his NFT to exit auction by repaying some loan debts (50% in default).

Please read the[ auction](auction.md) for liquidation details.

## Meaning of Health Factor

The definition for Health Factor: (Floor Price \* Liquidation Threshold) / Debt with Interests.

The risk level of the health factor:

* 0.0 < HF < 1.0: <mark style="color:red;background-color:red;">Dangerous</mark>, borrower maybe lose collateral if the debt is not repaid timely.
* 1.0 <= HF <= 1.5: <mark style="color:orange;background-color:red;">Risky</mark>, borrower should repay partly the debt timely.
* 1.5 < HF < 2.0: <mark style="color:yellow;background-color:yellow;">Careful</mark>, borrower should pay attention and monitor the debt timely.
* 2.0 <= HF: <mark style="color:green;background-color:green;">Safe</mark>, borrower no need to worry and keep the debt last.

Liquidation will be triggered if the NFT loan's health factor is below 1.

## NFT Loan State

![](<../.gitbook/assets/NFT Loan State 0320.jpg>)
