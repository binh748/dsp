[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```python
import scipy.stats

# mu = mean, sigma = standard deviation
mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)

def convert_ft_to_cm(height_ft):
    height_cm = height_ft * 30.48
    return height_cm

height1_cm = convert_ft_to_cm(5+10/12)
height2_cm = convert_ft_to_cm(6+1/12)

dist.cdf(height2_cm) - dist.cdf(height1_cm)
```
**Answer:** 34.3% of the U.S. male population is between 5'10" and 6'1", which is the range of heights a man is required to meet to join the Blue Man Group.  
