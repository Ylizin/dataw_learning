# This chapter is about elementary knowledge of statistics

## Descriptive
1. Central Tendency:   
   - mean:
      - $\mu$ : Population mean
      - $\bar{x}$ : Sample mean 
   - median(中位数)
   - mode(众数)

2. Dispersion(离心?):   
   - population variance:
     - $\sigma^{2}=\frac{\sum_{i=1}^{N}(x_i-\mu)^{2}}{N}$   
   - sample variance:   
      - $S^{2}=\frac{\sum_{i=1}^{n}(x_i-\bar{x})}{n}$   
        This formula will often underestimate the actual population variance.   

      - It turns out that the formula below is a better or called unbiased estimate of population variance  
        $S^{2}=\frac{\sum_{i=1}^{n}(x_i-\bar{x})^{2}}{n-1}$   
    - standard deviation:
      - $\sigma=\sqrt{\sigma^2}$
      - $S = \sqrt{S^2}$ 
      - the sample standard deviation is not an unbiased estimate of population
    - other ways of variance:
        $$ 
            \begin{aligned}
            \sigma^{2} &= \frac{\sum_{i=1}^{N}(x_i-\mu)^{2}}{N} \\
            \sigma^{2} &= \frac{\sum(x_i^{2}-2\mu\cdot x_i+\mu^{2})}{N} \\
            \sigma^{2} &= \frac{\sum x_i^{2}}{N}-2\mu\cdot \frac{\sum x_i}{N}+\mu^{2} \\
            \sigma^{2} &= \frac{\sum x_i^{2}}{N}-\mu^{2}    \\
            \end{aligned}
        $$   
      Samely we can generate another representation of $\sigma^2$
        $$ \begin{aligned}
            \sigma^{2} = \frac{\sum x_i^{2}}{N} - (\frac{\sum x_i}{N})^{2}
            \end{aligned}
        $$

3. Random Variable:   
   Its more of a function that maps us from the world of a random process to a number.   
   The expected value of random variable is population mean.
   - discrete :  
    The sum of all of the probabilities have to be equal to 1.
   - continuous :  
    A random variable can take on an infinite number of values and it can take on any value between an interval. So to get an exact value the probability is 0.
    - probability distribution and density function:  
      - binomial distribution:   
        $P(X=k)=C_n^{k}*p^k*(1-p)^{n-k}=b(k;n,p)$  
        $E(X) = n*p$  
        ![Binominal Distribution]('https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike80%2C5%2C5%2C80%2C26/sign=08cc6812d900baa1ae214fe92679d277/63d0f703918fa0ec9f0bc1f32e9759ee3c6ddb04.jpg' 'binominal distribution')
      - Poisson distribution:  
        $P(X=k)=\frac{\lambda^{k}}{k!}e^{-\lambda},k=0,1\cdots$  
        Poisson distribution is from binomial distribution,if the n in b-distribution is very very large and the p is small enough. We describe the $\lambda$ as $n*p$ which denote the exprectation of b-distribution  
        $$
         \begin{aligned}
            C_n^k*p^k*(1-p)^{n-k} &=\lim_{n \to \infin} \frac{n!}{(n-k)!(k!)}(\frac{\lambda}{n})^{k}(1-\frac{\lambda}{n})^{n-k}\\
            &=\lim_{n \to \infin}\frac{(n)(n-1)\cdots(n-k+1)}{n^k}(\frac{\lambda^k}{k^i})(1-\frac{\lambda}{n})^{n-k}\\
            &=\lim_{n \to \infin}\frac{n^k+\cdots}{n^k}(\cdots) \\
            &= 1*\frac{\lambda^k}{k^i}\lim_{n \to \infin}(1-\frac{\lambda}{n})^n(1-\frac{\lambda}{n})^{-k}\\
            &=\frac{\lambda^{k}}{k!}e^{-\lambda},k=0,1\cdots
           \end{aligned}
        $$
        usually $n\ge20,p\le0.05$
        


    
