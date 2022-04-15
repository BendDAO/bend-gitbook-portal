# - Adding an NFT

Bend protocol enables NFT loans through the pooling of funds. Each loan is secured by an NFT collateral acting as a risk mitigation tool against default.

Given the specificities of Bend’s evaluation model, the selection of NFTs has been performed with the following constraints:

1. Each additional NFT will slightly increase the gas cost of the borrow and repay actions permanently. The currency must be included in the smart contract, adding complexity and thus costs.
2. Each NFT added to Bend protocol as collateral increases the protocol risk of insolvency. From a financial perspective, the assets of Bend Protocol are the collaterals, while the liabilities are the loaned amounts. The underlying floor price of assets and liabilities often differ, with loans mostly taken in ETHs and backed by volatile NFTs. This means the protocol is heavily exposed to the failure of supported token systems as well as market fluctuations.
3. A centralized NFT accepted as collateral exposes the protocol to its centralization risk. The single point of failure risks of underlying currencies flow into Bend Protocol.
4. Collaterals are the assets of the protocol. To remain solvent, these assets must remain greater than the liabilities, the loans.

When adding a NFT to the protocol, significant controls are required to ensure the NFT will add more value than risk. Only NFTs with a great reputation and significant community are considered.&#x20;

In the first phase of project development, CryptoPunks, Bored Ape Yacht Club, Doodles, Meebits and Cool Cats can be used as collateral for NFT loans.
