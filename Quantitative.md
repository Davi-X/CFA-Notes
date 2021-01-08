## Time Value of Money
### Interest 
* Time Value of Money
   * Money available at the present time is worth more than the same amount in the future due to its **potential earning capacity**
   * Cash Flow additivity principle  
        Can only be added on if thery are indexed at the **same point of time**
   * Concers **Equivalence relationships** between *cash flows* occuring on *different dates*
* Interest Rate
  * 3 applications
    * Required Rate of Return  (From the risk perspectivce)
        Minimum rate of return an investor must receive in order to accepct the investment
    * Discounted Rate  
        We discount the future amounts to find the value today
    * Opportunity cost  (From the loss choosing others, not this one'sperspective)
        The value forgo by choosing a particular course of action
  * Components
    * RF Risk-free Rate (almost exists only in theory, value is small)
    * Risk premium (风险溢价)
      * Default risk premium
      * Liquidity premium (Intution: 要买买不到, 要卖卖不掉)
      * Maturity premium (From the time perspective, e.g. cannot ensure that the investors exist in 5 years)
      * ... 
    * Nominal IR = Nominal RFIR + Risk Premium
    * Nominal RFIR $\approx$ Real RF interest rate + Inflation Rate / Premium
    * Notes: In CFA exams
      * If talking about *Real IR*, then it must includes *Real*. Otherwise, it is nominal
      * If saying that the "T-bills; US Treasury Bill; U.S. Treasury securities; Treasury bills" (美国国库券)
        Then it is *Nominal RFIR*  
      * If saying that T-bills has short/middle/long term, then in Quantitative: use **short term IR** as the RFIR 
### Effective Annual 
* Simple / Compounding IR
  * Simple  
    $Principal \times (1 + IR \times n)$
  * Compounding  
    $Principal \times (1 + IR)^n$
* Effective annual IR  
  * Simple  
    same as above
  * Discrete Compounding  
    EAR = ($1 + \frac{I/Y}{n}$)$^n - 1$
  * Continuous Compounding  (Infinite times)
    EAR = $e^{r_s} - 1$  
    1. $lim_{n \rightarrow +\infty}(1 + \frac{1}{n})^n = e$
    2. $lim_{n \rightarrow +\infty}(1 + \frac{I/Y}{n})^{\frac{n}{I/Y} \times I/Y}= e^{I/Y}$
  * Compounding frequency $n$ 
  * Periodic IR ($\frac{I/Y}{n}$)

### Future Value and Present Value
* PV: value of an initial investment (discount of FV)
* FV: value of initial investment would be worth n periods from today
  |    Compounding    |           Discount           |
  |-------------------|----------------------------- |
  | $FV = (1 + r)^n \times PV$  |  $PV = \frac{FV}{(1 + r)^n}$ |
* Annuity  
  A set of **constant** sequential cash flows
  * Ordinary Annuity (普通年金 / 后付年金)   
    occur at the **end** of each period
  * Annuity Due (先付年金)  
    occur at the **beginning** of each period
  * Ordinary Annuinty * (1 + r) = Annuity Due  
    Main diff is the **beginning of 1st year**
* Perpetuity (永续年金)  
  set of constant **never-ending** sequential cash flows occuring at the **end of each period**
* PV of PMT / Annuity:  
  What we need to invest to get the PMT / Annuity
* PV of perpetutity  
  $PV = \frac{A}{r}$
* Note: Given PMT , FV = 0 to calculate, can be understood as 
  
  "You invest PV amount of money, and withdraw PMT amount at each period, such that our FV is 0"

### Application of Calculator
Note the diretcion of cash flow
details in the `Calculator` notes

## Statistical Concepts and Market Returns
### Basic Concepts of Statistics
* Basic Concepts
  * Descriptive statistics
    How data can be **summarised effectively** to describe the important aspects
  * Inferential statistics
    Involves making **forecasts**, **estimates**, or **judgements** about a larger group from the smaller group observed
  * Population
    * All members of a specified group
    * **Parameter**: any descriptive measure of a population characteristic
  * Sample
    * A subset of a population
    * **Sample statistic**: any descriptive measure of a sample characteristic
* Measurement Scales
  * Nominal Scale
  * Ordinal Scale
  * Interval Scale
  * Ratio Scale
* Frequency Distribution
  * Absolute 
  * Cumulative Absolute
  * Relative (%)
  * Cumulative Relative
* Quantitative Description of Destribution(矩 k power)
  * Central tendency
  * Dispersion 
    How far returns are dispersed from center
  * Skewness
    Whether the distribution of returns is symmetrically shaped
  * Kurtosis (峰度)
    Whether extreme outcomes are likely or whether fatty tails exist
### Measures of Central Tendency: Means
* Arithmetic Mean
  * Population Mean
    $\mu = \frac{\sum\limits_{i=1}^NX_i}{N}$
  * Sample Mean  
    $\bar{x} = \frac{\sum\limits_{i=1}^nX_i}{n}$
  * Focus on average **single-period** performance
  * Senstitive with extreme values
* Weighted Mean 
  
  Mostly used to calculate the **portfolio return** or the **expected value** based on probabolities
* Geometric Mean
  
  $G = (X_1X_2...X_n)^{\frac{1}{n}}$
  Used to calculate **average periodic compound rate of return** on investment
  over a **multi-period** horizon

  Period Return = $((1 + R_1)(1 + R_2)...(1 + R_n))^{\frac{1}{n}} - 1$
* Harmonic Mean
  
  $\bar{X} = \frac{N}{\sum\limits_{i=1}^N\frac{1}{X_i}}$
  * Used to find the **average cost per share of stock** purchased over time in ** constant dollar amounts**
  * Cannot be used when $x_i = 0$
* Comparison
  
  Harmonic $\le$ Geometric $\le$ Arithmetic
  * When all elements equal, then these equal
  * Great variablility, more disperse of data
### Measures of Central Tendency: Median & Mode
* Median
  * Odd $\frac{n + 1}{2}$
  * Even mean of $\frac{n}{2} $ and $\frac{n + 2}{2}$
  * Pros: Not affected by outliers
  * Cons: Only consider the middle one or two, rest are ignored
* Mode
  * Most frequently occuring value
  * Could have more than one (bimodal, trimodal)
  * Useful for large data as a supplement(difficult the mean)
* Quantile (4)/ Quintiles (5)/ Deciles (10)/ Percentiles (100)
  * Used to **rank performance** and investment research
  * Location: $L = (n + 1) \cdot \frac{y}{100}$
### Measures of Dispersion
* Dispersion describes the variability around the central tendency
* Range
  
  Only use 2 limit, tell nothing else
* Mean Absolute Deviation (MAD)
  
  $\frac{\sum\limits_{i=1}^n\lvert X_i - \bar{X}\rvert}{n}$
* Variance
  
  Equals to average of the sum of squared deviations around the mean  
  * Population Variance: $\sigma^2 = \frac{\sum\limits_{i = 1}^N(X_i - \mu)^2}{N}$
  * Sample Variance: $s^2 = \frac{\sum\limits_{i = 1}^n (X_i - \bar{X})^2}{n - 1}$ (where k is the degree of freedom, here is 1, so divided by n - 1.)
* Standard Deviation
### Chebyshev's Inequality and other topics
* Chebyshev's Inequality 
  
  For any distribution with finite variance, the minimum percentage of observations that lie within k standard deviations of the mean would be $1 - \frac{1}{k^2}$, givem $k > 1$
  * Note: the variance must be finite, which is a premise
* Coefficient of Variation (CV) 
   
  A measure of **risk per unit of mean return** thus the lower is better
  $CV = \frac{s}{\mu}$
* Sharpe Ratio  
  SR = $\frac{\bar{R_p} - \bar{R_F}}{\sigma_p}$

  * $R_f$: 无风险收益率, 
  * $\bar{R_p} - R_f$: Mean excess return (超额(无风险)收益)

  A measure of **excess return per unit of risk**, thus the higher is better (only valid for positive SR)
  (一单位的风险，几单位的超额收益)
### Skewness & Kurtosis
* Skewness 
  * Indicate the **degree of symmetry** of return distributions
  * Sample skewness($S_k$) = $[\frac{n}{(n-1)(n-2)}]\frac{\sum\limits_{i=1}^n(X_i - \mu)^3}{\sigma^3}$
  * $S_k = 0$ Mean = Median = Mode 
  * Positively (Right) skewed $S_k \ge 0$ 
    * Mode < Median < Mean
    * Frequent small losses
    * A few extreme gains
  * Negatively (left) skewed $S_k \le 0$ 
    * Mean < Median < Mode 
    * A few extreme losses
    * Frequent small gains
* Kurtosis
  Degree to which the distribution is **more or less peaked than normal distribution**

  * Sample kurtosis (K) = $[\frac{n(n + 1)}{(n-1)(n-2)(n-3)}]\frac{\sum\limits_{i=1}^n(X_i - \mu)^4}{\sigma^4}$
  * Excess kurtosis: k - 3
  * Assumption: $\mu$ and $\sigma$ are equal, then we can say if k > 3, then Leptokurtic...
  (Consider the conter-example Student T-Dist)
    * Leptokurtic (高峰态)
      * More peaked, fatter tailed than Normal Dist
      * Kurtosis > 3, excess > 0
    * Mesokurtic (常峰态)
    * Platykurtic (低峰态)
      * Less peaked, thinner tailed than Normal Dist
      * Kurtosis < 3, excess < 0

