# Derman_Approximation_on_QNM

In this project, our aim is to assess the performance of Derman's approximation for implied normal volatility within the quadratic normal local volatility framework. 
Interestingly, our findings reveal that Derman's approximation yields suboptimal results due to its failure to account for the impact of time-to-maturity. 
In particular, when we analyze the quadratic normal model with the current underlying price aligned with the vertex (the minimum point) of the parabolic curve, we anticipate that implied normal volatility should increase as the time to maturity extends.
The reasoning behind this expectation is rooted in the fact that over longer time periods, the underlying price is more likely to experience outward movements, accumulating higher levels of local volatility. 
However, Derman's approximation always provides the vertex value as the implied normal volatility, irrespective of the time to maturity.

To overcome this limitation, we have devised an improved version of Derman's approximation by introducing an additional term that accounts for the influence of time to maturity. 
This refined approximation can be derived with ease using the quadratic normal formula and Taylor expansion techniques. 
Our revised approximation has proven to be highly effective, as demonstrated in the plot below.
![performance](https://github.com/WuYenSun/Derman_Approximation_on_QNM/blob/main/derman00.png)

Moreover, our methodology enables a streamlined calibration process for the quadratic normal model, focusing on an analysis of key implied volatility metrics such as the vertex value, skewness, and kurtosis. 
This specific aspect will be explored in detail in our upcoming research.




