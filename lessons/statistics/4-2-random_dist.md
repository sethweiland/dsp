[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)
### Plot CDF using cumulative, step histogram. 
```python
import matplotlib.pyplot as plt

random_dist = np.random.random(size=1000)
fig,ax = plt.subplots(figsize=(8,4))
ax.hist(random_dist,cumulative=True, histtype='step',density=1)
```
![CDF plot of np.random.random(1000)](https://github.com/sethweiland/dsp/blob/master/lessons/statistics/CDF_Random_Dist_Ch4_E2.png)

```python
series_dist = pd.Series(random_dist)
pmf_rand_dist = series_dist.value_counts().sort_index() / len(series_dist)
plt.step(pmf_rand_dist.index, pmf_rand_dist.values,where='mid')
plt.xlabel("Value of Number in distribution(also from 0-1)")
plt.ylabel("PMF")
```
![PMF Plot of np.random.random(1000)](https://github.com/sethweiland/dsp/blob/master/lessons/statistics/PMF_Random_Dist_Ch4_E2.png)
