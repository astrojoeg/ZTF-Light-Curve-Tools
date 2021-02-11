# ZTF-Light-Curve-Tools
Python tools for time series analysis of Zwicky Transient Facility photometry.

Currently, I have only one script uploaded that estimates the 0.1% false alarm probability significance threshold for the Lomb-Scargle periodogram of the light curve. This is accomplished via bootstrapping the ZTF time series 10,000 times with replacement, and then calculating the 99.9th percentile of the distribution of maximum amplitudes of each periodogram.

I have a script in development that finds all the significant frequencies aboce this estimated threshold by running an automated prewhitening routine on the light cuve's periodogram, but it's a bit messy at the moment.

A script to apply the filtering to ZTF light curves as recommended by [Guidry et al. 2020](https://ui.adsabs.harvard.edu/abs/2020arXiv201200035G/abstract) and barycentric corrections to the timestamps will be up here soon too!
