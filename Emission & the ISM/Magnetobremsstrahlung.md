The magnetic counterpart to [[Bremsstrahlung#Bremsstrahlung|bremsstrahlung]]. 

Great summary and explanation [here](https://jila.colorado.edu/~pja/astr3730/lecture10.pdf). A highly detailed overview of all this in [this article](https://arxiv.org/pdf/1202.5949.pdf) (radiative processes in high energy astrophysics by Ghisellini)


## Larmor formula
Total power radiated by a nonrelativistic point charge as it accelerates. For a point charge $q$ accelerating with acceleration $a$ we have $$P = \frac{q^2a^2}{6\pi \epsilon_0 c^3}$$which is notably proportional to $a^2$. Note that the relativistic version is the same but replacing $a$ by the relativistic proper acceleration $\alpha$


## Cyclotron radiation
Electromagnetic radiation emitted by non-relativistic accelerating charged particles deflected by a magnetic field. The non-relativistic counterpart to [[#Synchrotron radiation]].

Much stronger emission from electrons than for heavier particles since power emitted $\propto 1/m^2$ (which is why highest energy particle accelerators are using protons and not electrons) which one can see from the [[#Larmor formula]] and the fact that for the Lorentz force $a\propto 1/m$.

**Cyclotron frequency**
- From [[Binaries#Circular motion|circular motion]] we have $v = r\omega_c$ and $a = v^2/r$ 
- From the Lorentz force we have $a = (q/m)vB$ 
- Put these together and we have $$\omega_c = \frac{v}{r} = \frac{qB}{m}$$and this $\omega$ is the *cyclotron frequency*. Note that $m$ here is the rest mass, often written $m_0$.

The spectrum then looks like a delta function at $\nu_c = qB/2\pi m$ but in reality we also see weak harmonics at integer multiples of this frequency. As a result, can be a great way to measure magnetic fields.
![[cyclotron_schematic.png|250]]


## Synchrotron radiation
Electromagnetic radiation emitted by relativistic accelerating charged particles deflected by a magnetic field. The relativistic counterpart to [[#Cyclotron radiation]]. 
![[synchrotron_diagram.png|500]]

A relativistically beamed dipole moving to the right looks like the following: 
![[dipole_relativistic.png]]

Relativistic effects are beaming and pulses are effectively shortened. Net effect is that the cyclotron spectrum for a single particle becomes (y axis is maybe logarithmic [[Units#Flux|specific flux]] but honestly hard to tell)
![[synchrotron.png|250]]

**Whyis it a spectrum and not a spike?**
(Formally it isnt a spectrum, but effectively it is; see link in heurostic derivation below). 
- The electric field at a detector from a cyclotron source (ignoring the high-frequency wiggles due to the electric field of individual photons) will be approximately sinusoidal. 
- Since the frequency spectrum goes as the fourier transform of the time signal, the FT will be a delta function (+ harmonics) as in [[#Cyclotron radiation]]. 
- The doppler beaming effectively turns the source into a flashlight (due to relativistic beaming, see image below) that points in the direction of motion of the particle, so our spectrum at the detector will look like a series of thinner peaks with a low continuum between. The timescale over which we can "see" the pulse is much smaller than the timescale of the rotation, due to beaming.
  ![[synchrotron_comb.png|300]]
- The FT of such a signal will be a series of broad spikes which are very close together, resulting in an effective spectrum.

**Heuristic derivation of single-particle spectrum** <mark class="hltr-pink">!UNFINISHED</mark>
For full derivation see Megan's notes (which are based on Chaudhuri pg 249) but I can't remember all that. Lots of details [here](https://www.cv.nrao.edu/~sransom/web/Ch5.html) too, Sec. 5.3 is very valuable for understanding this.

The only thing in the [[#Cyclotron radiation|cyclotron frequency]] $\omega_c = qB/m$ which would require "relativistic correction" is the mass, so we can postulate that the relevant frequency for synchrotron is $$\omega_s = \frac{qB}{\gamma m_0} = \frac{\omega_c}{\gamma}$$This is the frequency at which the charged particle gyrates. The opening angle of a cone in beaming goes as $\theta \sim 1/\gamma$. 
![[beaming.png|350]]


**Many particle spectrum**
The many-particle spectrum looks like the sum of many of the above
![[synchrotron2.jpg]]
This is a power law because we assume the underlying particle enegry distribution is a power law (as often happens in high energy astrophysics). The slope of this distribution can be derived in terms of the +slope of the energy distribution $f(\epsilon) \propto \epsilon^{-\beta}$ as $$\alpha = \frac{1}{2}(\beta - 1)$$where the $\alpha$ in the figure should have a minus sign.

In the optically thick regime, self-absorption (which occurs more at lower energies than higher) prevents radiation from escaping, meaning the low-energy end of the many-particle spectrum is strongly attenuated. 