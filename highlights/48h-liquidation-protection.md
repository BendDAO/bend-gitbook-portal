---
description: Never get liquidated if you repay within 24 hours
---

# Liquidation Protection

You can check this for an example of liquidation: https://github.com/BendDAO/bend-gitbook-portal/blob/main/faq/liquidation.md#an-example-of-liquidation

## Liquidation Protection

**Never get liquidated if you repay within 24 hours**

NFT holders don’t want to hand over the ownership of their NFTs. That's why they look for other liquidity solutions instead of selling NFTs. In order to avoid losses caused by the market fluctuations, the borrower will have a 24-hour liquidation protection period to repay the loan. Your NFT-backed loan will never get liquidated if you repay within the 24-hour liquidation protection period.

**Borrower (Collateralized NFT)**

During the auction (24h liquidation protection period), for the NFT holder's safety, the borrower (user with the collateralized NFT) will still be able to repay the loan within the 24-hour window starting from the beginning of the auction.

{% hint style="warning" %}
For safety and fairness, borrowers must repay some loan debts (50% in default) as well as pay a penalty of a maximum(5% of the debt, 0.2 ETH) to the liquidator, even after NFT floor prices recover to the normal price.
{% endhint %}

**Bidder**

Under the Bend Auction mechanism, any bidder can obtain ownership of an NFT as long as the bid is higher than the floor price. This way, all NFTs will be given a price discovery mechanism, making transactions transparent.

Bend’s Protocol is dependent on the 'health' of loans within the system, also known as the 'health factor' which is related to debt, floor pricings, and liquidation thresholds.

In order to avoid losses caused by the market fluctuations, an NFT auction will be activated when the health factor is below 1. Anyone can partake in auctions but for NFT holders’ safety, there will be a 24-hour auction window where they'll be able to repay loans. Once the auction begins, bidders will be able to bid as long as the bid is higher than the previous price placed.



_\*The liquidation protection is adjusted to 24 hours based on_ [_BIP#9 & BIP#10._](../governance/benddao-improvement-proposals-bips.md)__
