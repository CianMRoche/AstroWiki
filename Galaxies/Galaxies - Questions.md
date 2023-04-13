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
Consider a single gravitational scatter. If the deflection of the trajectory of the star involves a change in momentum at least as large as the original momentum of the star ($v\sim \Delta v$), then we would regard it as a collision. Assume the timescale of collisions is the timescale for relaxation via this mechanism $\tau_{relax} = \tau_{coll}$. For this working definition and labelling the impact parameter of the collision as $b$ (as in [[Emission & the ISM - Questions#86|Q86]]) for two stars of mass $m$ $$\Delta p \sim F\Delta t \sim \frac{Gm^2}{b^2}\frac{b}{v}\sim mv \implies b\sim \frac{Gm}{v^2}$$For a number density of stars $n$, a mass per star $m$ and an effective cross section $\pi b^2$ the mean free path is $l \sim 1/\pi b^2 n$ such that the mean time between collisions for a star of velocity $v$ is $$\tau_{coll} = \frac{l}{v} = \frac{1}{\pi b^2 n v} \sim \frac{v^3}{\pi n G^2 m^2}$$Lets eliminate the density $n$ by evaluating $R$. If our system has $N$ total stars then via the virial theorem $$0 = 2\langle T\rangle + \langle U\rangle = Nm\left(\langle v^2\rangle -\frac{GM}{2R} \right) \implies R = \frac{G N m}{2\langle v^2 \rangle}$$though I dont know why theres a factor of 2 in the PE (comes from Xiaowei's notes).Then with $\langle v^2 \rangle = \sigma^2$ and and replacing $n = N / \frac{4}{3}\pi R^3$ we have $$\tau_{coll} \sim \frac{GN^2 m}{6\sigma ^3} \propto N^2$$For a [[Clustering|star cluster]] this number is $\sim 10 \,\pu{Gyr}$ (ie the age of the universe) and for a [[Galaxies#Galaxy|galaxy]] it is $\sim 10^{10}\,\pu{Gyr}$, ie impossible to explain relaxation of galaxies $\implies$ violent relaxation (see [[#113|Q113]]).

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

## 113
**What is a violent relaxation?**
A process by which a body relaxes/virializes via the changing of the gravitational potential, rather than via gravitational collisions. Most efficient way to relax the system as it is comparable to the [[Timescales#Dynamical timescale|free-fall time]]. 

Basic idea: If the potential is time-varying then particles can gain or lose energy on a timescale much faster than by collisions. The potential can be time-varying to to the growth and collapse of density fluctuations From Megan's notes: 
![[violent_relaxation.png]]

This leads to the spreading out of particle energy distributions. 

**How does the phase space distribution function it produces differ from that of an isothermal gas?**
For an [[Density profiles#Isothermal sphere|isothermal sphere]] the phase space distribution is Maxwell-Boltzmann, but for violently relaxed systems it is more uniform. 

**How does the timescale for violent relation compare to that for weak 2-body interactions?**
The timescale for violent relaxation can be approximated by considering the time derivative of the energy per unit mass where $d$ represents the convective derivative, since the change happens to a particle as it is moving (using that $\vec{a} = \dot{\vec{v}} = -\nabla\phi = \vec{F}/m$) $$\begin{align}
\epsilon &= \frac{1}{2}v^2 + \phi  \\
\frac{d\epsilon}{dt} &= -\,\vec{v}\cdot\nabla \phi\, + \,\frac{d\phi}{dt} \\
&= \frac{\partial\phi}{\partial t}
\end{align}$$Then to estimate a timescale for the changes, we would like to take an expectation value of something like $\epsilon/\dot{\epsilon}$ but since changes can be positive or negative, the expectation value will be about zero. A better way to find the timescale is then to get expectation values of the squared quantity (we could just take absolute values, but variances are usually defined in this way) and take the root after $$\tau_{\rm{vr}} = \left\langle \frac{\epsilon^2}{\left(\frac{d\epsilon}{dt}\right)^2} \right\rangle^{1/2} \sim \left\langle \frac{\phi^2}{\left(\frac{\partial \phi}{\partial t}\right)^2} \right\rangle^{1/2}$$Weak 2-body timescale goes as $\tau_{coll} \sim N/\ln N$ so why the above is smaller than that is not clear to me. [source](http://www.astro.yale.edu/vdbosch/lecture10.pdf)


## 114
**Why do some galaxies have prominent spiral structure and others do not?**
Try to explain existence with differential rotation, that is maybe pattern arises due to the roughly flat rotation curve ($v=\text{const}$) and thus $\omega \propto 1/r$. Then the timescale for rotation is $$\tau_{rot} = \frac{2\pi}{\omega} = \frac{2\pi r}{v} \sim 10^8\,\pu{yr}$$assuming $v=200\,\pu{km s^{-1}}$ and $r=10\,\pu{kpc}$ (note that Megan's notes use [[Binaries#Kepler's laws|Keplers third]] here but we get the same number). That is, the spiral arms will wind ~10s to 100s of times in the age of the universe. In such a case, we should not see prevalent structure, as it would all be washed out by many rotations(the so-called "winding problem").

**Briefly describe the density wave theory of spiral structure?**
The idea is that there are density waves which propagate around the disk, like a sound wave in air, and that: 
- The stars experience roughly no net motion due to the passage of the wave (which contains different stars at any point in time except for the stars at a certain radius such that their angular velocity coincides with the angular velocity of the wave, $\Omega_{gp}$ below).
- The density wave increases the density of gas and thus boosts star formation rates, explaining why we see star formation mostly within spiral arms

![[spiral_arms.png]]


## 115
**How many globular clusters does our Galaxy contain? How are they distributed in space? What fraction of the total mass of the Galaxy do they contain?**
The [[Milky Way#Milky Way|Milky Way]] contains $\gtrsim 150$ [[Clustering#Globular Cluster|globular clusters]] 
- Distributed roughly isotropically in the stellar halo (i.e. not in the disk), but potentially an oblate/flattened distribution rather than perfectly isotropic
- Most contained within $\sim 40\,\pu{kpc}$ of the galactic center
- They make up about 1% of the stellar mass of the Milky Way


## 116
**A globular cluster at a distance of 10 kpc, containing 10$^6$ stars, subtends an angle of 1/3 arcminute. Estimate the velocity dispersion among its stars.**
Assuming [[Binaries#Circular motion|circular motion]] of the stars in the cluster, the [[Velocity dispersion#Velocity dispersion|velocity dispersion]] is $$\sigma = \sqrt{\frac{2GM}{3R}}$$We can estimate the mass as $10^6\,M_\odot$ by assuming the mean mass is a solar mass, and to get the radius we use the definition of the [[Units#Arcminute|arcmin]] and the [[Units#parsec|parsec]] and simply get $R = d\,\theta \simeq 1\,\pu{pc}$ resulting in $\sigma \simeq 50\,\pu{km s^{-1}}$ 


## 117
**What are the Oort A and B coefficients and what basic information about the Galaxy can be determined from them?**
By assuming all the stars in the [[The Sun#The Sun|solar]] neighborhood are on circular orbits and that the Milky Way has an axisymmetric potential, one can use measurements of the speeds of stars near the Sun to infer information about the Sun's orbit around the Milky Way (really the mean motion of the "local standard of rest" which is the collection of objects within $\sim 100\,\pu{pc}$ of the Sun), and furthermore obtain information about the circular and noncircular components of the motion of stars in the solar neighborhood. One can also use knowledge of them to infer distances to objects if their kinematics are known.

The constants are defined as $$
A =\frac{1}{2}\left(\frac{V_0}{R_0}-\left.\frac{d v}{d r}\right|_{R_0}\right)\quad ,\quad 
B =-\frac{1}{2}\left(\frac{V_0}{R_0}+\left.\frac{d v}{d r}\right|_{R_0}\right)
$$where $V_0$ and $R_0$ are the rotational velocity and distance to the galactic center measured at the position of the Sun, and $v$ and $r$ are the velocities and distances of stars at other positions in the solar neighborhood. With these parameters one

![[Oort_constants_derivation_diagram.jpg]]

**What are the four types of observations that go into constraining these coefficients, and how precisely are each measured by current technology.**

We can rewrite the coefficients as $$
A  =\frac{V_{\text {obs }, \mathrm{r}}}{d \sin (2 l)}\quad ,\quad 
B  =\frac{V_{\text {obs }, \mathrm{t}}}{d}-A \cos (2 l)
$$for an observation of a star with Galactic longitude $l$ at a distance $d$ from the Sun, with tangential and radial velocity components $V_{\rm{obs,t}}$ and $V_{\rm{obs,r}}$ as measured at the solar position (we assume circular orbits so $V_{\rm{obs,r}}$ would be zero if we measured with respect to the galactic center). Thus the observables necessary to determine the coefficients are:

1. Radial velocity - stellar spectra ([[Observatories#GAIA|GAIA]] DR3 has 33 million radial velocities)
2. On-sky velocity - proper motions from GAIA
3. Distances - Use GAIA parallaxes
4. Galactic longitude (not hard, GAIA works again)


## 118
**Define the following simple "laws" and "profiles" and for what galaxy component or galaxy type each is most relevant. Describe where observational data deviates from these idealized profiles.**

| Name | Form | Notes | Use |
| --- | ----------- | -------------| -------------|
| Sersic |  $I(r) = I_0 e^{-(r/r_0)^{1/n}}$ | $I_0$ is central surface brightness, $r_0$ is scale length and $n$ is the "Sersic index". Note for $n=1$ we recover exponential, and $n=4$ we recover de Vaucouleurs | Models the [[Units#Intensity\|surface brightness]] profiles of [[Galaxies#Galaxy\|galaxies]] |
| de Vaucouleurs | $I(r) = I_0 e^{-(r/r_0)^{1/4}}$ | Sersic with $n=4$ | Models the [[Units#Intensity\|surface brightness]] of an elliptical galaxy, or the galactic bulge of a disk galaxy |
| Exponential | $I(r) = I_0 e^{-(r/r_0)}$ | Sersic with $n=1$ | Models the [[Units#Intensity\|surface brightness]] of a spiral/disk galaxy, but deviations common due to spiral structure and existence of bulge|
| Einasto | $\rho(r) = \rho_s \exp\left[-\frac{2}{\alpha} \left(\frac{r}{r_s}\right)^\alpha \right]$ | Does not exhibit a divergent central density. People define in different ways, $r_s$ is a scale radius. [Source](https://cluster-toolkit.readthedocs.io/en/latest/source/density_profiles.html) | [[Density profiles\|Density profile]] of halos in [[Dark matter\|CDM]] |
| NFW | $\rho(r)=\frac{\rho_0}{\frac{r}{R_s}\left(1+\frac{r}{R_s}\right)^2}$ | Exhibits a divergent central density, goes as $r^{-1}$ toward $r=0$ and $r^{-3}$ toward $r\rightarrow \infty$. Also does not have a well-defined total mass. Shows up in simulations with this cuspy central region shape, but core/cusp problem appears with observational data (see [[#125\|Q125]]) | [[Density profiles\|Density profile]] of halos in [[Dark matter\|CDM]] |


## 119
**What is "Press-Schechter theory" and why is it wrong?**

This is the theory that the probability of a galaxy having a mass $>M$ is directly related to the probability of having an early universe overdensity with $\delta > \delta_{crit}$ and thus connecting early universe fluctuations visible on the CMB to the mass function of low redshift [[Galaxies#Galaxy|galaxies]]. The overdensity $\delta$ is defined in terms of the density $\rho$ and average density $\bar{\rho}$ by $$\delta = \frac{\rho - \bar{\rho}}{\bar{\rho}}$$and the critical overdensity $\delta_{crit}\simeq 1.68$ comes from (havent done cosmology section yet!UNFINISHED). Essentially $P(>M) = P(\delta > \delta_{crit}|\text{ smoothing scale })$ where the smoothing scale determines the minimum mass scale of halos we are considering (this is why we calculate a probability of having a mass $M$ or greater). Since the scale is a function of the minimum mass we're looking at, we typically write $$P(>M) = P(\delta > \delta_{crit}|M)$$
![[press_schechter_theory.png]]

Start with Gaussian random fluctuations in the early universe, and the smoothing scale enters as the width of the Gaussian noise $\sigma_M \propto M^{\frac{1}{6}(n+3)}$ ... I dont understand where a lot of this comes from !UNFINISHED

**Why is it wrong?**
In fact $P(>M) = 2P(\delta > \delta_{crit}|M)$. Why is there a factor of two? Look at an underdensity within an overdense region at some mass scale.
![[PS_underdensity.png|300]]

PS formalism would say that these objects are not part of a halo with mass > M. But, at a different scale M, they may be pulled up to be includedso there’s inconsistency. Another way to look at it is that once things go nonlinear, the collapse is able to draw matter in from less dense regions, hence much of the mass does end up in the overdense regions, albeit a different M.


## 120
**What is "biased galaxy formation"?**
Refers to the fact that galaxies are not perfect tracers of mass in the universe. Why would this be so?
- Baryonic physics different than that of the mass-dominant [[Dark matter]]
- Lack of good understanding of galaxy formation

The "bias" refers to some metric of the difference between the galaxy distribution and that of all matter. Bias sometimes used in the context of the linear bias model, where, on scales larger than a few megaparsecs, the galaxy density fluctuations are enhanced over those of the mass by a factor $b$, the linear bias factor $$\frac{\delta n_g}{\bar{n}_g}=b\left(\frac{\delta \rho}{\rho}\right)$$where $n_g$ is the number density of galaxies and $\rho$ is the mass density. Many groups have found that the halos formed in dark matter simulations are actually antibiased with respect to the mass, (i.e. the fluctuations in galaxy number density are smaller than that of mass $b < 1$), because of excessive merging of halos compared with real galaxies, giving for example some very large halos. But at the same time [[CMB#CMB|CMB]] measurements have yielded a very different $b \simeq 1.5$ with the opposite conclusion, ie that galaxies are more tightly clustered (higher number overdensities) than all mass.

Observationally, we can look at the galaxy-galaxy 2-point correlation function (see [[#122|Q122]]), ie "if we have a galaxy at $\vec{x}$ then what is the probability of finding a galaxy at $\vec{x} + \vec{r}$ ?". Can do such a thing with [[Catalogs#SDSS|SDSS]] for example.


## 121
**What fractions of each of the following is composed of "dark matter"? How are each of these estimates arrived at?**

**(i) The solar neighborhood**  |  $f_{DM} \lesssim 20\%$
Within the [[Milky Way#Milky Way|MW]] disk (and therefore in the [[The Sun#The Sun|Solar]] neighborhood), we expect to find little [[Dark matter]] since DM is not thought to be dissipative, and therefore will not collapse into a disk like baryons do. the number quoted above is estimated based on [[Observatories#GAIA|GAIA]] stellar kinematics ([source](https://arxiv.org/pdf/1711.03103.pdf) from Katelin Schutz, former MIT student).

**(ii) A typical galaxy like the Milky Way**  |  $f_{DM} \simeq 90-95\%$
From something like [[#101|rotation curves]] or [[Velocity dispersion#Velocity dispersion|velocity dispersions]] can infer a total DM mass. Can then estimate the DM and stellar contributions from a mass to light ratio or knowledge of stellar evolution (basically adding up all the stars masses via their light).

**(iii) A typical galaxy cluster like the Coma cluster**  |  $f_{DM} \simeq 90\%$
Total mass of cluster can be estimated from [[Lensing#Weak lensing|weak lensing]] or scaling relations like the fact that the net result of the SZ-effect (basically [[Scattering#Inverse-Compton scattering|inverse Compton scattering]]) is proportional to cluster mass. Can also estimate baryonic contributions using the [[Spectra#The electromagnetic spectrum|X-ray]] emission of the [[Cluster media#ICM|ICM]] assuming models for that emission. [[Velocity dispersion#Velocity dispersion|Velocity dispersions]] also work, as originally done by Zwicky in 1930s for the [[Galaxy cluster examples#Coma cluster|Coma cluster]]. 

**(iv) The universe**  |   $f_{DM} \simeq 83\%$
Constraints from [[Power spectrum]] of the [[CMB#CMB|CMB]], [[balmer_fraction.png#BAO|BAO]](?) and from [[BBN#BBN|BBN]] can give relative abundances of dark matter and baryonic matter $\Omega_m$ and $\Omega_b$ (?) !UNFINISHED come back to after cosmology


## 122
**What is the galaxy correlation function?**
Answers the question "if we have a galaxy at $\vec{x}$ then what is the probability of finding a galaxy at $\vec{x} + \vec{r}$ ?". Defined as $$\langle\rho(\vec{x})\rho(\vec{x}+\vec{r})\rangle = \bar{\rho}^2\langle1+\underbrace{\delta(\vec{x})\delta(\vec{x}+\vec{r})}_{\xi(\vec{r}) := \langle \delta(\vec{x})\delta(\vec{x}+\vec{r}) \rangle}\rangle$$for $\rho$ the mass density, $\delta$ the overdensity (defined in [[#119|Q119]]) and bars and angular brackets meaning averages and integrals over space, respectively. Tthe chosen scale $\vec{r}$ tells us aboout correlations across a specific length scale, leading to interesting inferences like measurements of [[BAO#BAO|BAO]]. 

How do we measure this? Via [[Galaxies#Galaxy|galaxy]] surveys (eg [[Catalogs#eBOSS|eBOSS]]).

**How do the correlation functions of galaxies and clusters of galaxies differ?**
Measurements suggest that$$\xi(\vec{r}) \simeq \left(\frac{|\vec{r}|}{r_0}\right)^\gamma$$ie a power law, and that for [[Galaxies#Galaxy|galaxies]] a good fit is given by $$\gamma = 1.7 \quad, \quad r_0 = 5\,\pu{Mpc}$$such on all scales (still for galaxies) the function looks like:
![[2_point_corr.png]]

For [[Galaxy clusters#Galaxy cluster|clusters]] of galaxies (ie treating a cluster as "one object" and getting the 2-point correlation for such objects) it has been found that the best fit is at $$\gamma = 2.1 \quad, \quad r_0 = 17\,\pu{Mpc}$$but critically, <mark class="hltr-pink">clusters are found to be much more strongly correlated in space than galaxies</mark> with $\xi_{cluster} \simeq 20 \xi_{gal}$, effectively representing the large-scale sctructure of the universe (modulo [[#120|galaxy bias]], which is less biased for clusters than for individual galaxies).

**How is the galaxy correlation function used to constrain H$_0$?**
If we measure the angular size of the [[BAO#BAO|BAO]] peak in a narrow range of [[Spectra#Redshift|redshifts]] (ie at roughly the same distance) then we can constrain $H_0$ using other parameters from [[CMB#CMB|CMB]] studies. The reason for this is that the BAO scale is comoving with the Hubble flow, therefore if we measure the angular size, using the expression for the [[Distances#Angular diameter distance|Angular diameter distance]] is given by !UNFINISHED (come back after cosmology)

BAO is a standard ruler in a similar way to the "standard candles" of type-1a [[Supernovae#Supernova|supernovae]]


## 123
**What are “active galactic nuclei”?**
See [[AGN#AGN|AGN]].

**What is the “unified model of AGN”, and how does it explain the variety of AGN that are observed?**
Explains the large differences seen in spectra between AGN when viewed form different lines of sight (Type 1 and 2). Also explains [[AGN#Blazar|blazars]] and "BL Lac"  objects, which are rapidly varying blazars, as AGN for which we look directly at the jet along the line of sight. Strongly 

![[agn_schematic.png]]

A table of the things that are "unified" in this picture is 

![[agn_unification.png]]

**How and when are AGN important for galaxy evolution?**
As mentioned in [[#108|Q108]] it inhibits star formation in large galaxies by heating the gas and preventing collapse.


## 124
**Describe the following relations and what they are useful for:**
**(i) Kennicutt-Schmidt**
The statement that the mass column density (mass per area) for star formation (rate?) depends on the mass column density of gas as $$\Sigma_{SFR} \propto (\Sigma_{gas})^n$$but apparently the LHS is also per unit time? This one is a mess. $n$ measured to be $2\pm 1$ ?

**(ii) M-sigma relation**
See [[Velocity dispersion#M-sigma relation|M-sigma relation]]. 

**(iii) the Madau plot**
Describes the cosmic evolution of the average star formation rate. 
- Cosmic star formation peaks at around $z\simeq 2$. (Is this cosmic noon?). This is also when the number density of [[AGN#Quasar|quasars]] appears to peak, inferring connection between galaxy and AGN evolutions like [[Velocity dispersion#M-sigma relation|M-sigma]]. 
- Suggests that many metals formed early during the deaths of massive stars, corroboarted by [[Galaxy clusters#Galaxy cluster|cluster]] [[Cluster media#ICM|ICM]] measurements.
![[madau.jpg|400]]
**(iv) the star-forming main sequence**
Star formation rate correlates with the stellar mass of a galaxy. Suggests that galaxies spend much of their lifetime building up stars in a self-regulated way. Seen across all broad classes of galaxy

![[sf_main_seq.png]]

## 125
**Describe the following galaxy-formation problems. Which of these are solved? What are their solutions?**
**(i) the missing satellite problem**
We dont see as many small satellite [[Galaxies#Galaxy|galaxies]] as predicted by CDM simulations. Interpretation could be that smallest DM halos are inefficient at forming stars, so they exist but we dont see them.

![[MSP.png|500]]
Resolution?
- recently deep surveys ([[Catalogs#SDSS|SDSS]]) have found many more extremely faint dwarf galaxies (raising up the observations above)
- [[Observatories#LSST|LSST]] is forecasted to improve this further
- What remains is the question "what is suppressing star formation in small halos?". Feedback?

**(ii) the core-cusp problem**
CDM and simulations predict a sharply rising density profile near the cores of halos ("cusp"), but observations show a cored (flatter) density profile near the centers of halos.

![[core_cusp.png|400]]
Resolution?
- Feedback: can remove matter from the core
- Warm or self-interacting [[Dark matter|DM]]
- MOND 😍

**(iii) the cooling flow problem**
Mass cooling rates from [[Spectra#The electromagnetic spectrum|X-ray]] measurements of the [[Cluster media#ICM|ICM]] suggest that gas should be cooling  
and forming stars at rates of $\sim 100-1000\, M_\odot\,\pu{yr^{-1}}$ yet we observe star formation rates on the  
order of ~1% of these rates in cluster cores (and not enough cool gas either to account for the  
difference via "it happened in the past").

Resolution?
- [[[AGN#AGN|AGN]] feedback heats up the gas and prevents star formation, but the details of how the jets deposit energy into the cluster are unclear.