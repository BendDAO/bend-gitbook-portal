# Security and Audits

## Audits

BendDAO has been implemented with security as the top priority. The system has been designed to be safe and secure, and we have spent all the necessary resources in order to ensure that the protocol matches the highest security standards.

Below are the links to all audit reports for BendDAO.

| Auditor           | Date       | Report                                                                               |
| ----------------- | ---------- | ------------------------------------------------------------------------------------ |
| Verilog Solutions | 2022-05-26 | [https://hackmd.io/@verilog/benddao-audit](https://hackmd.io/@verilog/benddao-audit) |
| Certik            | 2022-04-01 | [https://www.certik.com/projects/bend-dao](https://www.certik.com/projects/bend-dao) |

{% hint style="info" %}
Regarding the Unresolved Major issues in the Certik report:

1. For the risk of centralization, BendDAO has deployed Timelock Controller and Multi-Signature Wallet, please read the details [here.](security-and-audits.md#timelock-controller)
2. For the NFT Oracle, BendDAO has adopted various solutions such as backup nodes, time weighting, and threshold checking, please read the details [here](../protocol-overview/oracle-price-feeding.md).
{% endhint %}

## Timelock Controller

BendDAO has set the owner of all bend lending protocol contracts to 24 hours time lock controller address.

BendDAO has set the owner of all bound NFT protocol contracts to 7 days time lock controller address.

![](<../.gitbook/assets/Bend MultiSig Wallet & TimeLock 0526.png>)

| Name              | Duration | Address                                                                                                               |
| ----------------- | -------- | --------------------------------------------------------------------------------------------------------------------- |
| BendDAO Timelock  | 24 Hours | [0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214](https://etherscan.io/address/0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214) |
| BoundNFT Timelock | 7 Days   | [0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e](https://etherscan.io/address/0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e) |

## Multi-signature Wallet

BendDAO has used multiple Gnosis Safe Multi-signature wallets in contract upgrading and treasury fund.

BenDAO will transfer the Multi-signature wallet to the community after the Multi-signature election.

| Wallet Name             | Wallet Type | Address                                                                                                               |
| ----------------------- | ----------- | --------------------------------------------------------------------------------------------------------------------- |
| Init Token Distribution | Gnosis Safe | [0x16729FaD4DfD9F7c50f3b52a5deaF842D2c609B7](https://etherscan.io/address/0x16729FaD4DfD9F7c50f3b52a5deaF842D2c609B7) |
| Reserve Treasury        | Gnosis Safe | [0x472FcC65Fab565f75B1e0E861864A86FE5bcEd7B](https://etherscan.io/address/0x472FcC65Fab565f75B1e0E861864A86FE5bcEd7B) |
| Timelock Proposer 1     | Gnosis Safe | [0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C](https://etherscan.io/address/0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C) |
| Timelock Proposer 2     | Gnosis Safe | [0xF1465c7Ea04765853Facc2D1ea68bc6e47bE90e1](https://etherscan.io/address/0xF1465c7Ea04765853Facc2D1ea68bc6e47bE90e1) |
| Timelock Admin          | Gnosis Safe | [0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C](https://etherscan.io/address/0xe6b80f77a8B8FcD124aB748C720B7EAEA83dDb4C) |
