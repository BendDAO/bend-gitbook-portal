# NFT Risk Parameters

The DeFi ecosystem is built by DeFi projects. The risk assessment considers market and smart contract risks for the NFTs selected for Bend protocol.

The risk framework aims to analyse the inherent risks of the NFT assets in the Bend Protocol and describes the processes in place to mitigate them.

With Bend, NFT holders will now be able to actively participate in the DeFi ecosystem. However, it also exposes the protocol to financial contagion. NFT collateral used in the protocol affects the protocol at its core, in particular NFT projects accepted as collateral which safeguard the solvency of the protocol. To ensure a currency holds a reasonable amount of risk, we investigate five different parameters.

Refer to the NFT Performance Map designed by nonfungible.com, five key metrics will be involved.

* Trade Volume (Number of sales)
* Asset value (Average asset sales value)
* Interactions (Number of dapp transactions, including bids and other interactions)
* Community (Number of unique wallets interacting at the dapp level)
* Retention (Percentage of how many days a wallet is active in the time period, for example a retention rate of 14.3% indicates that users are only active one day of the week)

The table below shows a summary of the latest values.

| Name           | Symbol      | LTV / Collateral Ratio | Liquidation Threshold | Redeem Duration | Auction Duration | Redeem Fine                       | Redeem Threshold |
| -------------- | ----------- | ---------------------- | --------------------- | --------------- | ---------------- | --------------------------------- | ---------------- |
| Bored Ape YC   | BAYC        | 40%                    | 85%                   | 24 hours        | 24 hours         | maximum (5% of the debt, 0.2 ETH) | 50%              |
| CryptoPunks    | CryptoPunks | 40%                    | 85%                   | 24 hours        | 24 hours         | maximum (5% of the debt, 0.2 ETH) | 50%              |
| Mutant Ape YC  | MAYC        | 30%                    | 85%                   | 24 hours        | 24 hours         | maximum (5% of the debt, 0.2 ETH) | 50%              |
| Azuki          | AZUKI       | 30%                    | 85%                   | 24 hours        | 24 hours         | maximum (5% of the debt, 0.2 ETH) | 50%              |
| CLONE X        | CLONEX      | 30%                    | 85%                   | 24 hours        | 24 hours         | maximum (5% of the debt, 0.2 ETH) | 50%              |
| Doodles        | DOODLE      | 30%                    | 85%                   | 24 hours        | 24 hours         | maximum (5% of the debt, 0.2 ETH) | 50%              |
| Space Doodles  | SDOODLE     | 30%                    | 85%                   | 24 hours        | 24 hours         | maximum (5% of the debt, 0.2 ETH) | 50%              |

_\*The liquidation protection and liquidation threshold are adjusted to 24 hours based on_ [_BIP#9 & BIP#10._](../governance/benddao-improvement-proposals-bips.md) _Updated as of August 30th, 2022._
