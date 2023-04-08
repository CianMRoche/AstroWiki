## 100
**Make a sketch of the Galaxy to scale (top and side views) and indicate its various features and properties. How are stars, gas, dust, and dark matter distributed in our Galaxy?**

See [[Galaxies#Galaxy|galaxies]] for an overview and some images of different types of real galaxy. A schematic of a non-elliptical galaxy, in particular the [[Milky Way#Milky Way|Milky Way]] (from Megan's notes) is 
![[galaxy_schematic.png]]

Features of the different components:
1. Bulge
   - Old and metal-poor (metallicities of $z\sim 10^{-2}-10^{-3}$)
   - Contains [[Clustering#Globular Cluster|globular clusters]] with $\sim 10^6$ stars each
   - Hosts the galactic nucleus, which may have [[Black holes#Black hole|supermassive black hole]] or act as an [[AGN#AGN|AGN]]. For the Milky Way it is in [[AGN examples#Sagittarius A|Sagittarius A]].
2. Disk (see [[Galaxies#Disk galaxy|disk galaxy]] for details of when we have a disk or elliptical)
   - Young and metal-rich
   - Actively forming stars
   - Can exhibit spiral structure (except in lenticular [[Galaxies#Galaxy|galaxies]]) and a barred structure (hypothesized to be a recurrent dynamical feature while in the disk phase)
   - Contains the majority of the [[Dust#Dust|dust]] and gas in the galaxy.
   - See [[Galaxies#Disk galaxy|disk galaxies]] for a comparison of the thin and thick disk components
3. Stellar halo
   - Like the bulge contains an old and metal-poor population 
   - Contains remnants of minor sattelite galaxy mergers  (which has been used as a test of [[LCDM#LCDM|LCDM]])
   - Stars in the halo can be used to constrain the density profile of the Milky Way by inferring the escape velocity profile. I do this, google "escape velocity profile of milky way gaia dr3".
4. Dark matter halo
   - A quasi-spherical distribution of dark matter which can explain the flat rotation curves (circular velocity of stars as a funciton of radius) seen in galaxies (amongst other things, see [[Dark matter]] and [[#101|Q101]]).
   - The dominant component at large scales (see picture above).


## 101
**What observational evidence do we have for dark matter in galaxies and clusters of galaxies?**

<mark class="hltr-pink">Galaxy rotation curves</mark>
Newtonian dynamics predicts the following for the circular velocity of a stars in a galaxy $v_\phi$ versus galactocentric radius $r$ (see [[Binaries#Circular motion|circular motion]])$$m\frac{v^2}{r} = \frac{GM(<r)m}{r^2} \quad \implies \quad v_\phi = \sqrt{\frac{GM(<r)}{r}}$$The majority of the stellar mass in the [[Milky Way#Milky Way|Milky Way]] is contained within about $10\,\pu{kpc}$ and so we expect to see the circular velocity decrease, approaching a $1/\sqrt{r}$ curve as we "add no more enclosed mass with increasing radius". Excellent summary is below, from Xiaowei's paper. The dotted curves are all bayonic, with the gray dotted curve as the sum of all baryonic matter. The black line is a fit moddelling a DM halo as an Einasto profile (see [[#118|Q118]]). Clearly the baryonic matter we see cannot explain the rotation curves of the Milky Way (also seen in other galaxies). Can use [[Spectra#21cm line|12cm line]] to map rotation curves too (see [[#103|Q103]]).

![[rotation_curves.png]]
<mark class="hltr-pink">Galaxy velocity dispersion in clusters</mark>
Goes back to Zwicky in the 1930s observing the [[Galaxy cluster examples#Coma cluster|Coma cluster]]. The galaxies in [[Galaxy clusters#Galaxy cluster|clusters]] are moving with speeds far greater than can be explained by the observed stellar mass. In order to explain these speeds one would need a much greater mass, but our knowledge of the connection between mass and luminosity for galaxies (like the Schechter luminosity function) means that such a collection of galaxies should be far brighter. 

It is true that galaxies in clusters have an anomalous mass to light ratio, in that there is more mass for a given luminosity than we would expect for the same luminosity outside of a cluster (the reason being because cluster environments strip gas inhibiting star formation, and are primarily populated by "red and dead" ellipticals). However, the discrepancy observed between an inferred mass from light and the kinematics is still an order of magnitude.

In a similar manner to to measuring the mass of elliptical galaxies using *stellar* [[Velocity dispersion#Velocity dispersion|velocity dispersion]] (which can also be evidence for dark matter), we can measure the mass of a cluster via the galaxy velocity dispersion by assuming it is virialized, finding $$M \simeq \frac{3}{2}\frac{\sigma^2R}{G}$$In the [[Galaxy cluster examples#Coma cluster|Coma cluster]] Zwicky measured velocity dispersions of $\sim 1000\,\pu{km s^{-1}}$ and inferred a mass. Then comparing that mass to that expected from the light (and realising our inferred mass from kinematics is much larger) Zwicky offered the following possible resolutions:
1.  stars in the Coma Cluster behave very differently than those in the local Milky Way (emitting much less light at equivalent mass) or
2.  the Coma Cluster is not in equilibrium or
3.  the laws of physics are different here and in the Coma Cluster or
4.  the Coma Cluster contains lots of additional mass which doesn't emit much light: ie **dark matter** exists

<mark class="hltr-pink">The bullet cluster</mark>
The [[Galaxy cluster examples#Bullet Cluster|bullet cluster]] is a smoking gun for an alternative massive and abundant species not coupled (in a detectable way currently) to electromagnetism. It is a system of galaxies which have passed through each other

- In observations of the hot X-ray gas, we find that the gas and stars (which interact with each other via some complicated effective cross section) have experienced a large degree of friction during the collision, and have slowed down and become largely disrupted
- We can also map the mass distribution of two galaxies which just passed through each other using [[Lensing#Weak lensing|weak lensing]], and what we find is that most of the mass is invisible, and has travelled further and become less disrupted than the gas. This suggests a species which interacts with baryons and itself weakly (so less friction, can constrain self-interaction cross section of dark matter via this measurement) and not with light.

Below are two views of the bullet cluster, the first a composite image of <mark class="hltr-blue">mass map</mark>  <mark class="hltr-red">x-ray emission</mark> and background galaxies used for the weak lensing analysis. the second shows explicitly the <mark class="hltr-green">mass contours</mark> obtained via weak lensing

![[bullet_nice.jpg]]
![[bullet_map.jpg]]


## 102
**What are the typical mass ranges of dwarf galaxies, normal galaxies, and galaxy clusters?**
The below (from Megan's notes) described the approximate mass ranges for [[Galaxies#Galaxy|galaxies]], [[Galaxy groups#Galaxy group|groups]] and [[Galaxy clusters#Galaxy cluster|clusters]]. 
![[galaxy_mass_scales.png]]

**Describe a few ways in which we measure the masses of these different types of systems.**
1. [[Galaxy clusters#Galaxy cluster|Galaxy clusters]]
   - [[Lensing#Weak lensing|Weak lensing]] for total mass measurements (can strong lensing also constrain mass?)
   - Scaling relations from X-ray measurements or SZ-effect measurements
   - Assume [[Stellar structure equations#Hydrostatic equilibrium|hydrostatic equilibrium]] of [[Cluster media#ICM|ICM]] and obtain mass from measurements of density and temperature (both from X-ray). If we have density why cant we get mass?

2. [[Galaxies#Galaxy|Galaxies]]
   - Rotation curves (see [[#101|Q101]])
   - [[Velocity dispersion#Velocity dispersion|Velocity dispersion]]
   - [[Velocity dispersion#Tully-Fisher relation|Tully-Fisher]] gives $L\propto v_r^4$ + assume $M/L$ ratio to get mass
   - [[Velocity dispersion#Faber-Jackson relation|Faber-Jackson]] gives $L\propto \sigma_r^4$ + as above
   - Dynamical masses obtained for example by [[Observatories#GAIA|GAIA]] [[Clustering#Globular Cluster|globular cluster]] motions.