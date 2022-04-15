# Vote-escrowed BEND (veBEND)

To earn the protocol income or vote on the Bend DAO, users need to stake their BEND.&#x20;

Holders of BEND can participate in voting on which NFT as collateral that Bend protocol can support for borrowing ETH and providing liquidity. It will benefit all the NFT holders as long as the supported NFT liquidity improves.

Before the mainnet launch, veBEND holders will vote for 4 of 7 bluechip NFTs that will get initial ETH lending pool support. 7 NFT collections are Mutant Ape YC, Cool Cats, Doodles, CLONE X, Azuki, World of Women and CyberKongz.

Participating in BEND DAO governance requires that an account have a balance of vote-escrowed BEND (veBEND). veBEND is a non-standard ERC20 implementation, used within the Snapshot to determine each account’s voting power.

veBEND is represented by the VotingEscrow contract, deployed to the Ethereum mainnet at: TBD.

veBEND cannot be transferred. The only way to obtain veBEND is by locking BEND. The maximum lock time is four years. One BEND locked for four years provides an initial balance of one veBEND.

A user’s veBEND balance decays linearly as the remaining time until the BEND unlock decreases. For example, a balance of 4000 BEND locked for one year provides the same amount of veBEND as 2000 BEND locked for two years, or 1000 BEND locked for four years.

The max. Lockup period is 4 years. The formula is outlined below.

MAXTIME = 4 \* 365 \* 86400\
unlock\_time < (block\_time + MAXTIME) veBEND\_amount = BEND\_locked\_amount / MAXTIME \* (unlock\_time - block\_time)



