## 153
**Explain how a radio interferometer manages to produce sub-arcsecond images when none of the constituent dishes has an angular resolution of better than 1 arcmin.**

See [[Methods#Long baseline interferometry|LBI]]. Via [[#156|Q156]] can calculate that the diffraction limitation for the angular resolution of a radio telescope of diameter $D$ observing at a wavelength $\lambda$ is $$\Delta \theta  = 1.22\frac{\lambda}{D}$$where $\Delta \theta$ is measured in radians. Since $\lambda$ is relatively large for [[Spectra#The electromagnetic spectrum|radio]] we need a large dish to get decent angular resolution. One [[Units#Arcsecond|arcsecond]] is about $5\times 10^{-6}\,\pu{rad}$ and so at a wavelength of $1\,\pu{m}$ to get arcsecond resolution we would need a dish about $200\,\pu{km}$ across. We thus use multiple dishes (with careful clock-synchronization) to get bettwe resolution but much less collecting area than a telescope that large. [[Observatories#EHT|EHT]] has a basline of $\sim 1000\,\pu{km}$ so that at $1\,\pu{mm}$ we get $\sim 25\,\pu{\mu as}$ resolution.


## 154
**How does an X-ray telescope image? Why is it necessary to have the reflection take place at grazing angles of incidence?**
[[Spectra#The electromagnetic spectrum|X-rays]] dont usually reflect off of materials. For dense materials they get absorbed, and for rare materials they pass straight through. They can however be reflected for very large angles of incidence ("grazing incidence") in the same way that if you drop a stone in a pond, it will fall down through the water, but if you throw it quickly at grazing incidence it can skip across the surface. Our X-ray forcusing mirros thus look like this (for a Wolter type-1 telescope like [[Observatories#CHANDRA|CHANDRA]])
![[chandra_optics.png|500]]

looking at the foci of the different types of mirrors in this type-1 case we see

![[wolter_type1.png|500]]
The mirrors are often coated in gold or nickel since X-rays reflect best off of high-Z metals. When observing X-rays with a [[Electronics#CCD|CCD]] sensor, the incident photon energy is about equal to the energy released when hitting the detector, so we get low frequency-resolution spectra for "free".


## 155 
**How would you calculate the “signal-to-noise ratio” for a standard ground-based telescope performing CCD imaging?**

Lets quantify the number of photons observed $N$ and the various contributions to noise in those counts, without making explicit any frequency dependence.

Signal:
- $N$ = number of photons from the source + sky background + anything else
- $N_s$ = number of photons after we calibrate and quantify the other sources ($N_b, N_d, N_r$ below), and subtract their counts, leaving an estimate of the **total** source counts.

Noise contributions:
- $\sigma_s = \sqrt{N_s}$ = poisson noise from source 
- $\sigma_b = \sqrt{N_b}$ = poisson noise from background 
- $\sigma_d = \sqrt{N_d}$ = poisson noise from dark current (thermal noise in electrons, decreases if we lower temperature)
- $\sigma_r = N_r$ = [[Electronics#Read noise|read noise]]

The total magnitude of the noise is then the following, assuming all the above are independent $$\sigma = \sqrt{\sigma_s^2+\sigma_b^2+\sigma_d^2+\sigma_r^2} = \sqrt{N_s+N_b+N_d+N_r^2}$$where $n$ is the number of pixels. Thus the signal to noise ratio is $$\frac{\rm{Signal}}{\rm{Noise}}= \frac{N_s}{\sigma}$$**What terms dominate at optical versus infrared wavelengths?**

At [[Spectra#The electromagnetic spectrum|optical]] wavelengths we are usually object-limited, meaning the dominant source of noise is the large number of source counts $\sigma \simeq \sqrt{N_s}$ (even though the percentage error decreases with number of counts for poisson processes, the magnitude of the error itself still increases. Since this is assumed independent of the other sources, it will eventually dominate). 

At IR wavelengths the dark current is significant so $\sigma \simeq \sqrt{N_d}$ (why? not sure).

**Why, when observing objects that are fainter than physical foregrounds like the night sky, does SNR increase as sqrt(time)?**

Look at the observation in terms of intrinsic rates multiplied by exposure times $$N_s = R_st,\quad N_b =nR_bt,\quad N_d = nR_dt, \quad N_r = nR_r $$where $R_s$ has units photons per second and the others have units photons per second per pixel, noting that the read-out is time-independent. We can rewrite the signal to noise as $$\frac{\rm{Signal}}{\rm{Noise}}= \frac{R_s t}{\sqrt{R_s t + n(R_b t + R_d t + R_r^2)}} = \frac{R_s \sqrt{t}}{\sqrt{R_s + n(R_b + R_d + R_r^2/t)}}$$So for everything except readout noise-dominated, it scales as $\sqrt{t}$. 


## 156
**What is the diffraction limit for a telescope?**
Minimum angular separation that can be resolved by a telescope, set by the observing wavelength and diameter of the telescope. $$\theta_{min} = \frac{1.22\lambda}{D}$$Arises due to the width of the central peak in the Airy disk, which is the diffraction patters of light passing through a circular aperture.
![[airy.png|200]]

**Why does the signal-to-noise ratio scale like D^4 for diffraction limited imaging on ground-based telescopes with diameter D at IR wavelengths?**

The energy from a source hitting a detector of diameter $D$ per time is $$N = \frac{\pi D^2F}{4} \propto D^2$$where $F$ is the [[Units#Flux|flux]] of the source. In the [[Spectra#The electromagnetic spectrum|IR]] $\lambda$ is large and thus via diffraction limit $\theta \sim \lambda/D$ we have that the angular resolution is large (ie bad). Increasing $D$ makes $\theta_{min}$ go down as $D^{-1}$, and the number of "non-source" photons go down as the corresponding area (ie $D^{-2}$).

Then signal ($\propto D^2$) over noise ($\propto D^{-2}$)will go as $D^{4}$.


## 157
**Briefly describe the following kinds of astronomical instruments and their purpose:** 
Many from Megan's notes.

**(i) Schmidt camera** 
Optical telescope with large FOV and limited aberration. 

Examples: Hipparcos, Kepler
![[schmidt.png|400]]

**(ii) Ritchy-Chretien telescope** 
Specialized Cassegrain telescope with two hyperbolic mirrors to eliminate off axis  optical errors (a "classic" Cassegrain has parabolic primary mirror and hyperbolic secondary mirror). Similar to Shmidt but replace plate with mirror.

Examples: [[Observatories#HST|HST]], [[Observatories#VLT|VLT]], [[Observatories#KECK|Keck]] 
![[Ritchy_Chretien.png|400]]

**(iii) Multi-object spectrograph** 
Spectrograph that can get a spectrum for multiple different targets/points on the sky at a given time. Employed on almost all ground based telescopes these days.

Many different types:
- multi fiber ([[Catalogs#SDSS|SDSS]])
- multi slit ([[Observatories#GMT|GMT]]))
- slitless (Nirspec on [[Observatories#JWST|JWST]])
- integral field unit (IFU, e.g Gemini)

**(iv) Echelle spectrograph**
Diffraction grating that is optimized for high incident angles + high diffraction orders which gives better spectral resolution. 

Uses two gratings (one $\perp$ to the other) to cross disperse the light + separate the overlapping high orders

**(v) CCD**
See [[Electronics#CCD|CCD]]

**(vi) Coronograph** 
Instrument on a telescope used to block out the direct light from a star to see other dimmer features like solar corona or exoplanets.

Moon acts like a coronograph during solar eclipse

Examples: [[Observatories#JWST|JWST]] has Nircam+MIRI, [[Observatories#HST|HST]] has NIMCOS

**(vii) Laser interferometer**
Uses relative phases of two paths along which a light beam can travel to infer changes in proper length along the two paths. Eg [[Observatories#LIGO|LIGO]]
![[interferometer.png|400]]

**(viii) Adaptive optics**
Deformable mirrors for ground-based telescopes which can counter atmospheric turbulence and blurring using bright sources on the sky as "guides" for very fast timescale corrections. Measure time-dependent deflection of bright source and correct that deflection.

Examples: [[Observatories#VLT|VLT]], [[Observatories#KECK|Keck]]


## 158
**What limits the angular resolution of ground-based telescopes at 1μm, 10μm, or 100m?**

These are [[Spectra#The electromagnetic spectrum|Near-IR]], mid-IR and radio wavelengths. 
![[Atmospheric_electromagnetic_opacity.svg.png]]
![[absorb_atmosphere.svg]]

1. Near-IR
   Water absorbs strongly here, but can observe here at high altitudes where air is dry (or in desert, including poles). Atmospheric seeing limits resolution to $\theta_{atm} = 0.5 \gg \theta_{min}$ where the min is set by diffraction limitation (see [[#156|Q156]]) for a $10\,\pu{m}$ telescope, but can be overome somewhat by adaptive optics.
2. Mid-IR
   Absorbed by $\ce{CO_2}$ in the atmosphere, space often necessary for mid-IR observations, where observations are only diffraction-limited. 
3. Radio
   Far radio ($\gtrsim 10\,\pu{m}$) absorbed by ionosphere (related to [[Plasma and lensing - Questions#93|plasma frequency]]) so best to go to space. Resolution here limited by this absorption, but in mid-radio are diffraction-limited (below $10\,\pu{m}$)


## 159
**What are "apparent magnitude," "absolute magnitude" and "bolometric magnitude"? What are U,B and V colors?**
See the inset magnitudes file:
![[Magnitudes]]


## 160
**Briefly describe the main objectives and capabilities of the following astronomical observatories**
I wont link them all individually here, see [[Observatories]] for all.


## 161
**What are the pros/cons of having a space-based versus ground-based observatory? At what wavelengths can you do both? At what wavelengths can you only observe from space?**
From Megan's notes:
![[space_ground.png]]

See [[#158|Q158]]. 

Can do on ground and in space:
- Optical
- some NIR
- sub-mm
- radio

Need space:
- $\gamma$-ray
- X-ray
- UV
- most IR


## 162
**Derive the approximate (within a factor of a few) spectral resolution R required to detect a planet that perturbs its host star by a radial velocity amplitude of 10 cm/s.**
The spectral resolution of a spectrograph, or, more generally, of a frequency spectrum, is a measure of its ability to resolve features in the electromagnetic spectrum. It is usually denoted by $\Delta \lambda$, and is closely related to the resolving power of the spectrograph, defined as $$R = \frac{\lambda}{\Delta\lambda}$$where $\Delta \lambda$ is the smallest <mark class="hltr-pink">difference in wavelengths</mark> that can be distinguished at a wavelength of $\lambda$. The spectral resolution can also be expressed in terms of physical quantities, such as velocity; then it describes the difference between velocities $\Delta v$ that can be distinguished through the [[Spectra#Relativistic Doppler shift|doppler shift]]. Then, the resolution is $\Delta v$ and the resolving power is $$R = \frac{\lambda}{\beta\lambda} = \frac{1}{\beta}= \frac{c}{\Delta v}$$For a radial velocity measurement of $\sim 10\,\pu{cm s^{-1}}$ (see [[Exoplanets - Questions#9|Q9]] to understand order of magnitude) this would mean a resolving power of $R \sim 10^9$ but the best that exists right now is $R\sim 10^5$ on HARPS. 

The resolution is the ability to distinguish between lines, but really we need to measure the position of the center of a line (and compare it to the rest frame value to get a radial velocity). If we measure multiple lines rather than just one, we can measure shifts below the spectral resolution of the instrument. In general, if we have an observable $X$ and we can measure it to be $\mu_X$ with uncertainty for a single observation $\sigma_X$, then our uncertainty on the value of $\mu_X$ can be reduced by repeating observations (for a Gaussian process if we made the observation a billion times, we would get a beautiful Gaussian of well-measured width $\sigma_X$ and a very certain mean value $\mu_X$). The scaling on the uncertainty of the mean $\sigma_{\mu,X}$ for repeating the observation $N$ times is  $$\sigma_{\mu,X} = \frac{\sigma_X}{\sqrt{N}}$$In the case at hand, we want to measure the position of the center of a line $\mu$ which we do with some uncertainty $\sigma$ set by the spectral resolution, and if we measure several lines we can improve sensitivity roughly via the same math as above (since we are in principle measuring different things each time, but to get the same number) to get $$\sigma_\mu = \frac{\sigma}{\sqrt{N}}$$where $N$ is the number of lines. 

**Describe some practical challenges with calibration and stability, and how they are addressed for such instruments. Why have we not yet achieved this precision in RV measurements of real stars?**

Challenges:
- Instrument has to be extremely stable. Vacuum to prevent pressure fluctuations, cooled to prevent thermal fluctuations, no moving parts ideally, calibration via known sources
- Sources also vary in that they are spinning and have intrinsic variability in their atmospheres etc, which is really hard to subtract from signal. Has been proposed to observe in minima of solar cycles of stars strategically to minimize this effect.


## 163
**Summarize the current state of experimental gravitational wave detection, and the prospects for improvement in the near future**
Current: 
[[Observatories#LIGO|LIGO]] did the following (main points):
- GW150914 (14th Sept 2015) a [[Binaries|binary]] [[Black holes#Black hole|BH]] merger with [[Gravitational waves#Chirp mass|mass]] $\sim 30\,M_\odot$ which resulted in Nobel prize
- GW170817 (17th Aug 2017) a binary [[Neutron stars#Neutron stars|NS]] merger followed up by [[Observatories#Fermi|Fermi]] [[GRBs#GRB|GRB]] detector.
- GW190521 (21st May 2019) a binary BH merger for which one of the progenitors and the remnant lay in the [[Black holes#Pair instability gap|pair instability gap]] (one $\sim 85\,M_\odot$ progenitor and $\sim 150\,M_\odot$ intermediate mass BH remnant)

VIRGO and KAGRA also exist and form the LVK collaboration.

Future:
- continued improvement of LIGO, VIRGO and KAGRA GW observatories to build statistics and template generation
- [[Observatories#LISA|LISA]] which will be more sensitive to extreme mass ratio inspirals and supermassive BH mergers
- Cosmic explorer: Two $40\,\pu{km}$ arm observatories on the ground which increases sensitivity (sensitivity $\propto L^{2}$ says LISA paper but diminishing returns since longer arms means not sensitive to high frequency waves) with no additional noise (ideally).