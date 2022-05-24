# Liquidation and Redeem

The Bend Protocol utilizes a scored 'health factor' for loans. The formula is outlined below.

When the 'health factor' of an NFT loan is below 1, anyone can trigger a liquidation in terms of an [**NFT Auction**](auction.md). The liquidator is called Bidder on Bend. The bidder will pay back all of the debt and receive the collateralized NFT in return.

![](<../.gitbook/assets/image (3).png>)

Please read the[ auction](auction.md) for liquidation details.

## Health Factor

The definition for Health Factor: (Floor Price \* Liquidation Threshold) / Debt with Interests.

The risk level of the health factor:

![Health Factor Risk Level](<../.gitbook/assets/HF Color 0213.jpg>)

Liquidation will be triggered if the NFT loan's health factor is below 1.

## NFT Loan State

![](<../.gitbook/assets/NFT Loan State 0320.jpg>)
