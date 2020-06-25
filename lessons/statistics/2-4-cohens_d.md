[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

**Explanation:** The Cohen's d for totalwgt_lb and prglngth between first and non-first babies are both small. According to [Statistics How To](https://www.statisticshowto.com/cohens-d/), as a rule of thumb, a Cohen's d of .2 or below is a small effect and is difficult to notice with the naked eye. 

Despite both effects being small (both are below .2), the prglngth effect size is even smaller than the totalwgt_lb effect size in absolute value terms (.03 v. .09, respectively). 

**Code:**

```python
print("Cohen's d totalwgt_lb between first and non-first babies:",
      CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb))
print("Cohen's d prglngth between first and non-first babies:",
     CohenEffectSize(firsts.prglngth, others.prglngth))
```

**Code output (rounded to 2 decimal places):**  
Cohen's d totalwgt_lb between first and non-first babies: -0.09  
Cohen's d prglngth between first and non-first babies: 0.03
