## Cepheids
Pulsating supergiant stars that show a period-luminosity relation that allow us to use them as standard candles, appearing on the high end of the [[HR-diagram#Instability strip|instability strip]]). 

**Typical parameters**: (mostly evolved [[Spectra#Harvard Spectral Classification|B-type]] stars)
- Mass $\sim 4-20\,M_\odot$
- Luminosity $\sim 10^3-10^5\,L_\odot$
- Radius $\sim 50R_\odot$
- Pulsation period $\sim 1-50\,\text{days}$

The pulsations come from sound waves resonating within the star (see [[#Kappa-mechanism]]), and as such can estimate pulsation period from sound crossing time of the star in the following manner, assuming a [[Polytropes#Polytrope|polytrope]] equation of state such that $$v_s = \sqrt{\frac{\partial P}{\partial \rho}} = \sqrt{\kappa\gamma\rho^{\gamma -1}} = \sqrt{\frac{\gamma P}{\rho}}$$Assuming [[Stellar structure equations#Hydrostatic equilibrium|HSE]] and an approximately constant density we then have $$\frac{dP}{dr} = -\frac{GM_{<r}\rho}{r^2} \simeq -\frac{4\pi G\rho^2 r}{3}$$such that integrating we get $$P(r) = \frac{2\pi}{3}G\rho^2(R^2 - r^2)$$and using the sound speed  $$v_s(r) \simeq \sqrt{\gamma\frac{2\pi}{3}G\rho(R^2 - r^2)}$$Then $$T \simeq 2\int_0^R dr\,\frac{1}{v_s} \simeq \sqrt{\frac{3\pi}{2\gamma G \rho}} \propto \frac{1}{\sqrt{\rho}}$$such that higher density stars pulsate faster. 


## RR-lyrae stars
Periodic variable stars, commonly found in [[Clustering#Globular Cluster|GCs]]. They are used as standard candles to measure (extra) galactic distances, assisting with the cosmic [[Hubble constant#Distance ladder|distance ladder]] as they are more common than [[#Cepheids]] but less reliable pulses (more unstable). 


## Pulse sources
p modes have pressure restoring force
g has grav (deeper interior)
r has coriolis "inertial modes"

and each probes a different layer of the star. That said, there are mixed modes (eg. gravoinertial modes) that couple these effects.


## Pulsating binaries
One of them pulsating. Binaries can break some degeneracy in mode analysis mass from spectra tidal effects


## Kappa-mechanism
The driving mechanism behind the changes in luminosity of many types of pulsating variable stars like [[#Cepheids]] and [[#RR-lyrae stars]]
 
- In a "normal" (non-pulsating) star, an increase in compression of the atmosphere causes an increase in temperature and density and thus ionized Helium; this produces a decrease in the [[Optical depth#Opacity|opacity]] (labelled $\kappa$) of the atmosphere, allowing energy to escape more rapidly (since light is not absorbed before reaching the edge as to would be in a more neutral medium). The result is an equilibrium condition where temperature and pressure are maintained in a balance. 
- However, in cases where the opacity increases with temperature, the atmosphere becomes unstable against pulsations. If a layer of a stellar atmosphere moves inward, it becomes denser and more opaque, causing heat flow to be reduced. In return, this heat increase causes a build-up of pressure that pushes the layer back out again. The result is a cyclic process as the layer repeatedly moves inward and then is forced back out again.