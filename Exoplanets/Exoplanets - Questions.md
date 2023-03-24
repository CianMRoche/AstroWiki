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

So we would need centimeter per second velocity resolution or we wouldnt see any significant change over an orbit. No instrument does this, best is about $0.3\,\pu{m s^{-1}}$ of ESPRESSO on the [[Observatories#VLT|VLT]] with the goal to push to $0.1\,\pu{m s^{-1}}$ 

**What astrophysical processes complicate the measurement of radial velocities with this precision?**
Measured via spectrum.
- The material within the star is moving, causing noise in the spectra to appear
- Atmospheric seeing, turbulence in the atmosphere leads to additional noise in spectrum
- Need high-resolution spectrometer
- very hot stars (O,B,A) may not have enough narrow lines in their spectra for precise Doppler shift measurements.
- Need to understand the relative motion of Earth in the Solar system to the star down to $\pu{cm\,s^{-1}}$ precision.


## 10
**What is meant by the “obliquity” of an exoplanet orbit about its host star? How can obliquity be measured, and what are typical values?**
Angular offset between spin axis of star and normal to plane of orbit, or equivalently the angle between the planets spin axis and the ecliptic plane (orbital plane of planets around star). 

Can measure by the **Rossiter-Mclaughlin effect**, which is basically the fact that during a transit for which we have spectra, the planet will first block red or blue-shifted light, then block the other, causing a rise and fall in the measured radial velocity. ![[Rossiter-McLaughlin_effect.png|600]]
This can also be used to infer an obliquity based on how the inferred radial velocity varies over a transit. If the shape of the velocity anomaly (ie radial velocity relative to "mean") is asymmetric, the planet covers the approaching side more or less than the receding side, meaning the orbit is oblique
![[Rossiter-McLaughlin_velocity_anomaly.png|400]]

Values of obliquity in the Solar system: Variable, often small
![[obliquity.jpg|500]]

Other methods that have been used:
- Transit of planet over star spots (I guess if it passes two of them?) eg. Deming+11, Desert+11
- Gravity darkening from rapid stellar rotation, eg. Barnes +09,11
- Asteroseismology, eg. Chaplin+13


## 11
**What is meant by tidal locking between an exoplanet and its host star?**
When there is no change in the planets rotation rate over an orbit. Arises by similar mechanism to [[The Solar System - Questions#4|4]] whereby todal bulges result in a torque that exchanges angular momentum between the stars spin (slows down) and planets orbit (gets angular momentum so goes further away), until a point where net torque is zero.

Can lead to **synchronous rotation** as for the Earth-Moon system, wherein the orbital period = rotation period of planet, causing the same side of the planet to always face the star (or same side of moon to always face planet)

Can also lead to **asynchronous locking** such as the 3:2 spin:orbit resonance of Mercury around the Sun. (does Mercury also have an orbit:orbit resonance with other planets?)

**What are the circumstances where planets are likely to be tidally locked?**
Closer to host star $\implies$ higher torque, becomes locked more quickly / influence is larger. 

See C+O 2nd edition pg 722

## 12
**Describe qualitatively one of the theories explaining the presence of hot Jupiters -- Jupiter mass
planets orbiting at separations of less than 0.05 AU from the star**

**Hot jupiter** 
A ~Jupiter sized planet very close to host star. [[Exoplanet examples#51 Pegasi b|51 Peg b]] is an example.
- $a \lesssim 0.05\,\pu{AU}$
- $P \lesssim 10\,\pu{days}$

One possible explanation for existence is formation of planets far out and then [[Binaries#Tidal migration|tidal migration]]. Another possible explanation is **disk migration**, and finally **in-situ formation**. Disk migration is a migration which happens when the hot protoplanetary disk still exists, and in-situ is the direct formation near stars, however this has been shown to be very hard (see below).

Many detected hot Jupiters (see [[#11]]) have high obliquity, suggesting their orbit may be due to dynamical interaction rather than simple orbit migration.

The proposed steps for the tidal migration scenario are:
1. Large planet formed far out 
2. Orbit becomes eccentric via scattering from other planets, secular chaos in many-body systems or Lidov-Kozai oscillations in binary star systems
3. Tidal forces during pericentric passage shrink and circularize the orbit of the planet 

**Why was the discovery of these planets such a surprise?**
Astronomers did not expect giant gas planets to form at a radius that close to the host star. Giant planets are thought to form either by core accretion, in which a rocky proto-planet core accretes many times its mass in gas from the proto-planetary disk, or gravitational instability, in which part of the proto-planetary disk fragments into bound clumps. Close to the star, gas conditions prevent formation by gravitational instability. Core accretion can operate close to the star, but building a sufficiently large core (∼10M⊕) is challenging. Feeding zones are small so the local available solids are insufficient, mergers of multiple smaller cores are prevented by the disk, and accretion of radially transported pebbles stalls at a much lower mass. It is almost certain that these hot Jupiters could not have formed where they are observed today, but rather have formed further out and migrated to their current location. While there are theories, the exact mechanisms are still unclear and more than one formation pathway is needed


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
   - Measuring shift of spectral lines $\implies$ biased toward large masses to have large enough spectral line shifts. Dont measure Earth-mass planets yet (see [[#9]]).
   
5. **Pulsar timing** 
   The first exoplanet was discovered in 1992 by Aleksander Wolszczan and Dale Frail using [[Pulsar timing]] methods. These exoplanets orbit a [[Neutron stars#<mark class="hltr-orange">Pulsar</mark>|pulsar]], and small periodic changes in the pulsar period indicate the gravitational influence of a companion. Stars discovered by this method are poor cadidates for life because they live next to a terrifying pulsar.  

**In summary**:
![[exoplanet_methods.png|450]]


## 14
**Describe a sequence of observations to identify an exoplanet, to determine that it has a rocky
composition, and to measure the chemical constituents of its atmosphere.**
1. Discovery likely to be by transits or radial velocity. Transit gives you $R_p$ (see [[#8]]), and this may or may not include the atmosphere, depending on wavelength of observation and atmospheric composition.
2. Radial velocity measurement can constrain $M_p$ (if planet $\gtrsim 10\,\pu{M_\odot}$, see [[#8]], [[#13]]) 
3. $M_p$ and $R_p$ gives an estimate of the density. Higher density (lower radius for a given mass) means rockier planet. There exist some mass-radius relationships for planets of different composition to do the actual constraining.
4. For the atmosphere, look for absorption features in the spectrum during a transit.

**What have we learned about exoplanet interiors and atmospheres from these observations?**
- High level of diversity in exoplanet composition and properties
- Have seen hot Jupiters with opaque clouds and inflated planets with larger radii than expected (how would we know this? Not with the method described above anyway)


## 15
**Why are M Dwarfs thought to be promising candidates for identifying Earth-sized, temperate (but
not necessarily habitable) planets?**
