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