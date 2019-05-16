# Linear regression
$$ \begin{aligned}
    y &= mx+b \\
    SE_{line} &= \sum_0^{n}(y_i-(mx_i+b))^2 \\
    &= \sum_0^n(y_i)^2 +(-2m)\sum_{0}^n(x_iy_i) + (-2b)\sum(y_i)+(m^2)\sum(x_i)^2+2mb\sum(x_i)+nb^2 \\
    &=n\bar{y}^2-2mn\bar{xy}-2bn\bar{y}+m^2n\bar{x^2}+2mbn\bar{x}+nb^2
\end{aligned}$$  
So if we want to minimize the $SE_{line}$ then $\frac{\partial{SE}}{\partial{m}}=0$ and $\frac{\partial {SE}}{\partial{b}}=0$

Then :  
$$\begin{aligned}
    -2n\bar{xy}+2n\bar{x^2}m+2bn\bar{x} &= 0\\
    -2n\bar{y} + 2mn\bar{x} + 2bn &= 0 \\

\end{aligned}
$$

it can be solved as:  
$$
m=\frac{\bar{x}\bar{y}-\bar{xy}}{\bar{x}^2-\bar{x^2}}\\
b = \bar{y}-m\bar{x}
$$
  


## coefficient of determination(决定系数)$R^2$
$SE_{line} = \sum(y_i-\hat{y_i})$  
$SE_{\bar{y}}=\sum(y_i-\bar{y})$  
$R^2 = 1- \frac{SE_{line}}{SE_{\bar{y}}}$

$R^2$ smaller the better your line fit the data.


## covariance
$Cov(x,y)=E[(X-E(X))(Y-E(Y))]=E(XY)-E(Y)E(X)=\bar{xy}-\bar{y}\bar{x}$  
$Cov(x,x)=\bar{x^2}-\bar{x}^2=Variance(x)$  
So the slope(斜率) of the regression line can be write as $\frac{Cov(x,y)}{Var(x)}$

## Chi-squared distribution
Assume we have some independent random variables from normal distribution. For example, $X\sim N(0,1) E(X)=0,Var(X)=1$  
Then assume we have the result of the sample $Q=x^2$, the distribution of $Q$ is one degree of freedom chi-suqared distribution.$Q_2 = x_1^2+x_2^2$ remember that $x_1,x_2$ is independently sampled from normal distribution. $Q_n \sim \chi_n^2$ n means the degree of freedom.  
![chi suqred distribution](https://gss0.bdstatic.com/-4o3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike116%2C5%2C5%2C116%2C38/sign=79a65832b0fb43160e12722841cd2d46/6159252dd42a283470500ef259b5c9ea14cebf50.jpg)
the x axis means the result of n samples' squared sum.  
Chi squared distribution can be applied in some hypothesis tests.  
For example, if we have n samples, and n given corresponding data, ~~so we assume the difference between our sample data and the given data is normal distributed~~.  
So:  ($\sum \limits_1^n\frac{(y_{given}-y_{sample})^2}{y_{sample}})$ then calculate the probability according to the $n-1$ degrees of freedom $\chi^2$ distribution. 

## SST(Sum of Squares Total):  
the numerator of the variance, remember we can always calculate the last point from the previous n-1 number and the mean so the degree of freedom is always mn-1.

1. SSW(Sum of squares within group):  
   calculate every groups' square dist and sum them 
   and its' degree of freedom is m(n-1)
2. SSB(****bwtween group):  
   calculate the mean of each group and then calculate the $(\bar{group}-\bar{total})^2*elemnetInThisGroup$ and its degree of freedom is m-1 ,where n is element of each group m is the number of goups.  

The $SST = SSB+SSW$ and degree of freedom $totalfree = SSBFree+SSWFree$

 F-statistics:  $\frac{SSB\div(m-1)}{SSW\div(mn-m)}$  
 this means two different chi-squared distribution with ***m-1 and mn-m degree of freedom***.
 ![F-distribution](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1557996017080&di=57300b2d1ae31ab9ed0d6524ba96dba6&imgtype=0&src=http%3A%2F%2Fgss0.baidu.com%2F-4o3dSag_xI4khGko9WTAnF6hhy%2Fzhidao%2Fpic%2Fitem%2F29381f30e924b8997501765468061d950a7bf699.jpg)  
 in the image above, the n1 is the numerator's degree and the n2 is the denominator's degree,and compare the result of F-statistics and the value you get, the larger F is, the smaller the probability you will get.
    

