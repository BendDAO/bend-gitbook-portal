# Interest Rate Model

## Rationale

Bend’s interest rate model is calibrated to manage liquidity risk and optimize utilization. The borrow interest rates come from the Utilization Rate $$U$$.

$$U$$ is an indicator of the availability of capital in the pool. The interest rate model is used to manage liquidity risk through user incentivizes to support liquidity:

* When capital is available: lower interest rates to encourage loans.
* When capital is scarce: higher interest rates encourage repayments for the loans and additional deposits.

You can read the technical details about the interest rate model [here](../risk/interest-rate-model.md).

## Interest Rate Curves

### 2022-09-07 For Ethereum Merge

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 45%             | 20%      | 16%    | 200%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-45-0908.png" alt=""><figcaption></figcaption></figure>

| Utilization Rate | Borrow Rate | Deposit Rate |
| ---------------- | ----------- | ------------ |
| 1.00%            | 20.36%      | 0.14%        |
| 5.00%            | 21.78%      | 0.76%        |
| 10.00%           | 23.56%      | 1.65%        |
| 15.00%           | 25.33%      | 2.66%        |
| 20.00%           | 27.11%      | 3.80%        |
| 25.00%           | 28.89%      | 5.06%        |
| 30.00%           | 30.67%      | 6.44%        |
| 35.00%           | 32.44%      | 7.95%        |
| 40.00%           | 34.22%      | 9.58%        |
| 45.00%           | 36.00%      | 11.34%       |
| 50.00%           | 54.18%      | 18.96%       |
| 55.00%           | 72.36%      | 27.86%       |
| 60.00%           | 90.55%      | 38.03%       |
| 65.00%           | 108.73%     | 49.47%       |
| 70.00%           | 126.91%     | 62.19%       |
| 75.00%           | 145.09%     | 76.17%       |
| 80.00%           | 163.27%     | 91.43%       |
| 85.00%           | 181.45%     | 107.96%      |
| 90.00%           | 199.64%     | 125.77%      |
| 95.00%           | 217.82%     | 144.85%      |
| 100.00%          | 236.00%     | 165.20%      |

### 2022-08-23 For Liquidity Crisis

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 80%             | 20%      | 8%     | 100%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-80-0908.png" alt=""><figcaption></figcaption></figure>

| Utilization Rate | Borrow Rate | Deposit Rate |
| ---------------- | ----------- | ------------ |
| 1.00%            | 20.10%      | 0.14%        |
| 5.00%            | 20.50%      | 0.72%        |
| 10.00%           | 21.00%      | 1.47%        |
| 15.00%           | 21.50%      | 2.26%        |
| 20.00%           | 22.00%      | 3.08%        |
| 25.00%           | 22.50%      | 3.94%        |
| 30.00%           | 23.00%      | 4.83%        |
| 35.00%           | 23.50%      | 5.76%        |
| 40.00%           | 24.00%      | 6.72%        |
| 45.00%           | 24.50%      | 7.72%        |
| 50.00%           | 25.00%      | 8.75%        |
| 55.00%           | 25.50%      | 9.82%        |
| 60.00%           | 26.00%      | 10.92%       |
| 65.00%           | 26.50%      | 12.06%       |
| 70.00%           | 27.00%      | 13.23%       |
| 75.00%           | 27.50%      | 14.44%       |
| 80.00%           | 28.00%      | 15.68%       |
| 85.00%           | 53.00%      | 31.54%       |
| 90.00%           | 78.00%      | 49.14%       |
| 95.00%           | 103.00%     | 68.50%       |
| 100.00%          | 128.00%     | 89.60%       |

### 2022-03-21 For The Begining

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 65%             | 10%      | 8%     | 100%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-65-0908.png" alt=""><figcaption></figcaption></figure>

| Utilization Rate | Borrow Rate | Deposit Rate |
| ---------------- | ----------- | ------------ |
| 1.00%            | 10.12%      | 0.07%        |
| 5.00%            | 10.62%      | 0.37%        |
| 10.00%           | 11.23%      | 0.79%        |
| 15.00%           | 11.85%      | 1.24%        |
| 20.00%           | 12.46%      | 1.74%        |
| 25.00%           | 13.08%      | 2.29%        |
| 30.00%           | 13.69%      | 2.87%        |
| 35.00%           | 14.31%      | 3.51%        |
| 40.00%           | 14.92%      | 4.18%        |
| 45.00%           | 15.54%      | 4.90%        |
| 50.00%           | 16.15%      | 5.65%        |
| 55.00%           | 16.77%      | 6.46%        |
| 60.00%           | 17.38%      | 7.30%        |
| 65.00%           | 18.00%      | 8.19%        |
| 70.00%           | 32.29%      | 15.82%       |
| 75.00%           | 46.57%      | 24.45%       |
| 80.00%           | 60.86%      | 34.08%       |
| 85.00%           | 75.14%      | 44.71%       |
| 90.00%           | 89.43%      | 56.34%       |
| 95.00%           | 103.71%     | 68.97%       |
| 100.00%          | 118.00%     | 82.60%       |
