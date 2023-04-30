The magnetic counterpart to [[Bremsstrahlung#Bremsstrahlung|bremsstrahlung]]. 

Great summary and explanation [here](https://jila.colorado.edu/~pja/astr3730/lecture10.pdf). A highly detailed overview of all this in [this article](https://arxiv.org/pdf/1202.5949.pdf) (radiative processes in high energy astrophysics by Ghisellini)

## Synchrotron radiation
Electromagnetic radiation emitted by relativistic accelerating charged particles deflected by a magnetic field. The relativistic counterpart to [[#Cyclotron radiation]]. A relativistically beamed dipole moving to the right looks like the following: 
![[dipole_relativistic.png]]

Relativistic effects are beaming and pulses are effectively shortened. Net effect is that the cyclotron spectrum for a single particle becomes (y axis is maybe logarithmic [[Units#Flux|specific flux]] but honestly hard to tell)
![[synchrotron.png|250]]

**Why does the spectrum become a spectrum and not a spike?**
The electric field at a detector from a cyclotron source (ignoring the high-frequency wiggles due to the electric field of individual photons) will be approximately sinusoidal. Since the frequency spectrum goes as the fourier transform of the time signal, the FT will be a delta function (+ harmonics) as in [[#Cyclotron radiation]]. The doppler beaming effectively turns the source into a flashlight (due to relativistic beaming) that points in the direction of motion of the particle, so our spectrum at the detector will look like a series of thinner peaks with a low continuum between. The FT of such a signal is very broad. (Note its not a Dirac comb, whose FT is a Dirac comb again, rather it looks like a train of Lorentzians or similar).

**Why does the single-particle spectrum have a break? (very unfinished note)** 
Could be for many reasons(?): Can get a broken spectrum either by 
1. Injecting a broken power law of light? 
2. The distribution of electron energies being a power law. Why not a Maxwell-Boltzmann distribution or similar? These plasmas where sychrotron is important (extremely high energies) are often non-collisional relative to the emission (that is the collision timescale is much longer than the synchrotron timescales) and thus nonthermal. The reason you get a power law is that in these plasmas you get lots of "Fermi-type" acceleration mechanisms, in which the particles gain energy through some interactions (for example, for crossing a shockwave). It can be shown (it's somewhere in Rybicki and Lightman for example) that the energy gain is proportional to the particle's energy so it kind of adds up multiplicatively - the more energy a particle has, the more it's going to receive each time it is accelerated. Eventually it all adds up to a power-law distribution in energy.

**Many particle spectrum**
The many-particle spectrum looks like the sum of many of the above
![[synchrotron2.jpg]]
In the optically thick regime, self-absorption (which occurs more at lower energies than higher) prevents radiation from escaping, meaning the low-energy end of the many-particle spectrum is strongly attenuated. 


## Cyclotron radiation
Electromagnetic radiation emitted by non-relativistic accelerating charged particles deflected by a magnetic field. The non-relativistic counterpart to [[#Synchrotron radiation]].

Much stronger emission from electrons than for heavier particles since power emitted $\propto 1/m^2$ (which is why highest energy particle accelerators are using protons and not electrons).

The name contains "cycle" because it is derived by considering a charged particle in circular motion with a certain frequency due to a uniform magnetic field. The spectrum then looks like a delta function at $\nu = qB/2\pi m c$ (might be in CGS units?) but in reality we also see weak harmonics at integer multiples of this frequency. As a result, can be a great way to measure magnetic fields.
![[cyclotron_schematic.png|250]]


## Larmor formula
Total power radiated by a nonrelativistic point charge as it accelerates. For a point charge $q$ accelerating with acceleration $a$ we have $$P = \frac{q^2a^2}{6\pi \epsilon_0 c^3}$$which is notably proportional to $a^2$. Note that the relativistic version is the same but replacing $a$ by the relativistic proper acceleration $\alpha$