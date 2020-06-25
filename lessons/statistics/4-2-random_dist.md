[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

**Explanation:** Yes, the numpy.random.random distribution is uniform as can be seen by the straight line given by the plotted CDF.  

```python
random_1000 = np.random.random(1000)
random_1000_pmf = thinkstats2.Pmf(random_1000, label='random')
thinkplot.Pmf(random_1000_pmf, linewidth=0.1)
thinkplot.Config(xlabel='Random Number', ylabel='PMF')
```
![Random_Number_PMF](https://user-images.githubusercontent.com/62628676/85786809-9cfa1080-b6f8-11ea-9cd7-7ee694a5cdf8.png)  
```python
random_1000_cdf = thinkstats2.Cdf(random_1000, label='random')
thinkplot.Cdf(random_1000_cdf)
thinkplot.Config(xlabel='Random Number', ylabel='CDF')
```
![Random_Number_CDF](https://user-images.githubusercontent.com/62628676/85786878-af744a00-b6f8-11ea-9484-81ffc0133611.png)  
