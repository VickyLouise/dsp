[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

import random
rand_dist = []
for x in range(0,1000):
    r = random.random()
    rand_dist.append(r)
rank_cdf = thinkstats2.Cdf(rand_dist)
thinkplot.Cdf(rank_cdf)
thinkplot.Show(xlabel = 'percentile rank', ylabel = 'CDF')
