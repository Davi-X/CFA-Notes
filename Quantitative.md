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