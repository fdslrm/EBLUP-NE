## Estimating variances in time series kriging using convex optimization and empirical BLUPs
*a research paper and supplementary materials - software, notebooks*

by **Martina Hančová, Andrej Gajdoš, Jozef Hanč, Gabriela Vozáriková**  
<martina.hancova@upjs.sk>

### Abstract of the paper

We revisit and update estimating variances, fundamental quantities in a time series forecasting approach called kriging, in time series models known as FDSLRMs, whose observations can be described by a linear mixed model (LMM). 

As a result of applying the convex optimization, we resolved two open problems in FDSLRM research: (1) theoretical existence and equivalence between two standard estimation methods --- least squares estimators, non-negative (M)DOOLSE, and maximum likelihood estimators, (RE)MLE, (2) and a practical lack of free available computational implementation for FDSLRM. As for computing (RE)MLE in the case of *n* observed time series values, we also discovered a new algorithm of order *O*(*n*), which at the default precision is 10<sup>7</sup> times more accurate and *n*<sup>2</sup> times faster than the best current Python(or R)-based computational packages, namely CVXPY, CVXR, nlme, sommer and mixed. 

The LMM framework led us to the proposal of a two-stage estimation method of variance components based on the empirical (plug-in) best linear unbiased predictions of unobservable random components in FDSLRM. The method, providing non-negative estimators with a simple explicit analytic form and performance comparable with REMLE in the Gaussian case, can be used for any absolutely continuous probability distribution of time series data. 

We illustrate our results via applications and simulations on three real data sets (electricity consumption, tourism and cyber security), which are easily available, reproducible, sharable and modifiable in the form of interactive Jupyter notebooks.

## Research paper 

This is a pre-print of an article published in [Statistical Papers](https://link.springer.com/journal/362). The final revised authenticated version is available online at: <https://link.springer.com/article/10.1007%2Fs00362-020-01165-5>

A preprint, the first version of the paper is available at <https://arxiv.org/abs/1905.07771>.

## Software [![render in nbviewer](misc/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/fdslrm/EBLUP-NE/blob/master/index.ipynb) 

The notebooks folders ([`Modeling`](Modeling), [`PYnotebooks`](PYnotebooks), [`Rnotebooks`](PYnotebooks)) contain Python based and R based Jupyter notebooks which are detailed records of our computing 
with explaining narratives ilustrating explored concepts and methods. 

Notebooks can be studied and **viewed** statically in [Jupyter nbviewer](https://nbviewer.jupyter.org/github/fdslrm/EBLUP-NE/blob/master/index.ipynb) [![render in nbviewer](misc/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/fdslrm/EBLUP-NE/blob/master/index.ipynb) with full visualisation. If there is a need, they can be also viewed directly on Github [`index.ipynb`](index.ipynb), also as a raw code. 

For interactive **executing** notebooks as live documents without any need to install or compile the software,
**use** the following links
* [`Python based notebooks using CVXPY and Scipy`](https://mybinder.org/v2/gh/fdslrm/Binder-CVXPY/master?filepath=index.ipynb) - [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fdslrm/Binder-CVXPY/master?filepath=index.ipynb)
* [`Python based notebooks using SageMath`](https://mybinder.org/v2/gh/fdslrm/Binder-Sage/master?filepath=index.ipynb) - [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fdslrm/Binder-Sage/master?filepath=index.ipynb)
* [`R based notebooks`](https://mybinder.org/v2/gh/fdslrm/Binder-R/master?filepath=index.ipynb) - [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fdslrm/Binder-R/master?filepath=index.ipynb)

There is also another very comfort alternative, fully tested by us, [CoCalc](https://share.cocalc.com/share/63aaaa44-3155-4ade-9e48-79bb8461aaf2/EBLUP-NE/?viewer=share/) providing interactive computing with our Jupyter notebooks.
 
All source code is distributed under [the MIT license](https://choosealicense.com/licenses/mit/).

## Related materials

The [`misc`](misc) folder contains our previously published papers related to the fdslrm project.

## Acknowledgements

This work was supported by the Slovak Research and Development Agency under the contract No. APVV-17-0568, the Scientific Grant Agency 
of the Slovak Republic (VEGA), VEGA grant No.1/0311/18 and the Internal Research Grant System of Faculty of Science, P.J. Šafárik  University in Košice (VVGS PF UPJŠ) &mdash; project VVGS-PF-2018-792.

## Further applications
The developed algorithms and open science digital tools were embedded and became a starting point for computational, simulation and theoretical reseach in our
current projects supported by the Slovak Research and Development Agency under the Contract no. APVV-21-0216 and APVV-21-0369.
