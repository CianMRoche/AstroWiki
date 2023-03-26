## Space-based detector orbits
**Lagrange points** - JWST

**Low Earth orbit** - HITOMI XRISM SWIFT NuSTAR AMS (on ISS)

**Lunar resonsance** - TESS

**High Earth orbit** - Chandra XMM


## Telemetry
The recording and communication of information from the instrument to us. In the context of space-based observatories, refers to returning the data to Earth via a retrieval mechanism like the [[Observatories#Deep space network|deep space network]].


## Long baseline interferometry
Using multiple detectors, one can increase the effective resolution to an instrument of the same size as the separation between detectors (but with less light collection area). 

The image below shows that detectors aligned colinearly improve the resolution along that axis (variation in that dimension of the image happens more quickly than orthogonal direction). Need to use at least a triangle if you want details in both dimensions
![[interferometry.png|650]]


## Strell ratio
ratio of power in wings of psf versus in sharp bit in middle


## Reverberation mapping
Uses the time lags between correlated observed signals to infer information about the environment very close to a black hole. See [this page](https://ned.ipac.caltech.edu/level5/March10/Peterson/frames.html) for a reverberation mapping overview.

**Optical/broad line region:** 
Measure the delay between optical broad lines wrt continuum; light travel time induces a delay $\tau_{LT} \sim R_{BLR}/c$ to estimate location of the broad line region.

Can relate the mass of the black hole to the location of the BLR and velocity dispersion of lines via $$M_{BH} = \frac{f(\Delta\,v)^2\,R_{BLR}}{G}$$where $f$ is a scale factor related to geometry and kinematics of the broad line region. Usually about 5.

Requirements:
- High time resolution ($\lesssim 1$ day)
- Long duration monitoring (~ months)
- Moderate spectral resolution ($\sim 600\,\pu{km\,s^{-1}}$)
- High signal to noise

**X-ray**
Probe time delays between corona and disk in reflection features ($\tau_{LT, Xray} \ll \tau_{LT,opt}$). Can fit lag enegry spectrum to measure the mass, as the lag depends on the mass since we are probing $R_{\rm{ISCO}}$ 