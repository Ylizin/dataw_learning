# Hypothesis test

1. null hypothesis:  
   experiment has no effect$\to$the distribution of the experiment is the same as before$\to$calculate that the probability of experiment's result in the previous distribution.  
2. alternative hypothesis:  
3. two-tailed test:  
   no matter the result is better than before or bad  
   contrast to the one-tailed test.

Assume $H_{0}$ is the null hypothesis  
First we assue the null hypothesis is true, calculate the $\bar{x},\sigma_{\bar{x}}$ of the samples distribution through the samples' amount, then according to the 'assume', the distribution should be very the same as before, so calculate the probability that $H_{0}$ is true. If the $p$ is smaller than the threshold we consider that the $H_{0}$ is wrong and take $H_{1}$ .

$E(z) = E(X+Y)= E(X)+E(Y)$  
$Var(X\pm Y)= Var(X) + Var(Y)$ since the var take the square

then:  
$\mu_{\bar{X}-\bar{Y}}=\mu_{\bar{X}}-\mu_{\bar{Y}}$  
$\sigma_{\bar{X}-\bar{Y}} = \sqrt{\frac{\sigma_{x}^2}{n}+\frac{\sigma_Y^2}{m}}$  
**remeber usually we estimate the 'true' $\mu$ through samples' mean $\bar{x}$ as well as the $\sigma^2$ by $S^2$**
**and notice if we do a hypothesis all of the variance and mean should be reconsidered in the hypothesis situation.[video for explanation](http://open.163.com/movie/2011/6/V/F/M82IC6GQU_M83JD0RVF.html) and [for confidential interval](http://open.163.com/movie/2011/6/G/I/M82IC6GQU_M83JD9CGI.html),these cases can also reveal the difference between hypothesis test and confidential interval.**   
This can be applied in questions that calculate the difference between two distributions' change become larger or not. Or if you have already sampled two distribution then get the difference of the mean of two sample $\bar{x}-\bar{y}$ and you want to make sure that if in $H_{0}$ how large is the probability this situation happens.

