[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

#### Cohen effect for difference in pregnancy length for first babies and others (rounded third decimal place).

```python
cohen_effect_length_firsts_others = CohenEffectSize(firsts.prglngth, others.prglngth)
print (cohen_effect_length_firsts_others)
```
Result: .029

#### Cohen effect size for difference in totalwgt_lb for first babies and others.

```python 
cohen_effect_totalwgt_lb_firsts_others = CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)
print(cohen_effect_totalwgt_lb_firsts_others)
```
Result: -.089

#### Comparing the two effect size

From the internet, I gather that Cohen suggested that a Cohen effect of 0.2 could represent a 'small' effect size meaning that there is a real effect yet could only be seen through careful study as opposed to with the naked eye. The Cohen effect size for difference in totalwgt_lb is larger between the firsts and others as opposed to the cohen effect size for pregnancy lenght, yet it is still considered to be less than a small effect, and suggests the means between the two groups (for total weight lbs.) are not enough pooled standard deviations away from each other to be statistically significant. 
