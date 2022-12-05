# Ape Staking Intro & FAQ

## Ape Staking

BendDAO Ape Staking's goal is to empower anyone holding Yuga assets to join the ApeCoin Staking. Initially, it is designed to facilitate borrowers' eligibility for the staking when their Apes are used as collateral on BendDAO. Inspired by the community, now the BendApeStaking is open to all users holding Yuga assets.

<figure><img src=".gitbook/assets/BendApeStaking Arch 1201.png" alt=""><figcaption></figcaption></figure>

## How it works

Once the NFTs are deposited in BendDAO, the minted boundNFT will be in the holders’ wallets. With the boundNFT, the user can initiate a pairing listing to pair with ApeCoin holders to join the ApeCoin Staking.

According to the [docs](https://docs.apestake.io/#/README) released by Horizen Labs, the ApeCoin holder will lose all the staked ApeCoin if the paired NFT doesn’t uncommit before selling. That’s why all NFTs need to be deposited before pairing to protect the rights and interests of ApeCoin users.

NFT holders still can sell and borrow ETH on BendDAO when the NFT is deposited.

* Join ApeCoin Staking pairing
* Borrow instant ETH liquidity

While participating in staking, users can also continue to borrow ETH from the lending pool.

* List and sell the original NFT on BendDAO

The NFT will automatically be uncommitted when transactions are successful.

When the NFT is sold, the matching contract can perform an uncommit operation in advance through the interceptor at the appropriate time to withdraw all tokens and rewards from the staking contract, and return them to the original NFT holders and ApeCoin holders.

## FAQ

### Security

#### Q: How do you ensure BendApeStaking's security?

A: First, all BendApeStaking's smart contracts have been fully tested and the coverage is beyond 90%. Second, all smart contracts have been audited by Verilog Solution, you can find the reports [here](risk/security-and-audits.md). Third, the owner of the BendApeStaking contracts will be configured with a timelock and multi-signature wallet, and we plan to remove the owner through community voting, 1 to 3 months after the mainnet goes live.

#### Q: Is my NFTs safe in BendApeStaking?

A: Yes, Your NFTs are locked in the boundNFT protocol which has been configured with a 7 days timelock as the owner. The owner of the BendApeStaking smart contract also will be configured with a timelock. For the timelock and multi-signature, you can read the detail [here](faq/security-faq.md).

#### Q: Is My ApeCoin safe in BendApeStaking?

A: Yes, Your ApeCoin tokens are only locked in the official ApeCoinStaking contract which has been audited also. For our pairing service, only the NFT holders and ApeCoin holders can have operating permission.

### Pairing Service Fee

#### **Q: Any charge if I use BendApeStaking service?**

A: If the NFT and ApeCoin are from the same wallet address, there is **NO** fee.

If you pair with others to join the staking, there will be a **4**% pairing service fee based on staking earnings. The management fee is decided by the on-chain voting. All the management fees go to the DAO Treasury. [Snapshot](https://snapshot.org/#/benddao.eth)

#### **Q: How does BendApeStaking charge the pairing service fee?**

A: The pairing service fee is charged at the time of staking rewards claim, and calculated based on time since the previous claim.

#### **Q: Any chance to change the pairing service fee?**

A: Yes. BendDAO is a DAO owned by the community. Anyone can propose a related proposal to adjust the setting.

### BAYC/MAYC holder

#### **Q: Do I need to take out a loan against my BAYC to use this BendApeStaking? I really just want to stake for ApeCoin not risk a loan.**

A: No, you don't need to take out a loan to join. Anyone holding Ape NFT or ApeCoin can join the BendApeStaking. NFTs need to be deposited before pairing to protect the rights and interests of ApeCoin users.

#### **Q: Do I need to find someone with ApeCoin, or will the platform connect?**

A: Your pairing listing will be displayed on BendDAO to find an ApeCoin holder to pair.

#### **Q: Why do I need to deposit my NFT to join BendApeStaking?**

A: The interest of the paired ApeCoin holders can’t be guaranteed without the NFT deposit. The ApeCoin holder will lose all staked ApeCoin and unclaimed rewards when the NFT holder sells the NFT without uncommit. [Reference](https://docs.apestake.io/#/README?id=if-i-sell-my-nft-while-it-is-committed-in-a-bayc-or-mayc-pool-will-i-lose-all-of-my-staked-apecoin)

#### **Q: How to make sure my NFT is safe with BendApeStaking?**

A: The audit report will be issued before the BendApeStaking launch. And BendDAO has been running safely for more than 7 months.

#### **Q: Can I still sell my NFT?**

A: Yes. You can list when your NFT is participating in the BendApeStaking. When you sell the NFT, the contract will uncommit and return the unclaimed rewards and ApeCoin to the deposit addresses.

#### **Q: Can I still borrow ETH?**

A: Yes. You can borrow instant ETH against your Ape NFT anytime you want.

#### **Q: I’m a borrower, can I join the BendApeStaking?**

A: Yes. You can choose to pair with other ApeCoin holders or you can join the staking with your own ApeCoin.

#### **Q: How long do I need to wait for the pairing?**

A: It depends. If you set your share ratio more attractive, your pair listing properly will be paired with the ApeCoin very soon.

#### **Q: How can I get back my NFT during the staking?**

A: Both NFT stakers and ApeCoin staker can end the staking anytime them want, but the unstaker need to pay the gas to make all the assets go back to the owners.

#### **Q: Will I miss the airdrop when I am staking?**

A: BendDAO support [flashclaim](https://docs.benddao.xyz/portal/faq/flash-claim-faq) for your NFT, but you need to uncommit first to make sure ape coin holder is safe.

### ApeCoin Holder

#### **Q: What if the paired NFT is sold during the staking?**

A: You can claim the staked ApeCoin and unclaimed rewards once the NFT is sold.

### Share Ratio

#### **Q: How to set the share ratio?**

A: The BAYC/MAYC holder who initiates the pairing listing sets the share ratio. The staking rewards will be automatically distributed by the ratio when claimed.

#### **Q: Can I change the share ratio during the staking?**

A: Yes, if the staking hasn't started yet. If the staking starts, you need to end the staking and create a new pairing listing.



