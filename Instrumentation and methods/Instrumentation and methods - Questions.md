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

Lets quantify the number of photons observed per pixel $N$ and the various contributions to noise in that pixel's counts, without making explicit any frequency dependence.

Signal:
- $N$ = number of photons from the source + sky background + anything else
- $N_s$ = number of photons after we calibrate and quantify the other sources ($N_b, N_d, N_r$ below), and subtract their counts per pixel times umber of pixels, leaving an estimate of the **total** source counts.

Noise contributions:
- $\sigma_s = \sqrt{N_s}$ = poisson noise from source 
- $\sigma_b = \sqrt{N_b}$ = poisson noise per pixel from background 
- $\sigma_d = \sqrt{N_d}$ = poisson noise per pixelfrom dark current (thermal noise in electrons, decreases if we lower temperature)
- $\sigma_r = N_r$ = [[Electronics#Read noise|read noise]] per pixel

The total magnitude of the noise is then the following, assuming all the above are independent $$\sigma = \sqrt{\sigma_s^2+n(\sigma_b^2+\sigma_d^2+\sigma_r^2)} = \sqrt{N_s+n(N_b+N_d+N_r^2)}$$where $n$ is the number of pixels. Thus the signal to noise ratio is $$\frac{\rm{Signal}}{\rm{Noise}}= \frac{N_s}{\sigma}$$**What terms dominate at optical versus infrared wavelengths?**

At [[Spectra#The electromagnetic spectrum|optical]] wavelengths we are usually object-limited, meaning the dominant source of noise is the large number of source counts $\sigma \simeq \sqrt{N_s}$ (even though the percentage error decreases with number of counts for poisson processes, the magnitude of the error itself still increases. Since this is assumed independent of the other sources, it will eventually dominate). 

At IR wavelengths the dark current is significant so $\sigma \simeq \sqrt{n N_d}$ (why? not sure).

**Why, when observing objects that are fainter than physical foregrounds like the night sky, does SNR increase as sqrt(time)?**

Look at the observation in terms of intrinsic rates multiplied by exposure times $$N_s = R_st,\quad N_b =nR_bt,\quad N_d = nR_dt, \quad N_r = nR_r $$where $R_s$ has units photons per second and the others have units photons per second per pixel, noting that the read-out is time-independent. We can rewrite the signal to noise as $$\frac{\rm{Signal}}{\rm{Noise}}= \frac{R_s t}{\sqrt{R_s t + n(R_b t + R_d t + R_r^2)}} = \frac{R_s \sqrt{t}}{\sqrt{R_s + n(R_b + R_d + R_r^2/t)}}$$So for everything except readout noise, it scales as $\sqrt{t}$. 