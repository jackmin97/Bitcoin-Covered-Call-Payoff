# Bitcoin-Covered-Call-Payoff
In this notebook, we will build a payoff graph for covered call by using the payoff graph of long 17500 Bitcoin spot and short 17500 strike call on Bitcoin. A covered call strategy is built by going long on a underlying asset and simultaneously selling a call option on that asset. The strategy is used when the view on the underlying asset is neutral. 

### 1. Import libraries
First, we will import the necessary libraries

### 2. Call payoff
We define a function that calculates the payoff from buying a call option. The function takes St which is a range of possible values of the Bitcoin price at expiration, the strike price of the call and premium of the call option as input. It returns the call option payoff.

### 3. Define the parameters
We define various parameters required to calculate the call payoff. One of the parameters is the range of Bitcoin price at expiry. To calculate the Bitcoin price range at the call's expiration, we define a range for the Bitcoin price at expiry from -10% to +10% from the spot price. That is from 90% or 0.90 to 110% or 1.10 from the spot price. These range values are for illustration purposes and can be changed.

### 4. Long 17500 Bitcoin spot payoff
We plot the payoff of the long 17500 Bitcoin spot. 

### 5. Short 17500 strike call payoff
We plot the payoff of the short 17500 strike call option.

### 6. Covered call payoff
The max profit is capped at USD 500 if Bitcoin moves to any price above USD 17500 and the max loss is proportional to price fall below USD 17500.
