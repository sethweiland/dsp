[Think Stats Chapter 6 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2007.html#toc60) (household income)

```python
from scipy.stats import skew

sample_mean = sample.mean()
#answer: 74279

sample_median = np.median(sample)
#answer: 51227

sample_skew = skew(sample)
#answer: 4.95

pearsons_skew = 3*(sample_mean-sample_median)/np.std(sample)
#answer: 0.74

#Percentage of people below the mean income:
cdf.Prob(sample_mean)
#answer: 0.66
```
