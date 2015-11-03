.. image:: http://www.astro.washington.edu/users/rodluger/img/templar_logo.jpg

A suite of Python routines to analyze Kepler lightcurve data using Gaussian processes 
and Markov Chain Monte Carlo. **templar** is still under development, so please check
back soon for more.

abstract
========

We present **templar**, a Python/C-based software package for generating robust posterior probability distributions of planet orbital parameters from the Kepler, K2, and TESS datasets. **templar** detrends KOI lightcurve data using a combination of pixel-level decorrelation (PLD) to remove instrumental systematics and Gaussian processes (GPs) to remove astrophysical red noise. The code uses an intelligent interpolation scheme to calculate fast transit lightcurves for the general case of a non-circular orbit with transit timing variations (TTVs). **templar** employs GPs to enforce a quasi-periodic covariance for the TTVs, yielding unbiased posterior distributions for the transit parameters even in the case of low signal-to-noise and small, previously undetected TTVs.

We are currently developing a catalog of posterior distributions for the transit parameters of ~2,000 short-period KOIs in conjunction with an observational campaign to constrain the masses and radii of their hosts. This catalog will greatly improve upon existing ones, which often assume circular orbits, periodic transit times, and uncorrelated photometric noise. The distributions will in turn allow us to better understand tidal evolution in planetary systems and provide independent constraints on the radius boundary between rocky and gaseous exoplanets. Both the catalog and the **templar** source code will be made publicly available on github.
