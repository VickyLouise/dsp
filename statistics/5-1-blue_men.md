[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)
dist.mean(), dist.std()
dist.cdf(mu-sigma)
high = dist.cdf(189)
low = dist.cdf(181)
high - low
