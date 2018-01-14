[Think Stats Chapter 6 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2007.html#toc60) (household income)

log_sample = InterpolateSample(income_df, log_upper=6.0)
log_cdf = thinkstats2.Cdf(log_sample)
thinkplot.Cdf(log_cdf)
thinkplot.Config(xlabel='Household income (log $)',
               ylabel='CDF')
sample = np.power(10, log_sample)
cdf = thinkstats2.Cdf(sample)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Household income ($)',
               ylabel='CDF')
Mean(sample)
Median(sample)
Skewness(sample), PearsonMedianSkewness(sample)
'''
The high skewness compared with the Pearson Median Skewness suggests that
outliers play a role in income
'''
