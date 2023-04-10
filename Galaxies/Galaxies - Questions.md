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
   - Scaling relations from X-ray measurements (see Geoffrey's notes 165) or SZ-effect measurements
   - Assume [[Stellar structure equations#Hydrostatic equilibrium|hydrostatic equilibrium]] of [[Cluster media#ICM|ICM]] and obtain mass from measurements of density and temperature (both from X-ray). If we have density why cant we get mass?

2. [[Galaxies#Galaxy|Galaxies]]
   - Rotation curves (see [[#101|Q101]])
   - [[Velocity dispersion#Velocity dispersion|Velocity dispersion]]
   - [[Velocity dispersion#Tully-Fisher relation|Tully-Fisher]] gives $L\propto v_r^4$ + assume $M/L$ ratio to get mass
   - [[Velocity dispersion#Faber-Jackson relation|Faber-Jackson]] gives $L\propto \sigma_r^4$ + as above
   - Dynamical masses obtained for example by [[Observatories#GAIA|GAIA]] [[Clustering#Globular Cluster|globular cluster]] motions.


## 103
**Sketch the rotation curve of our Galaxy, with approximate scales on the axes.**
See [[#101|Q101]]. 

**How can information about the rotation curve be determined from 21 cm observations?**
Can do the following within the radius of Earth's orbit ($\sim 8\,\pu{kpc}$). Make observations of the [[Spectra#21cm line|21cm line]] in some direction. In a situation where we have multiple disconnected clouds of neutral Hydrogen along that line of sight, each on a $\sim$ circular orbit, the signal we see will be Doppler shifted to various degrees depending on the relative velocity with Earth. If all are moving with the same speed, then the Doppler shift will be largest for the cloud whose velocity points directly toward Earth, ie the one whose orbit is tangent to our chosen line of sight ("B" below). Note that if they arent moving with the same speed, I dont know how this works. Maybe it works for any galactocentric radius range over which the circular velocity profile monotonically decreases, making the bulge problematic.

![[21cm_rotation_curves.png]]

Once we've measured and identified that velocity $v_B$ we know it is the full speed, and so via [[Binaries#Kepler's laws|Kepler's third law]] (assuming a circular orbit, or equivalently just [[Binaries#Circular motion|circular motion with gravity]]) we have $$r = \frac{GM}{v^2}$$This measurement is hard to make toward the galactic center because of galactic bulge, reason unclear.


## 104
**What is the density profile of a self-gravitating isothermal gas sphere? What is the corresponding rotation curve for this system?**

See [[Density profiles#Isothermal sphere|Isothermal sphere]] for the derivation of $$\rho(r) = \frac{\sigma^2}{2\pi G r^2}$$where $\sigma$ is the [[Velocity dispersion#Velocity dispersion|velocity dispersion]]. To calculate the shape of the rotation curve, assume [[Binaries#Circular motion|circular motion]] such that $$ v = \sqrt{\frac{GM_r}{r}}$$Calculating $M_r$ from [[Stellar structure equations#Mass continuity|mass continuity]] we see $$M_r = \int_0^r dr\, 4\pi r^2 \rho = \frac{2\sigma^2 r}{G}$$and this results in $$v = \sqrt{2} \sigma$$That is, a <mark class="hltr-pink">flat rotation curve</mark> which arises since $M_r\propto r$. 


## 105
**What is two-body relaxation?**
The ”relaxation” of stars is the process deflecting the individual trajectories of stars from the one they would have if the distribution of matter was perfectly smooth. The ”2-body relaxation” is induced by the individual star-star interactions, while the ”violent relaxation” is induced by a large collective variation of the stellar system shape (see [[#113|Q113]]).

**For a self-gravitating cluster of N objects, each of mass m, with a velocity dispersion $\sigma$, what is the relaxation time?**
Consider a single gravitational scatter. If the deflection of the trajectory of the star involves a change in momentum at least as large as the original momentum of the star ($v\sim \Delta v$), then we would regard it as a collision. Assume the timescale of collisions is the timescale for relaxation via this mechanism $\tau_{relax} = \tau_{coll}$. For this working definition and labelling the impact parameter of the collision as $b$ (as in [[Emission & the ISM - Questions#86|Q86]]) for two stars of mass $m$ $$\Delta p \sim F\Delta t \sim \frac{Gm^2}{b^2}\frac{b}{v}\sim mv \implies b\sim \frac{Gm}{v^2}$$For a number density of stars $n$ and an effective cross section $\pi b^2$ the mean free path is $l \sim 1/\pi b^2 n$ such that the mean time between collisions for a star of velocity $v$ is $$\tau_{coll} = \frac{l}{v} = \frac{1}{\pi b^2 n v} \sim \frac{v^3}{\pi n G^2 m^2}$$Lets eliminate the density $n$ by evaluating $R$. If our system has $N$ total stars then via the virial theorem $$0 = 2\langle T\rangle + \langle U\rangle = Nm\left(\langle v^2\rangle -\frac{GM}{2R} \right) \implies R = \frac{G N m}{2\langle v^2 \rangle}$$Then with $\langle v^2 \rangle = \sigma^2$ and and replacing $n = N / \frac{4}{3}\pi R^3$ we have $$\tau_{coll} \sim \frac{GN^2 m}{6\sigma ^3} \propto N^2$$For a [[Clustering|star cluster]] this number is $\sim 10 \,\pu{Gyr}$ (ie the age of the universe) and for a [[Galaxies#Galaxy|galaxy]] it is $\sim 10^{10}\,\pu{Gyr}$, ie impossible to explain relaxation of galaxies $\implies$ violent relaxation (see [[#113|Q113]]).

**How long does it take for a massive object (M>> m) to sink to the bottom of a cluster potential well?**
Using the expression for $R$ we also have that the [[Timescales#Dynamical timescale|dynamical timescale]] is $$\tau_{ff} \sim \frac{1}{\sqrt{G\rho}} \sim \frac{GNm}{\sigma^3} \propto N$$Since the free-fall timescale is a factor of $N$ smaller than the collisional timescale, objects sink into the potential well effectively without collisions when $N$ is large. The sinking timescale is thus simply $\tau_{ff}$.

**Bonus**
It may be that a large number of smaller collisions with $\Delta v \ll v$ are in fact responsible for relaxation rather than single large collisions (seems more reasonable). Sum up many small interactions over a random walks and end up with $\tau_{coll}\sim N^2/\ln N$ which is closer to the free fall timescale.


## 106
**What is the "Local Group"?**
See [[Galaxy groups#Local Group|Local group]].


## 107
**What is the morphology-density relation for galaxies? Give several possible explanations for this trend.**

Basic idea is that 
- Elliptical [[Galaxies#Galaxy|galaxies]] are more likely to be found in denser environments like [[Galaxy groups#Galaxy group|groups]] and [[Galaxy clusters#Galaxy cluster|clusters]] 
- Conversely, spiral galaxies are more likely to be found in less dense environments like the field

Illustrated below, where $S0$ is another name for "lenticular" [[Galaxies#Galaxy|galaxy]].

![[morphology_density.png|400]]

Potential explanations:
- Denser environments lead to more mergers, disrupting spiral structure
- Gas more easily stripped in these environments due to [[Definitions - The Solar System#Ram pressure|ram pressure]] and ellipticals and lenticulars are gas-poor relative to spirals. 


## 108
**What is the "Schechter luminosity function"? What is the luminosity of a typical bright galaxy?**
Empirical relationship to describe the observed galaxy luminosity function (distribution of number of galaxies over luminosities). $$\Phi(L) = \frac{\Phi_*}{L_*}\left(\frac{L}{L_*}\right)^\alpha e^{L/L_*}$$where $\Phi(L)$ has dimensions "per volume per luminosity" such that $\Phi(L) dL$ is the number of galaxies with luminosity between $L$ and $L+dL$ per unit volume. Bbserved best-fit numbers $$\cases{\alpha \simeq 1.1 \\ L_* \simeq 10^{10}\,L_\odot \sim \text{MW luminosity} \\\Phi_* \simeq 0.02\,\pu{Mpc^{-3}}}$$The function has the following shape (from Megan's notes):
![[shechter.png|300]]

and a typical galaxy has a luminosity like that of the [[Milky Way#Milky Way|Milky Way]] ($\sim 2\times 10^{11} L_\odot$ ). We see few galaxies far above this luminosity because theyre rare, and few far below because theyre faint.

**How does the luminosity function of galaxies compare to the mass function of halos from simulations?**
Observations compare in the following way to our expectations from simulations (effort is put into addressing this in sims by adjusting feedback and baryonic physics models)
![[schechter_function_comparison.png]]

Take-home is smaller galaxies cant form as many stars by the disruption of gas due to [[Supernovae#Supernova|supernovae]] and larger galaxies cant due to heating from [[AGN#AGN|AGN]] feedback.


## 109
**Describe Hubble's classification scheme for galaxies and explain why it is useful.**

A classification scheme that separates ellipticals from barred and non-barred spirals. The letter subclasses in spirals S and barred galaxies SB refer to how tightly wound the spiral arms are. S0 refers to lenticular [[Galaxies#Galaxy|galaxies]]. 
![[Hubble_classification.png]]

Another view with some galaxy images
![[Hubble_Tuning_Fork_diagram.svg]]

Usefulness: Captures some trends in galaxy populations, such as: 
- **Support**:
  Ellipticals tend to be supported pressure-supported with random motions, but spirals tend to be rotation-supported (ie more net angular momentum).
- **Brightness profiles**:
  Spirals are exponential, but ellipticals are de Vaucoleurs (see [[#118|Q118]])
- **Age**:
  Spirals are young(ish) and ellipticals are old ("Pop 2")
- **Stellar motion**:
  Spirals fit [[Velocity dispersion#Tully-Fisher relation|TF-relation]] and ellipticals fit [[Velocity dispersion#Faber-Jackson relation|FJ-relation]]
  
Not an evolutionary sequence as Hubble once thought.


## 110
**What is the "Tully-Fisher relation"? Derive this relation beginning with the virial theorem and
using simplifying assumptions about galaxies.**

See [[Velocity dispersion#Tully-Fisher relation|Tully-Fisher relation]].

**How can this relation be used to determine H0?**
Measuring the [[Hubble constant#Hubble constant|Hubble constant]] $H_0$ requires both distances and recessional velocities. Velocities follow easily from redshifts. Tully-Fisher allows us to determine intrinsic luminosities from [[Spectra|spectral]] line widths, and therefore distances to the object. 


## 111
**What are cD galaxies and where are they found? How might they be formed?**
Another name for a [[Galaxy clusters#Brightest cluster galaxy|BCG]]. "c" refers to very large and "D" refers to diffuse. "Central dominant" is a backronym. Formed via mergers and dynamical friction.


## 112
**What is the “Faber-Jackson relation” for elliptical galaxies?**

The [[Velocity dispersion#Faber-Jackson relation|Faber-Jackson relation]] is a connection between the velocity dispersion of elliptical [[Galaxies#Galaxy|galaxies]] and their luminosity. Analogue to [[Velocity dispersion#Tully-Fisher relation|Tully-Fisher]] but for elliptical galaxies. I dont see how its different. !UNFINISHED

**How is this different than the "fundamental plane" for elliptical galaxies?**
Large scatter in the Faber-Jackson relationship for different types of population lead to the development of the "fundamental plane" which incorporates a 3rd independent parameter $R_e$ called the "effective radius". FJ is then a projection of this relationship down the $R_e$ axis.

Defined by $$L^\alpha R_e^\beta \sigma^\gamma = \text{const}$$