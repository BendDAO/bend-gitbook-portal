# Ape Staking Intro & FAQ

## Ape Staking

BendDAO Ape Staking's goal is to empower anyone holding Yuga assets to join the ApeCoin Staking and maximize the yield. Initially, it is designed to facilitate borrowers' eligibility for the staking when their Apes are used as collateral on BendDAO. Inspired by the community, now the BendApeStaking is open to all users holding Yuga assets.

<figure><img src=".gitbook/assets/BendApeStaking Arch 1201.png" alt=""><figcaption></figcaption></figure>

## How it works

Once the NFTs are deposited in BendDAO, the minted boundNFT will be in the holders’ wallets. With the boundNFT, the user can initiate a pairing listing to pair with ApeCoin holders to join the ApeCoin Staking.

According to the [docs](https://docs.apestake.io/#/README) released by Horizen Labs, the ApeCoin holder will lose all the staked ApeCoin if the paired NFT doesn’t uncommit before selling. That’s why all NFTs need to be deposited before pairing to protect the rights and interests of ApeCoin users.

NFT holders still can sell and borrow ETH on BendDAO when the NFT is deposited.

* Join ApeCoin Staking pairing and enjoy the best yield&#x20;
* Borrow instant ETH liquidity

While participating in staking, users can also continue to borrow ETH from the lending pool.

* List and sell the original NFT on BendDAO

The NFT will automatically be uncommitted when transactions are successful.

When the NFT is sold, the matching contract can perform an uncommit operation in advance through the interceptor at the appropriate time to withdraw all tokens and rewards from the staking contract, and return them to the original NFT holders and ApeCoin holders.

## FAQ

[Security](bendapestaking-intro-and-faq.md#security)

[Pairing Service Fee](bendapestaking-intro-and-faq.md#pairing-service-fee)

[Pairing Listing](bendapestaking-intro-and-faq.md#pairing-listing)

[Staking Rewards](bendapestaking-intro-and-faq.md#staking-rewards)

[Share Ratio](bendapestaking-intro-and-faq.md#share-ratio)

[More Features](bendapestaking-intro-and-faq.md#more-features)

[Gas Cost](bendapestaking-intro-and-faq.md#gas-cost)


### Security

#### **Q: How do you ensure BendApeStaking's security?**

A: First, all BendApeStaking's smart contracts have been fully tested and the coverage is beyond 90%. Second, all smart contracts have been audited by Verilog Solution, you can find the reports [here](risk/security-and-audits.md). Third, the proxy admin owner of the BendApeStaking contracts has been configured with a 24 hours timelock and multi-signature wallet, and we plan to remove the owner through community voting, 1 to 3 months after the mainnet goes live.

#### **Q: Is my NFTs safe in BendApeStaking?**

A: Yes, Your NFTs are locked in the boundNFT protocol which has been configured with a 7 days timelock as the owner. The proxy admin owner of the BendApeStaking smart contract also has been configured with a 24 hours timelock. For the timelock and multi-signature, you can read the detail [here](faq/security-faq.md).

#### **Q: Is My ApeCoin safe in BendApeStaking?**

A: Yes, Your ApeCoin tokens are only locked in the official ApeCoinStaking contract which has been audited also. For our pairing service, only the NFT holders and ApeCoin holders can have operating permission.

#### **Q: If I sell my NFT while it is committed in a BAYC or MAYC pool, will I lose all of my staked ApeCoin?**

NO, YOU WILL NOT LOSE YOUR STAKED $APE. For BoundNFT, BendApeStaking will automatically repay the debt and uncommit from the pool when your NFT is been sold. For Orignal NFT, You must manually uncommit from the pool before it's been sold.

#### **Q: If I sell my NFT while it is committed in a Paired pool, will I lose all of my staked $APE?**

NO, YOU WILL NOT LOSE YOUR STAKED $APE. For BAYC or MAYC holders, please look at the above question. For BAKC holders, You must manually uncommit from the pool before it's been sold.

### Pairing Service Fee

#### **Q: Any charge if I use BendApeStaking service?**

A: If the NFT and ApeCoin are from the same wallet address, there is **NO** fee.

If you pair with others to join the staking, there will be a **4**% pairing service fee based on staking earnings. The service fee is decided by the [community voting](https://snapshot.org/#/benddao.eth/proposal/0x695996117077bf6b2ca93db1673827b4cba647d8a121c09090024d40a4fdbc3e). All the service fees go to the DAO treasury and will be voted by the community to decide how to deal with it soon.

#### **Q: How does BendApeStaking charge the pairing service fee?**

A: The pairing service fee is charged at the time of staking rewards claim, and calculated based on time since the previous claim.

#### **Q: Any chance to change the pairing service fee?**

A: Yes. BendDAO is a DAO owned by the community. Anyone can propose a related proposal to adjust the setting.

### Pairing Listing

#### **Q: Who can use BendApeStaking for the pairing?**

A: Users who hold any of the following assets can join ApeCoin Staking with pairing.

1\) [boundBAYC](lending-protocol/boundnft.md); 2) [boundMAY](lending-protocol/boundnft.md); 3) BAYC; 4) MAYC; 5) BAKC; 6) ApeCoin

#### **Q: Do I need to take out a loan against my BAYC to use this BendApeStaking? I really just want to stake for ApeCoin not risk a loan.**

A: No, you don't need to take out a loan to join. Anyone holding Ape NFT or ApeCoin can join the BendApeStaking. NFTs (including BAKC) need to be deposited before pairing to protect the rights and interests of ApeCoin users.

#### **Q: Do I need to find someone with ApeCoin, or will the platform connect?**

A: Your pairing listing will be displayed on BendDAO to find an ApeCoin holder to pair.

#### **Q: Why do I need to deposit my NFT to join BendApeStaking?**

A: The interest of the paired ApeCoin holders can’t be guaranteed without the NFT deposit. The ApeCoin holder will lose all staked ApeCoin and unclaimed rewards when the NFT holder sells the NFT without uncommit. [Reference](https://docs.apestake.io/#/README?id=if-i-sell-my-nft-while-it-is-committed-in-a-bayc-or-mayc-pool-will-i-lose-all-of-my-staked-apecoin)

Your NFT will be deposited to the BendApeStaking contract when it has been paired with other users.&#x20;

#### **Q: How to make sure my NFT is safe with BendApeStaking?**

A: The audit report will be issued before the BendApeStaking launch. And BendDAO has been running safely for more than 7 months.&#x20;

#### **Q: Can I still sell my NFT?**

A: Yes. You can list when your NFT is participating in the BendApeStaking. When you sell the NFT, the contract will uncommit and return the unclaimed rewards and ApeCoin to the deposit addresses.

#### **Q: Can I still borrow ETH?**

A: Yes. You can borrow instant ETH against your Ape NFT anytime you want.

#### **Q: I’m a borrower, can I join the BendApeStaking?**

A: Yes. You can choose to pair with other ApeCoin holders or you can join the staking with your own ApeCoin.

But if you pay off the loan, the paired staking will be unstaked because the NFT will be transfer from the lending contract to your own wallet.

#### **Q: How long do I need to wait for the pairing?**

A: It depends. If you set your share ratio more attractive, your pair listing properly will be paired with the ApeCoin very soon.&#x20;

#### **Q: How can I get back my NFT during the staking?**

A: Both NFT stakers and ApeCoin staker can end the staking anytime they want, but the user who unstaked needs to pay the gas to make all the assets go back to the owners.

#### **Q: Is there any lock-up period for the pairing?**

A: NO. All users can unstake anytime. The user who unstaked needs to pay the gas to make all the assets go back to the owners.

#### **Q: Will I miss the airdrop when I am staking?**

A: BendDAO supports [flashclaim](https://docs.benddao.xyz/portal/faq/flash-claim-faq) for your NFT, but you need to uncommit first to make sure the ApeCoin holder is safe.

#### **Q: How many co-stakers can join the pairing?**

A: One asset, one address.&#x20;

### Staking Rewards

#### **Q: What if the paired NFT is sold during the staking?**

A: You can claim the staked ApeCoin and unclaimed rewards once the NFT is sold.

#### **Q: When can I claim rewards?**

A: You can claim your rewards anytime. The rewards claim on BendDAO follows the rules of official ApeCoin Staking.

#### **Q: What if liquidation happens?**

A: After the liquidation, the contract will uncommit and return the unclaimed rewards and ApeCoin to the deposit addresses.



### Share Ratio

#### **Q: How to set the share ratio?**

A: The BAYC/MAYC holder who initiates the pairing listing sets the share ratio. The staking rewards will be automatically distributed by the ratio when claimed.

#### **Q: Can I change the share ratio during the staking?**

A: Yes, if the staking hasn't started yet. If the staking starts, you need to end the staking and create a new pairing listing.

#### **Q: When can I withdraw my paired NFT/ApeCoin during the staking?**

A: Anytime. But the co-staker who ends the pairing will pay the reward distribution gas. The unclaimed reward after the 4% pairing service fee will be distributed to each co-staker based on the sharing ratio.

#### **Q: Who can claim the staking rewards?**

A: Every co-staker can claim the rewards.

### More Features

#### **Q: How can I add more ApeCoin to staking order?**

A: The only way to add ApeCoin is unstake and stake with more ApeCoin, the official smart contract does not provide add ApeCoin function.

#### **Q: Can I auto-compounding the staking?**

A: No, the only way to compounding is unstake and stake with more ApeCoin.

#### **Q: Can I claim all the rewards in one transaction for all my staking orders?**

A: The Dev team is working on that, but claim all would not save the gas, it would only save the time you making more than one transaction.

### Gas Cost

#### **Q: Why claim gas for BendDAO staking is more than official website?**

A: BendDAO staking is more complicated than official contract, pairing and preventing ApeCoin holder lost ApeCoin by pairing cost that gas.

#### **Q: Can BendDAO save the gas by distributing the rewards if anyone claim the rewards?**

A: We are figuring out the solution, it won't be easy, need more contract development and auditing, stay tuned.
