## 8
**TESS finds an exoplanet. What can one directly determine from this measurement?** 
TESS is a transiting survey (see [[#13]]) so one can determine the period simply enough, but also the radius in the following way:
- Without an atmosphere: $\delta = R_p^2 / R_*^2$ 
- With an atmospere of constant [[Optical depth#Optical depth|optical depth]] $\tau_\nu$:  $$\delta = \frac{R_p^2 + 2R_p H(1 - e^{-\tau_\nu})}{R_*^2}$$ 
From Megan's notes:
![[transit.png|300]]

One can also in some cases determine the temperature of the planet

**What additional observations are needed to determine the mass of this planet?**







## 13
**Describe four methods for detecting an exoplanet, and the potential biases in the inferred  
populations of planets associated with each method. Roughly how many planets have been  
detected using each?**
1. **Transits** (~3500 confirmed as of 2022)
   If the planet passes in front of the star along the line of sight, we see a dip in the flux of light, the shape being approximately trapezoidal (but with curvy edges)
   
   Direct observables:
   - Period (if you observe at least 2 transits)
   - Size of planet
   - Temperature of planet can in theory be observed when the planet goes behind star, should see the subtraction of a blackbody spectrum at a certain temperature

   Problems:
   - Biased towards detecting planets close to the star
   - Biased towards larger planets
   - Increasing sensitivity reduces effect of biases
   - Can only detect edge-on binary systems

2. **Direct imaging** (~25 confirmed as of 2022)
   Look at a star + planet system. The planet emits as a [[Blackbody radiation|blackbody]], goal is to subtract the star's light to observe the planet's spectrum (+ temperature). Related to temperature measurement of transit method.
   
   Direct observables:
   - Radius of orbit (if distance to system is known)
   - If proper motion can be determined, the period of the orbit

   Problems:
   - Biased towards detecting hot and/or large planets (more blackbody flux to increase planet/star contrast)
   - Require large separations to be able to resolve planet $\implies$ biased toward long-period planets
   
3. **Microlensing** (~100 confirmed as of 2022)
   When a background source is lensed by a foreground star, a planet which orbits in the [[Einstein ring]] can briefly increase the magnification of the lensing, resulting in an increase in flux.   ![[microlensing.jpg]]
   
   Direct observables:
   - Timescale of orbit (require accurate relative proper motion of lens-source system)

   Problems:
   - Detection probability maximized when separation of planet-star system is $\sim$ size of Einstein ring at that distance $\implies$ bias toward large-separation systems
   - Mostly independent of mass of planet

4. **Radial velocity** (~1000 confirmed as of 2022)
   Measure wobble of star due to gravitational influence of planet(s). First planet discovered with this method was [[Exoplanet examples#51 Pegasi b|51 Peg b]]. 

   Direct observables:
   - Period
   - Semi-amplitude of velocity shift $\implies$ lower bound on mass (see [[#8]])

   Problems:
   - Measuring shift of spectral lines $\implies$ biased toward large masses to have large enough spectral line shifts. 
   
5. **Pulsar timing** 
   The first exoplanet was discovered in 1992 by Aleksander Wolszczan and Dale Frail using [[Pulsar timing]] methods. These exoplanets orbit a [[Neutron stars#<mark class="hltr-orange">Pulsar</mark>|pulsar]], and small periodic changes in the pulsar period indicate the gravitational influence of a companion. Stars discovered by this method are poor cadidates for life because they live next to a terrifying pulsar.  

**In summary**:
![[exoplanet_methods.png|450]]