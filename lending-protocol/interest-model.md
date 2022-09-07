# Interest Rate Model

Bend’s interest rate model is calibrated to manage liquidity risk and optimize utilization. The borrow interest rates come from the Utilization Rate $$U$$.

$$U$$ is an indicator of the availability of capital in the pool. The interest rate model is used to manage liquidity risk through user incentivizes to support liquidity:

* When capital is available: lower interest rates to encourage loans.
* When capital is scarce: higher interest rates encourage repayments for the loans and additional deposits.

You can read the technical details about the interest rate model [here](../risk/interest-rate-model.md).

## Interest Rate Curves

#### 2022-09-07 Ethereum Merge

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 45%             | 20%      | 16%    | 200%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-45-0907.png" alt=""><figcaption></figcaption></figure>

#### 2022-08-23

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 80%             | 20%      | 8%     | 100%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-80-0907.png" alt=""><figcaption></figcaption></figure>

#### 2022-03-21 The Begining

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 65%             | 20%      | 8%     | 100%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-65-0907.png" alt=""><figcaption></figcaption></figure>
