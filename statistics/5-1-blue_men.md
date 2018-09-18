[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> import scipy.stats

mu = 178
sigma = 7.7

norm_dist = scipy.stats.norm(mu, sigma)

height_low = 2.54 * 70
height_high = 2.54 * 73

(norm_dist.cdf(height_high) - norm_dist.cdf(height_low)) * 100
