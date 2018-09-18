[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> import thinkstats2
import thinkplot
import nsfg

def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)

    for x, p in pmf.Items():
        new_pmf.Mult(x, x)
        
    new_pmf.Normalize()
    return new_pmf

resp = nsfg.ReadFemResp()
actual = resp['numkdhh']
pmf = thinkstats2.Pmf(actual, label = 'numkdhh')
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Number of children', ylabel='Probability')
biased = BiasPmf(pmf, label = 'biased')
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased])
thinkplot.Config(xlabel='Number of children', ylabel='Probability')
pmf.Mean(), biased.Mean()
