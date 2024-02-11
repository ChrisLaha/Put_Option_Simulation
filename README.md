# Put Option Simulation
* If you own a stock, buying a put option on the stock will greatly reduce your risk. This is the idea behind portfolio insurance. To illustrate, consider a stock that currently sells for $56 and has an annual volatility of 30%. Assume the risk-free rate is 8%, and you estimate that the stock’s annual growth rate is 12%.

* Suppose you own 100 shares of this stock. Use simulation to estimate the probability distribution of the percentage return earned on this stock during a one-year period.
  
* Now suppose you also buy a put option for $238 on the stock. The option has an exercise price of $50 and an exercise date one year from now. Use simulation to estimate the probability distribution of the percentage return on your portfolio over a one-year period. Can you see why this strategy is called a portfolio insurance strategy?

* Use simulation to show that the put option should, indeed, sell for about $238.

1. Simulate the stock price after one year to estimate the distribution of percentage return on the stock.
2. Incorporate the put option into the simulation to see how it affects the distribution of returns.
3. Estimate the fair price of the put option using simulation.

4. First, let's define some variables based on the given information:

- Initial stock price $S_0 = \$56$
- Annual volatility $\sigma = 30\%$
- Risk-free rate $r = 8\%$
- Stock’s annual growth rate $\mu = 12\%$
- Number of shares $N = 100$
- Put option exercise price $K = \$50$
- Option cost $C_{\text{option}} = \$238$

We'll simulate the stock price after one year using the geometric Brownian motion model, which is a common model for stock price dynamics. The formula for a future stock price after time $t$ is:

$$S_t = S_0 e^{(\mu - \frac{1}{2} \sigma^2)t + \sigma \sqrt{t} Z}$$

where $Z$ is a random variable from the standard normal distribution.
