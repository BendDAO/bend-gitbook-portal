# Interest Model

Bend’s interest rate model is calibrated to manage liquidity risk and optimize utilization. The borrow interest rates come from the Utilization Rate $$U$$.

$$U$$ is an indicator of the availability of capital in the pool. The interest rate model is used to manage liquidity risk through user incentivizes to support liquidity:

* When capital is available: low interest rates to encourage loans.
* When capital is scarce: high interest rates to encourage repayments for the loans and additional deposits.

## Borrow Interest Rate Curve

![](<../.gitbook/assets/Borrow Interest Rate Model.png>)

## Deposit Interest Rate Curve

![](<../.gitbook/assets/Deposit Interest Rate Model.png>)

## Interest Rate Models

We have listed three different sets of base interest rate models, and the final interest rate model will be decided by the community through voting.

### Base Interet Rate 3%

| Utilization Rate(%) | Borrow Rate(%) | Deposit Rate(%) |
| ------------------- | -------------- | --------------- |
| 1                   | 3.12           | 0.02            |
| 5                   | 3.62           | 0.13            |
| 10                  | 4.23           | 0.3             |
| 15                  | 4.85           | 0.51            |
| 20                  | 5.46           | 0.76            |
| 25                  | 6.08           | 1.06            |
| 30                  | 6.69           | 1.4             |
| 35                  | 7.31           | 1.79            |
| 40                  | 7.92           | 2.22            |
| 45                  | 8.54           | 2.69            |
| 50                  | 9.15           | 3.2             |
| 55                  | 9.77           | 3.76            |
| 60                  | 10.38          | 4.36            |
| 65                  | 11             | 5.01            |
| 70                  | 25.29          | 12.39           |
| 75                  | 39.57          | 20.77           |
| 80                  | 53.86          | 30.16           |
| 85                  | 68.14          | 40.54           |
| 90                  | 82.43          | 51.93           |
| 95                  | 96.71          | 64.31           |
| 100                 | 111            | 77.7            |

### Base Interest Rate 5%

| Utilization Rate(%) | Borrow Rate(%) | Deposit Rate(%) |
| ------------------- | -------------- | --------------- |
| 1                   | 5.12           | 0.04            |
| 5                   | 5.62           | 0.2             |
| 10                  | 6.23           | 0.44            |
| 15                  | 6.85           | 0.72            |
| 20                  | 7.46           | 1.04            |
| 25                  | 8.08           | 1.41            |
| 30                  | 8.69           | 1.82            |
| 35                  | 9.31           | 2.28            |
| 40                  | 9.92           | 2.78            |
| 45                  | 10.54          | 3.32            |
| 50                  | 11.15          | 3.9             |
| 55                  | 11.77          | 4.53            |
| 60                  | 12.38          | 5.2             |
| 65                  | 13             | 5.92            |
| 70                  | 27.29          | 13.37           |
| 75                  | 41.57          | 21.82           |
| 80                  | 55.86          | 31.28           |
| 85                  | 70.14          | 41.73           |
| 90                  | 84.43          | 53.19           |
| 95                  | 98.71          | 65.64           |
| 100                 | 113            | 79.1            |

### Base Interest Rate 10%

| Utilization Rate(%) | Borrow Rate(%) | Deposit Rate(%) |
| ------------------- | -------------- | --------------- |
| 1                   | 10.12          | 0.07            |
| 5                   | 10.62          | 0.37            |
| 10                  | 11.23          | 0.79            |
| 15                  | 11.85          | 1.24            |
| 20                  | 12.46          | 1.74            |
| 25                  | 13.08          | 2.29            |
| 30                  | 13.69          | 2.87            |
| 35                  | 14.31          | 3.51            |
| 40                  | 14.92          | 4.18            |
| 45                  | 15.54          | 4.9             |
| 50                  | 16.15          | 5.65            |
| 55                  | 16.77          | 6.46            |
| 60                  | 17.38          | 7.3             |
| 65                  | 18             | 8.19            |
| 70                  | 32.29          | 15.82           |
| 75                  | 46.57          | 24.45           |
| 80                  | 60.86          | 34.08           |
| 85                  | 75.14          | 44.71           |
| 90                  | 89.43          | 56.34           |
| 95                  | 103.71         | 68.97           |
| 100                 | 118            | 82.6            |

### Base Interest Rate 20%

| Utilization Rate | Borrow Rate(%) | Deposit Rate(%) |
| ---------------- | -------------- | --------------- |
| 1                | 20.12307692    | 0.1408615385    |
| 5                | 20.61538462    | 0.7215384615    |
| 10               | 21.23076923    | 1.486153846     |
| 15               | 21.84615385    | 2.293846154     |
| 20               | 22.46153846    | 3.144615385     |
| 25               | 23.07692308    | 4.038461538     |
| 30               | 23.69230769    | 4.975384615     |
| 35               | 24.30769231    | 5.955384615     |
| 40               | 24.92307692    | 6.978461538     |
| 45               | 25.53846154    | 8.044615385     |
| 50               | 26.15384615    | 9.153846154     |
| 55               | 26.76923077    | 10.30615385     |
| 60               | 27.38461538    | 11.50153846     |
| 65               | 28             | 12.74           |
| 70               | 34.36571429    | 16.8392         |
| 75               | 48.65142857    | 25.542          |
| 80               | 62.93714286    | 35.2448         |
| 85               | 77.22285714    | 45.9476         |
| 90               | 91.50857143    | 57.6504         |
| 95               | 105.7942857    | 70.3532         |
| 100              | 120.08         | 84.056          |
