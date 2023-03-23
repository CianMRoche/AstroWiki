## 8
**TESS finds an exoplanet. What can one directly determine from this measurement?** 
TESS is a transiting exoplanet survey (see [[#13]]) so one can determine the period simply enough, but also the radius in the following way, since TESS also measures spectral type and therefore also an estimate of the size and mass of the host star.
- Without an atmosphere: $\delta =\frac{\text{area of planet}}{\text{area of star}} = R_p^2 / R_*^2$ if we assume the emission is the same over the disk of the star. 
- With an atmospere of constant [[Optical depth#Optical depth|optical depth]] $\tau_\nu$ and atmospheric scale height $H$:  $$\delta = \frac{R_p^2 + 2R_p H(1 - e^{-\tau_\nu})}{R_*^2}$$though I dont understand why its $\tau_\nu$ here and not $\tau$ unless the $\delta$ is defined for some thin frequency band. 

From Megan's notes: Note that this would have to be normalized so that the lat bit on top is at 1 for the $\delta$ label to be correct. Otherwise $\delta$ is a ratio such that $F_{dip} = (1-\delta) F_{top}$
![[transit.png|300]]

One can also in some cases determine the temperature of the planet by measuring a much smaller dip when the planet passes behind the star. Need to assume both are blackbodies.

**What additional observations are needed to determine the mass of this planet?**
Need a radial velocity (ie spectroscopic follow-up). Why does this give you the mass? Start with [[Binaries#Kepler's laws|Kepler's third law]] $$\frac{P^2}{a^3} = \frac{4\pi^2}{GM_{tot}}$$Then replace $a$ with velocity by assuming circular orbit (most eccentricities in the solar system are below $e=0.1$) via $v = a\omega = a\,2\pi/P$ where $v$ is the **true** velocity in the orbit when the planet is moving along the line of sight (directly away from or towards us) and the fact that the radial velocity we measure depends on the inclination of the orbit as $v_r = v/\sin(i)$ where $i$ is the inclination angle of the orbit to get $$a = a_* + a_p =\frac{P}{2\pi\sin(i)}(v_{*,r}+v_{p,r})$$From Megan's notes (where line of sight is along the $v_r$ axis)
![[inclination.png|300]]

Since we only measure $v_{*,r}$ in practice, we use the mass ratio to express $v_{p,r}$ in terms of the other parameters. Since we measure the semi-major axes from the center of mass (focus of ellipse) it holds that $M_* a_* = M_p a_p$ and thus (again using circular orbits criteria above in the first step) $$\frac{a_p}{a_*} = \frac{v_p}{v_*} = \frac{M_*}{M_p}$$Then by using  Kepler' third law above we have $$ \frac{2\pi G}{P} = \left(\frac{v_{*,r}}{\sin(i)}\right)^3 \frac{M_{tot}^2}{M_p^3} \implies v_{*,r} = \left(\frac{2\pi G}{P}\right)^{1/3}\frac{M_p\sin(i)}{M_{tot}^{2/3}}$$can be solved impllicitly for $M_p$ or just approximate $M_{tot} = M_*$ for a simpler relation. There is a version one can derive without assuming circular orbits that results in $$v_{*,r} = \left(\frac{2\pi G}{P}\right)^{1/3}\frac{M_p\sin(i)}{M_{tot}^{2/3}} \frac{1}{\sqrt{1-e^2}}$$

## 9
**With what velocity precision must one measure the reflex motion of a sun-like star to detect an  
Earth-mass planet in a 1-year orbit about it?**
Based on the formula at the end of [[#8]], using a [[The Sun|solar]] mass star $M_* = 1\,\pu{M_\odot}$, $P = 1\,\pu{yr}$ , inclination $i = \pi/2$, and $M_p = 1 M_\bigoplus \simeq 6\times 10^{24}\,\pu{kg}$ we find a radial velocity amplitude of $v_{*,r }\sim\pu{cm\,s^{-1}}$  

So we would need centimeter per second velocity resolution or we wouldnt see any significant change over an orbit.

**What astrophysical processes complicate the measurement of radial velocities with this precision?**
Measured via spectrum.
- The material within the star is moving, causing noise in the spectra to appear
- Atmospheric seeing, turbulence in the atmosphere leads to additional noise in spectrum
- Need high-resolution spectrometer


## 10
**What is meant by the “obliquity” of an exoplanet orbit about its host star?**
Angular offset between spin axis of star and normal to plane of orbit



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