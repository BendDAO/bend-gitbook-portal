# Otherdeeds with KODA FAQ

## KODA and BendDAO NFT Wrapper Contract

KODA is a collection of 10,000 creatures that inhabit Otherdeeds of Otherside.

The BendDAO NFT wrapper contract allows the recognition of different traits in NFT collections while creating wrapped versions of them. With the BendDAO NFT Wrapper contract, Otherdeeds with KODA traits can be used as collateral on BendDAO. ([BIP#20](https://snapshot.org/#/benddao.eth/proposal/0xcc2ef1acd927a78f6ca2bfc93b05eaf015ce3c2ce07707910d8a4e9416c4c521))

Details of the Audit Report: [https://www.verilog.solutions/audits/benddao\_nft\_wrapper/](https://www.verilog.solutions/audits/benddao\_nft\_wrapper/)

## FAQ

#### Q: Can I use my Otherdeeds NFT as collateral to borrow instant ETH on BendDAO?

A: Yes, if your Otherdeed contains a KODA.

Parameters:

* LTV / Collateral Ratio: 30%
* Liquidation Threshold: 80%
* Auction & Redeem Duration: 24 hours
* Redeem Fine: maximum (5% of the debt, 0.2 ETH)
* Redeem Threshold: 50%

#### Q: Since BendDAO supports KODA, can I buy a KODA with down payments?

A: Sorry, no for now. Because the KODA is not a separate collection. The KODA NFT needs to be wrapped to borrow ETH.

#### Q: We know that Yuga intends to separate the KODA from the Otherdeeds land at some point. What if they enable the movement of KODAs out of existing lands, is the BendDAO contract equipped to recognize that and disallow that land as collateral?

A: Flash Claim for KODA is disabled to avoid this kind of situation. And the KODA-backed loan may be paused when departing which will be updated based on Yuga’s future announcement.

#### Q: If the flash claim is disabled, does that mean I need to pay off the loan to get the separated KODA NFT?

A: It depends on Yuga’s future announcement. Join our Discord to stay tuned. [http://discord.gg/BendDAO](http://discord.gg/BendDAO)

#### Q: What will happen when wrapped KODA is liquidated?

A: No difference with the other NFTs. The liquidator will get the unwrapped KODA when the auction ends.
