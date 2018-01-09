[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

# Computing biased pmf
pmf = thinkstats2.Pmf(resp.numkdhh, label = 'actual')
biased_pmf = BiasPmf(pmf, label = 'observed')

# Plotting biased and unbiased pmf
biased_pmf = BiasPmf(pmf, label='observed')
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Show(xlabel='class size', ylabel='PMF')

# Calculating means
print('Unbiased mean:', round(pmf.Mean(), 2))
print('Biased mean:', round(biased_pmf.Mean()))
