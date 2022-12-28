# Security and Audits

## Audits

BendDAO protocol has been implemented with security as the top priority. The system has been designed to be safe and secure, and we have spent all the necessary resources in order to ensure that the protocol matches the highest security standards.

Below are the links to all audit reports for BendDAO.

| Auditor           | Scope             | Date       | Report                                                                                                                       |
| ----------------- | ----------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Verilog Solutions | Ape Staking       | 2022-12-05 | [https://www.verilog.solutions/audits/bend\_apecoin\_staking/](https://www.verilog.solutions/audits/bend\_apecoin\_staking/) |
| Verilog Solutions | Exchange Protocol | 2022-08-03 | [https://www.verilog.solutions/audits/benddao\_liquidity/](https://www.verilog.solutions/audits/benddao\_liquidity/)         |
| Verilog Solutions | Lending Protocol  | 2022-05-26 | [https://www.verilog.solutions/audits/benddao/](https://www.verilog.solutions/audits/benddao/)                               |
| Certik            | Lending Protocol  | 2022-03-14 | [https://www.certik.com/projects/bend-dao](https://www.certik.com/projects/bend-dao)                                         |

{% hint style="info" %}
Regarding the Unresolved Major issues in the Certik report:

1. For the risk of centralization, BendDAO has deployed **Timelock Controller** and **Multi-Signature Wallet**, please read the details [here.](security-and-audits.md#timelock-controller)
2. For the NFT Oracle, BendDAO has adopted various solutions such as backup nodes, time weighting, and threshold checking, please read the details [here](../lending-protocol/oracle-price-feeding.md).
{% endhint %}

## Timelock Controller

BendDAO has set the owner of all bend lending protocol contracts to 7 days time lock controller address.

BendDAO has set the owner of all bound NFT protocol contracts to 7 days time lock controller address.

<figure><img src="../.gitbook/assets/Timelock 1228.jpg" alt=""><figcaption></figcaption></figure>

| Name                | Duration | Address                                                                                                               |
| ------------------- | -------- | --------------------------------------------------------------------------------------------------------------------- |
| BendDAO Timelock 7D | 7 Days   | [0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e](https://etherscan.io/address/0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e) |

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

## Proxy Admin

| Name          | Owner Type      | Address                                    |
| ------------- | --------------- | ------------------------------------------ |
| BoundNFT      | 7 Days Timelock | 0xe635D0fb1608aA54C3ca99c497E887d2e1E3E690 |
| Lending Pool  | 7 Days Timelock | 0x501c991E0D31D408c25bCf00da27BdF2759A394a |
| Treasury Fund | 7 Days Timelock | 0x2A71a0F5cef1fFc519027AD12f19453110e70666 |
| Incentive     | 7 Days Timelock | 0x859f6e05410893fe64BC84d92BdA773fF798cf66 |
| Team Lockup   | 7 Days Timelock | 0x49b1fE3db39D8ee873b4B45602A5127E99d4cfF6 |
| Ape Staking   | 7 Days Timelock | 0xdBE0985E7570041e1BDfB6DeD30E159CFb3718CF |
