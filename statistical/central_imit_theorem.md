# Central limit theorem
It tells us we could start off with **any** distribution that has a well-defined **mean** and **variance** or some **others statistics** like mode or range. And it can be continuous or discrete. If we take n-samples from that distribution and repeat this action enough times, the distribution of n-samples' mean or sum approaches the normal distribution(which means the x-axe is the value of 'n-mean' and y is the 'frequency'). **As n get larger, it approximates better**.  

1. Skewness(偏度) and kurtosis(峰度):  
   
   ![Skewness](https://gss0.bdstatic.com/94o3dSag_xI4khGkpoWK1HF6hhy/baike/s%3D220/sign=792a3548c65c1038207ec9c08210931c/cf1b9d16fdfaaf5163a4b4ed8c5494eef01f7a18.jpg)  
   [Here is a brief introduction of S and K](https://www.cnblogs.com/jiaxin359/p/8977333.html 'here ')  

2. Samples mean and variance:  
   $\mu_{\bar{x}}=\mu$  
   $\sigma_{\bar{x}}=\frac{\sigma^2}{n}$  
   here when the $\sigma^2$ is not easy to get we can use $S^2=\sigma^2$ where $S^2 =\frac{SUM}{N-1}$

3. Bernoulli Distribution:  
   It's the simplest case of the binomial distribution.  
   $\mu=p$  
   $\sigma^2=p(1-p)$  

4. Confidence interval:  
   $P(\bar{x}$ is within $2\sigma_{\bar{x}}$ of $\mu_{\bar{x}})=0.95$  
   that means, if we take n samples and the mean $\bar{x}$ is near the $\mu_{\bar{x}}$ within 2$\sigma_{\bar{x}}$, then it means that the sample mean $\bar{x}$ is within interval $(\mu_{\bar{x}}-2\sigma_{\bar{x}},\mu_{\bar{x}}+2\sigma_{\bar{x}})$ and what matters is that the at the same time it means $\mu_{\bar{x}}=\mu$ is in $(\bar{x}\pm2\sigma_{\bar{x}})$ with the probability of 0.95. So if we take a sample with n=100 and the mean is $\bar{x}$, remember no matter when, the $P(\bar{x}$ is within $2\sigma_{\bar{x}}$ of $\mu_{\bar{x}})=0.95$ right, then the $\mu_{\bar{x}}=\mu$ is at the possibility of 0.95 in $(\bar{x}\pm2\sigma_{\bar{x}})$. Through that, we could calculate the unknow mean of the population.
   

   