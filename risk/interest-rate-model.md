# Interest Rate Model

## Overview

Bend is an NFT liquidity and lending protocol that enables borrowing ETH from the liquidity pools. Depositors receive bETH, in exchange of cryptocurrency deposits.

The liquidity of the protocol is the availability of the capital to face business operations: borrowing amounts and redeeming bTokens. It is a key metric, as lack of liquidity will block business operations.

At any point in time, the liquidity of the protocol can be assessed through the utilisation ratio: the share of reserve that is currently borrowed for each currency.

In this section, we dive into Bend's liquidity risk by analysing the historical availability of Bend's assets and identify periods of lack of liquidity. Then we look at the valuation of bTokens, illiquid assets often suffer from illiquidity discounts due to the difficulty to find counter parties.

The historical utilisation and bToken valuation help us assess the level of liquidity risk of the protocol. Once this risk is understood, we can put in place risk management techniques through the borrow interest rate model and set up alternative sources of bToken liquidity.

## Interest Rate Model

Bend’s interest rate model is calibrated to manage liquidity risk and optimize utilization. The borrow interest rates come from the Utilization Rate U.U is an indicator of the availability of capital in the pool. The interest rate model is used to manage liquidity risk through user incentivizes to support liquidity:

* When capital is available: low interest rates to encourage loans.
* When capital is scarce: high interest rates to encourage repayments for the loans and additional deposits.

## Interest Rate Model <a href="#interest-rate-model" id="interest-rate-model"></a>

Liquidity risk materializes when utilization is high, it becomes more problematic as gets closer to 100%. To tailor the model to this constraint, the interest rate curve is split into two parts around an optimal utilization rate $$U_{optimal}$$. Before $$U_{optimal}$$ the slope is small, after it starts rising sharply.

The interest rate $$R_t$$ follows the model:

$$if U < U_{optimal}: R_t = R_o + U_t / U_{optimal} * R_{slope1}$$

$$if U \ge U_{optimal}: R_t = R_o + R_{slope1} + (U_t - U_{optimal}) / (1 - U_{optimal}) * R_{slope2}$$

In the borrow rate technical implementation, the calculateCompoundedInterest method relies on an approximation that mostly affects high interest rates.

## Model Parameters

It's also key to consider market conditions: how can the asset be used in the current market Bend's borrowing costs must be aligned with market yield opportunities. Or there would be a rate arbitrage with rational users incentivized to borrow all the liquidity on Bend to take advantage of higher yield opportunities.

When market conditions change, the interest rate parameters can be adapted. These changes must adapt to utilization on Bend’s market.

Bend also adapted its cost of borrowing by lowering of the assets affected. This increased the borrow costs that are now partially offset by the liquidity reward.

Following the favorable historical review of liquidity risk, the interest rate models have been optimized to be more competitive while keeping theirs risk mitigation properties.

| Asset | Uoptimal | Ro | Rslope1 | Rslope2 |
| ----- | -------- | -- | ------- | ------- |
| ETH   | 65%      | 0  | 8%      | 100%    |

### Borrow Interest Rate Curve

![](<../.gitbook/assets/Borrow Interest Rate Model.png>)

## Deposit APY

The borrow interest rates paid are distributed as yield for bendETH holders who have deposited in the protocol, excluding a share of yields sent to the ecosystem reserve defined by the reserve factor. This interest rate is paid on the capital that is lent out then shared among all the liquidity providers.

The deposit APY, $$D_t$$, is:

$$D_t = U_t * B_t * (1-R_t)$$.

$$U_t$$: the utilisation ratio.

$$B_t$$: the variable borrow rate.

$$R_t$$: the reserve factor.

### Deposit Interest Rate Curve

![Deposit Interest Rate Model](<../.gitbook/assets/Deposit Interest Rate Model.png>)

You can view the protocol's deposit APY on the Bend App for each asset.
