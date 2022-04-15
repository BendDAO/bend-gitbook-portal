# Fee Collection and Distribution

Bend lending pool contracts have the capability to charge an “admin fee”, that is Bend protocol income, 100% claimable by the veBEND holders proportionally. The admin fee is represented as a 30% of the total interest income collected on NFT loans.&#x20;

For borrowing the fee is taken in the borrowed currency and calculated against the final amount received. For example, if borrowing ETH using NFTs as collateral, the fee is taken in **ETH**.

### VeBEND holder income estimation

The first column is the estimated Bend loan volume in ETH.

The second column is the estimated protocol annual fee. It is assumed that 30% of the ETH in the pool is lent out, the borrowing interest rate is 15%, and the protocol "admin fee" is 30%. &#x20;

The third column is the estimated APR in ETH for veBEND holders.&#x20;

![ Estimated earnings for veBEND holders](<../.gitbook/assets/image (3).png>)

All fees are distributed to **veBEND holders** by week. The proportional amount of fees that each user is to receive is calculated based on their veBEND balance relative to the total veBEND supply.&#x20;

This amount is calculated at the _start_ of the week. The actual distribution occurs at the _end_ of the week based on the fees that were collected. As such, a user that creates a new vote-lock should expect to receive their first fee payout at the end of the following epoch week.

The available BWETH balance to distribute is tracked via the “token distribute checkpoint”. This is updated at a minimum every 24 hours. Fees that are received between the last checkpoint of the previous week and first checkpoint of the new week will be split evenly between the weeks.

![](<../.gitbook/assets/image (8).png>)



