# Fee Collection and Distribution

Bend lending pool contracts have the capability to charge an “admin fee”, that is Bend protocol income, 100% claimable by the veBEND holders proportionally. The admin fee is represented as a 30% of the total interest income collected on NFT loans.&#x20;

For borrowing the fee is taken in the borrowed currency and calculated against the final amount received. For example, if borrowing ETH using NFTs as collateral, the fee is taken in **ETH**.

### VeBEND holder income estimation

The first column is the estimated Bend loan volume in ETH.

The second column is the estimated protocol annual fee. It is assumed that 30% of the ETH in the pool is lent out, the borrowing interest rate is 15%, and the protocol "admin fee" is 30%. &#x20;

The third column is the estimated APR in ETH for veBEND holders.&#x20;

![ Estimated earnings for veBEND holders](<../.gitbook/assets/image (3).png>)

All fees are distributed to **veBEND holders** by week. The proportional amount of fees that each user is to receive is calculated based on their veBEND balance relative to the total veBEND supply.&#x20;

This amount is calculated at the _start_ of the week. The actual distribution occurs at the _end_ of the week based on the fees that were collected. As such, **users who create a new voting lock will have no fee income for the current epoch week and should expect to receive their first fee payment at the end of the next epoch week**.

It should be noted that the week here is not the ISO_8601 standard week, but epoch week based on unix timestamp , so the first day of the week is not Monday, for more details please refer to Wikipedia [unix time](https://en.wikipedia.org/wiki/Unix_time) , [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)

Example:\
Suppose user lock bend at the current time Mon Apr 18 2022 06:40:39 GMT+0000\
Then the timestamp is 1650264039\
Current epoch week = 1650264039/604800(seconds of one week) = 2728.6111756\
So the current epoch week 2728 starts at Thu Apr 14 2022 00:00:00 GMT+0000, and ends at Thu Apr 21 2022 00:00:00 GMT+0000\
And next week 2729 will end on Thu Apr 28 2022 00:00:00 GMT+0000, when the user first fee will be received

The available BWETH balance to distribute is tracked via the “token distribute checkpoint”. This is updated at a minimum every 24 hours. Fees that are received between the last checkpoint of the previous week and first checkpoint of the new week will be split evenly between the weeks.





