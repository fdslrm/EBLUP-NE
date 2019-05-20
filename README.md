## Estimating variances in time series linear regression models using empirical BLUPs and convex optimization
*a research paper and supplementary materials - software, notebooks*

by **Martina Hančová, Gabriela Vozáriková, Andrej Gajdoš, Jozef Hanč**  
<martina.hancova@upjs.sk>

### Abstract of the paper

We propose a two-stage estimation method of variance components in time series models known as FDSLRMs, whose observations can be described by a linear mixed model (LMM). We based estimating variances, fundamental quantities in a time series forecasting approach called kriging, on the empirical (plug-in) best linear unbiased predictions of unobservable random components in FDSLRM. 

The method, providing invariant non-negative quadratic estimators, can be used for any absolutely continuous probability distribution of time series data. As a result of applying the convex optimization and the LMM methodology, we resolved two problems &mdash; theoretical existence and equivalence between least squares estimators, non-negative (M)DOOLSE, and maximum likelihood estimators, (RE)MLE, as possible starting points of our method and a practical lack of computational implementation for FDSLRM. As for computing (RE)MLE in the case of *n* observed time series values, we also discovered a new algorithm of order *O*(*n*), which at the default precision is 10<sup>7</sup> times more accurate and *n*<sup>2</sup> times faster than the best current Python(or R)-based computational packages, namely CVXPY, CVXR, nlme, sommer and mixed. 

We illustrate our results on three real data sets &mdash; electricity consumption, tourism and cyber security &mdash; which are easily available, reproducible, sharable and modifiable in the form of interactive Jupyter notebooks.

## Research paper 

The research paper has been submitted for publishing in [Statistical Papers](https://link.springer.com/journal/362).

A preprint version is available at <https://arxiv.org>.

## Software [![render in nbviewer](misc/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/fdslrm/EBLUP-NE/blob/master/index.ipynb) [![launch binder](misc/binder_badge.svg)](link)

The notebooks folders ([`Modeling`](Modeling), [`PYnotebooks`](PYnotebooks), [`Rnotebooks`](PYnotebooks)) contain Python based and R based Jupyter notebooks which ilustrate explored concepts and methods. 

Notebooks can be statically viewed on Github [`index.ipynb`](index.ipynb) or **rendered** in [Jupyter nbviewer](https://nbviewer.jupyter.org/github/fdslrm/EBLUP-NE/blob/master/index.ipynb) with full visualisation 
[![render in nbviewer](misc/nbviewer_badge.svg)](link) or **executed** in [Binder](link) [![launch binder](misc/binder_badge.svg)](link) without any need to install or compile the software.

All source code is distributed under [the MIT license](https://choosealicense.com/licenses/mit/).
