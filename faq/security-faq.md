# Security FAQ

## Q: How does BendDAO stay secure?&#x20;

A: BendDAO team has spent all the necessary resources in order to ensure that the protocol matches the highest security standards.

* The second audit report by Verilog. [https://www.verilog.solutions/audits/BendDAO](https://www.verilog.solutions/audits/BendDAO)
* Before BendDAO Mainnet launch, Certik issued an audit report for BendDAO. [https://www.certik.com/projects/bend-dao ](https://www.certik.com/projects/bend-dao)
* Up to $1m BendDAO Bug Bounty [https://immunefi.com/bounty/benddao/](https://immunefi.com/bounty/benddao/)&#x20;
* All boundNFT Protocol Contracts with 7 days timelocks.
* All BendDAO Lending Protocol Contracts with 24 hours timelocks.

https://docs.benddao.xyz/portal/risk/security-and-audits

## Q: How can timelocks protect users?&#x20;

A: Timelocks are used to add a delay of key operations such as contracts upgrading and token transferring, enabling users to know the operations and take action before the protocol operations really take effect. This time delay gives users a chance to exit protocol if the team becomes malicious or compromised.

* All boundNFT Protocol Contracts - 7 days timelocks&#x20;
* All BendDAO Lending Protocol Contracts - 24 hours timelocks&#x20;

More details of Timelock: [https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller](https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller)

## Q: How can users monitor timelocks?&#x20;

A: Users can set up alerts using Etherscan. Emails will be sent once any contract change is confirmed on a contract address including funds transactions and protocol upgrades. Here is the guide on how to set up email notifications. [https://info.etherscan.com/watch-list/](https://info.etherscan.com/watch-list/)

All boundNFT Protocol Contracts - 7 days timelocks: [https://etherscan.io/address/0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e ](https://etherscan.io/address/0x4e4C314E2391A58775be6a15d7A05419ba7D2B6e)

All BendDAO Lending Protocol Contracts - 24 hours timelocks: [https://etherscan.io/address/0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214](https://etherscan.io/address/0x652DB942BE3Ab09A8Fd6F14776a52ed2A73bF214)&#x20;

## Q: Why does BendDAO use upgradeable proxy contracts?&#x20;

A: The reason why we use an upgradeable proxy for the BendDAO contracts is to make sure the funds are safe. The team can improve the functionality with the upgradeable proxy if some bugs are found.

To avoid trust issues, all contracts have timelocks. Timelocks are a smart contract feature that states that upgrades will only be performed after a certain period of time rather than immediately. All users have a window of time to take action before upgrades really take effect.

* All boundNFT Protocol Contracts - 7 days timelock&#x20;
* All BendDAO Lending Protocol Contracts - 24 hours timelock&#x20;

More details of Timelocks: [https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller](https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller)

## Q: I worry about the rug pull, what if BendDAO rug pull?&#x20;

A: A rug pull in the crypto is when the team suddenly abandons a project and sells or removes all its liquidity from the Dex.

DAO members instead of the team provide all BEND/ETH liquidity on Uniswap. The first team token release will happen on May 9th, 2023 at 14:29 UTC. The team doesn’t have any BEND tokens now.

Team token contract details: [https://mirror.xyz/benddaoteam.eth/VLTqI6yPC\_YojeUreU1YvJfHT27KFEkHFW5BN1CH48M](https://mirror.xyz/benddaoteam.eth/VLTqI6yPC\_YojeUreU1YvJfHT27KFEkHFW5BN1CH48M)

## Q: What if the BendDAO team takes away all bluechip NFTs and ETH from the lending pool?&#x20;

A: Technically, only the borrowers’/ lenders’ addresses can call the withdrawal function. More details of the BendDAO protocol: https://github.com/BendDAO

## Q: What if the BendDAO team whitelists their addresses to withdraw all bluechip NFTs and ETH from the lending pool?&#x20;

A: Technically, the team is not able to do that. But even if the team can, there will be a delay in implementation because of the timelocks. Timelocks enable users to know the updates and take action before the protocol upgrades really take effect. This time delay gives users a chance to withdraw all assets and exit the protocol if the team becomes malicious or compromised.

More details of the BendDAO protocol: [https://github.com/BendDAO ](https://github.com/BendDAO)

More details of Timelocks: [https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller](https://docs.benddao.xyz/portal/risk/security-and-audits#timelock-controller)

## Q: Any insurance for BendDAO smart contracts?&#x20;

A: No. Since insurance would not work for scalable protocol. And no insurance really covered the loss of DeFi exploitations before. Secure operations and audits are the keys to diminishing risks of security vulnerabilities instead of insurance.
