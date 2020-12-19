## Memory
* TVM (Time Value of Money)
* CF (Cash Flow)

## Setting up decimal places
1. 2nd -> . (Format mode)
2. [number e.g. 4 / 6 / 9] -> **ENTER**
3. 2nd -> CPT (Quit mode)

## Setting up the algo
* CHN (Chain)
  According to the numbers key in orderly  
  e.g. 2 + 5 x 4 = 28
* AOS (Algebraic Operating Mode)
  According to maths algo  
  e.g. 2 + 5 x 4 = 22
* Chaning
  1. 2nd -> . (Format Mode)
  2. up/down arrow to find 'CHN' or 'AOS'
  3. 2nd -> ENTER (Set mode)

## Setting up BGN / END mode
Cash flow 
* BEG 
* END
* Chaning 
  1. 2nd -> PMT(payment) (Check current)
  2. 2nd -> ENTER (Set Mode)

## Store into / Recall from / Check memory
* Store  
  number -> STO -> index(0 up to 9) 
* Recall  
  number -> RCL -> index
* Check / Store  
  1. 2nd -> 0 (Memory mode)  
  2. number -> set (Assign value / Store into specify memory block)

## Time Value of Money
* N  
  \# compounding periods
* I/Y  
  Periodic Rate (Default annuly)
* PV  
  Present Value
* PMT  
  Periodic Payments
* FV  
  Future Value

* Time Line
PV -> Each epriod additional PMT + interest -> ... (N times) -> FV

Note: Cash flow has direction, so we have +/-
input has different direction then FV/PV(given) 
(input usually is negative, output is positive)

Order of entering do not matter

END       PMT        PMT        PMT        PMT
/-------------------------------------------/
|    Y1    |    Y2    |    Y3    |    Y4    |
/-------------------------------------------/
BGN PMT   PMT        PMT        PMT        

* For unequal PMT each period, using CF(cash flow)
* NPV (net present value)
  if CF0 = 0:
    NPV == Pv is true
* Discount Rate (I/Y)
  * PV = total
  * FV = 0

## Capital Budgeting
* NPV same as above
  1. CF (series)
  2. NPV -> CPT
* IRR (Inside Rate of Return)
  Intution: Find the I/Y to let NPV = 0
  1. CF (series)
  2. IRR -> CPT

## Statistics
* Input Data  
  2nd -> 7 (Data mode)
  * X: data
  * Y: prob. / 2nd Series of data
* Stat Mode  
  1. 2nd -> 8
  2. 2nd -> ENTER 
  * Modes
    * LIN (Linear Regression)
    * Ln (Log n)
    * EXP 
    * PWR
    * 1-V (One variable)
  * Values
    * Mean
    * Sample sd : $S_X$
    * Population sd : $\sigma_X$
    * sample of Correlation Coefficient: r
    * Cov(x,y)  
      compute manually: $r * S_x * S_y$

## Probabilities
* Factorial  
   [n][2nd][x]
* Combination (nCr) $\binom{n}{r}$  
   [n][2nd][+][r]
* Permutation (nPr) $^nP_k$
   [n][2nd][-][r]