# Interest Rate Model

## Rationale

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

| Utilization Rate | Borrow Rate | Deposit Rate |
| ---------------- | ----------- | ------------ |
| 0.01             | 0.2036      | 0.0014       |
| 0.05             | 0.2178      | 0.0076       |
| 0.10             | 0.2356      | 0.0165       |
| 0.15             | 0.2533      | 0.0266       |
| 0.20             | 0.2711      | 0.0380       |
| 0.25             | 0.2889      | 0.0506       |
| 0.30             | 0.3067      | 0.0644       |
| 0.35             | 0.3244      | 0.0795       |
| 0.40             | 0.3422      | 0.0958       |
| 0.45             | 0.3600      | 0.1134       |
| 0.50             | 0.5418      | 0.1896       |
| 0.55             | 0.7236      | 0.2786       |
| 0.60             | 0.9055      | 0.3803       |
| 0.65             | 1.0873      | 0.4947       |
| 0.70             | 1.2691      | 0.6219       |
| 0.75             | 1.4509      | 0.7617       |
| 0.80             | 1.6327      | 0.9143       |
| 0.85             | 1.8145      | 1.0796       |
| 0.90             | 1.9964      | 1.2577       |
| 0.95             | 2.1782      | 1.4485       |
| 1.00             | 2.3600      | 1.6520       |

#### 2022-08-23 Liquidity Crisis

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 80%             | 20%      | 8%     | 100%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-80-0907.png" alt=""><figcaption></figcaption></figure>

| Utilization Rate | Borrow Rate | Deposit Rate |
| ---------------- | ----------- | ------------ |
| 0.01             | 0.2010      | 0.0014       |
| 0.05             | 0.2050      | 0.0072       |
| 0.10             | 0.2100      | 0.0147       |
| 0.15             | 0.2150      | 0.0226       |
| 0.20             | 0.2200      | 0.0308       |
| 0.25             | 0.2250      | 0.0394       |
| 0.30             | 0.2300      | 0.0483       |
| 0.35             | 0.2350      | 0.0576       |
| 0.40             | 0.2400      | 0.0672       |
| 0.45             | 0.2450      | 0.0772       |
| 0.50             | 0.2500      | 0.0875       |
| 0.55             | 0.2550      | 0.0982       |
| 0.60             | 0.2600      | 0.1092       |
| 0.65             | 0.2650      | 0.1206       |
| 0.70             | 0.2700      | 0.1323       |
| 0.75             | 0.2750      | 0.1444       |
| 0.80             | 0.2800      | 0.1568       |
| 0.85             | 0.5300      | 0.3154       |
| 0.90             | 0.7800      | 0.4914       |
| 0.95             | 1.0300      | 0.6850       |
| 1.00             | 1.2800      | 0.8960       |

#### 2022-03-21 The Begining

| UtilizationRate | BaseRate | Slope1 | Slope2 |
| --------------- | -------- | ------ | ------ |
| 65%             | 10%      | 8%     | 100%   |

<figure><img src="../.gitbook/assets/Borrow Rate and Deposit Rate-65-0907.png" alt=""><figcaption></figcaption></figure>

| Utilization Rate | Borrow Rate | Deposit Rate |
| ---------------- | ----------- | ------------ |
| 0.01             | 0.1012      | 0.0007       |
| 0.05             | 0.1062      | 0.0037       |
| 0.10             | 0.1123      | 0.0079       |
| 0.15             | 0.1185      | 0.0124       |
| 0.20             | 0.1246      | 0.0174       |
| 0.25             | 0.1308      | 0.0229       |
| 0.30             | 0.1369      | 0.0287       |
| 0.35             | 0.1431      | 0.0351       |
| 0.40             | 0.1492      | 0.0418       |
| 0.45             | 0.1554      | 0.0490       |
| 0.50             | 0.1615      | 0.0565       |
| 0.55             | 0.1677      | 0.0646       |
| 0.60             | 0.1738      | 0.0730       |
| 0.65             | 0.1800      | 0.0819       |
| 0.70             | 0.3229      | 0.1582       |
| 0.75             | 0.4657      | 0.2445       |
| 0.80             | 0.6086      | 0.3408       |
| 0.85             | 0.7514      | 0.4471       |
| 0.90             | 0.8943      | 0.5634       |
| 0.95             | 1.0371      | 0.6897       |
| 1.00             | 1.1800      | 0.8260       |
