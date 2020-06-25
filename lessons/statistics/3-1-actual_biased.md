[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```python
resp = nsfg.ReadFemResp()
numkdhh_pmf_actual = thinkstats2.Pmf(resp.numkdhh, label='actual')
numkdhh_pmf_biased = BiasPmf(numkdhh_pmf_actual, label='observed')
thinkplot.PrePlot(2)
thinkplot.Pmfs([numkdhh_pmf_actual, numkdhh_pmf_biased])
thinkplot.Config(xlabel='number of children under 18 in household', ylabel='PMF')

print('numkdhh actual mean:', numkdhh_pmf_actual.Mean())
print('numkdhh observed mean:', numkdhh_pmf_biased.Mean())
print('Difference:', numkdhh_pmf_actual.Mean() - numkdhh_pmf_biased.Mean())
```

**Code output:**  
numkdhh actual mean: 1.024205155043831  
numkdhh observed mean: 2.403679100664282  
Difference: -1.3794739456204512  
