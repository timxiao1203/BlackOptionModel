# BlackOptionModel

Black’s vanilla option pricing model can be applied to a wide range of vanilla European options such as caps/floors, European swaptions, bond options, bond futures options and interest rate (IR) futures options.

Black’s option pricing model, which is in a closed-form formula, can be applied to vanilla European type options under the Black-Scholes framework. Black’s option pricing formula has been widely applied in fixed income derivative market for years. A vanilla European call option can be defined by its payoff at maturity where X is an underlying rate, T is the payoff reset time and K is the strike price. Accordingly, the payoff for a vanilla European put option is

The matured payoffs is paid at a settlement time T' which is greater than or equal to T . Under the Black-Scholes framework, the key assumption is that, in the risk-neutral measure with respect to the zero bond price matured at T' , T is log-normally distributed with a single parameter X σ , the volatility of the underlying rate X .

Black’s vanilla option pricing model can be applied to pricing a variety of instruments including caps/floors, European swaptions, bond options, bond futures options and IR futures options. In the case of caps/floors and European swaptions1, X is the forward term rate and forward swap rate, respectively. For European bond options, the rate X represents the bond price (see https://finpricing.com/lib/FiBond.html). For European bond futures options and European IR futures options, X stands for bond futures price and Euro-Dollar futures price, respectively.

In the Black’s model, the fair price for the vanilla European call option as above is computed where F0 is a current expectation of the underlying rate X at maturity, r is the risk-free interest rate, N(⋅) denotes the cumulative distribution function (cdf) for a standard normal random variable and

A bond put option with the same specifications has a fair value. Based on the above closed-form results, one can easily determine the various risk numbers associated with this instrument. For a call option, the risk numbers are calculated where n(⋅) denotes the probability density function (pdf) for a standard normal random variable, i.e.,

Similarly, risk numbers for a put option are computed, i.e., Gamma and Vega are identical in both cases. Principal adjustment is necessary if dealing with caps/floors and swaptions.

The current expectation of an underlying rate at maturity must be known. It may be a current forward term rate, a current forward swap rate, a current forward price or a current futures price, depending upon cases. The volatility of the underlying rate must be provided. Usually, it can be interpolated from a given set of market implied volatilities.


