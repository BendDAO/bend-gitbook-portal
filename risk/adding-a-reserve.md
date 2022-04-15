# - Adding a Reserve

Bend enables users to deposit and borrow digital currencies through the pooling of funds. Depositors receive protocol-issued bTokens, which gather deposits and the interest generated. Each loan is secured by NFT collateral acting as a risk mitigation tool against default. As the means of exchange, currencies are central in Bend’s non-custodial lending operations.Given the specificities of Bend’s evaluation model, the selection of currencies has been performed with the following constraints:

1. Each additional currency will slightly increase the gas cost of the borrow and repay actions permanently. The currency must be included in the smart contract, adding complexity and thus costs.
2. A centralized currency accepted as collateral exposes the protocol to its centralization risk. The single point of failure risks of underlying currencies flow into Bend Protocol.
3. Currencies only enabled for depositing and borrowing (not usable as collaterals) present lower risk for the protocol.

When adding a currency to the protocol, significant controls are required to ensure the currency will add more value than risk. Only currencies with a worthy product and significant community are considered. The currency risk assessment explores whether the currencies represent a reasonable amount of risk for the protocol, calibrating the currencies parameters to mitigate those risks.
