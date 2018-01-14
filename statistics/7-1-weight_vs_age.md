[Think Stats Chapter 7 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2008.html#toc70) (weight vs. age)

# Scatterplot
thinkplot.Scatter(live.agepreg, live.totalwgt_lb, alpha=1, s=10)
thinkplot.Config(xlabel='Age (years)',
                 ylabel='Baby Weight (lb)',
                 legend=False)
# Pearson's correlation
Corr(live.agepreg, live.totalwgt_lb)
np.corrcoef(live.agepreg, live.totalwgt_lb)
# This suggests a very weak relationship between age of the mother
# and weight of the baby
# SpearmanCorr
SpearmanCorr(live.agepreg, live.totalwgt_lb)
# The Spearman Correlation suggests a slightly stronger relationship than 
# the Pearson's. Looking at the scatter plot, this is most likely due to
# outliers rather than a non-linear relationship.
