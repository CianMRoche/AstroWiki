## Circular motion
Summary: For an object moving in a circle we have $$v = r\omega\quad,\quad a = \frac{v^2}{r}$$**Reason**:
The first follows from $$v = \frac{\text{distance}}{time} = \frac{2\pi r}{P} = r\omega$$The second from the fact that we can view the velocity vector as rotating with period $P$ on a circle of radius $v$ since the magnitude of $v$ never changes. Then the arc length traced in $dt$ is $a\,dt$ where $a$ is the acceleration required to change the direction of $v$ and simultaneously the arc length is $v\,d\theta$ with $\theta$ in radians. put those together and we get $a = v\omega = r\omega^2 = v^2/r$

**For gravity**
For a small thing of mass $m$ orbiting in a circle around an unmoving big thing of mass $M$ we have $$a_{cent} = \frac{v^2}{r} = a_{grav} = \frac{GM}{r^2}$$which leads to $$ v^2 = \frac{GM}{r}\quad \iff \quad w^2 = \frac{GM}{r^3}$$


## Kepler's laws
For one object in a binary:
1. The orbit is ellipse with center of mass at one focus
2. The line joining the focus and the object sweeps out equal areas in equal time $\frac{dA}{dt} = \frac{1}{2} r^2 \dot{\phi}$
3. $P^2\sim a^3$ where $P$ is period and $a$ is semi-major axis. In full its $$P^2 = \frac{4\pi^2 a^3}{G M_{tot}}$$Note that if you measure $P$ in years, $a$ in AU, and $M$ in solar masses, this reduces to (due to Earth following this law and the definition of an AU/year) $$P^2 = \frac{a^3}{M_{tot}} \simeq\frac{a^3}{M_{star}}$$so this is particularly simple in the solar system

Can also derive $r(\varphi)$ relationship for a Keplerian orbit
$$r = \frac{a(1-e^2)}{1+e\cos(\varphi)}$$


## Binary evolution
- stable mass transfer (to do with roche lobe and radius tradeoff)
- common envlope(?)
- dynamical formation, merging by collision (?) (for binary NS this is rare)


## Tidal migration
(Will use labels "planet" and "star" but in principle applies more widely).

When the tidal force on the planet creates a bulge and a torque that serves to reduce the semi-major axis of the orbit, especially near perihelion of highly-eccentric orbits.

**Why?**
The tidal bulges are not aligned between the two bodies (ie not along the same axis). This is because if the rotation period of the star is longer than the orbital period of the planet, the location of the bulge lags behind a line between the planet and the center of the star creating a torque between the planet and the star. As a result, the planet loses angular momentum and its semi-major axis decreases with time.


(See C+O ed. 2 pg 721)


## X-ray binary
A [[Neutron stars#Neutron stars|neutron star]] or [[Black holes#Black hole|black hole]] [[Accretion#Accretion disk|accreting]] from a companion (often a [[Spectra#Main sequence|main sequence]] star) and emitting strongly in the x-ray. Neutron stars are invisible in the optical so the x-ray lines are how we typically identify the accreting binary. 

- High mass companions accrete via stellar wind losses 
- Low mass companions accrete via [[Binaries#Roche-lobe overflow|Roche-lobe overflow]] (see also [[Compact objects - Questions#48|this question]])

![[xrb.jpg|400]]


## Cataclysmic variable
A [[Stellar classes#White dwarf|white dwarf]] accreting matter from a secondary star which irregularly increases in brightness by a large factor, then drops back down to a quiescent state. Not accreting enough mass to go over Chandrasekhar limit and go [[Supernovae#Supernova|supernova]].

**Typical parameters**
- Period of binary orbit $P\sim 20\,\pu{mins} - 5\,\pu{days}$ 
- Average WD mass $\sim 0.9\,M_\odot > 0.6\,M_\odot$ for isolated white dwarfs
- Companion star typically G [[Spectra#Harvard Spectral Classification|type]]

![[cataclysmic_variable.png|400]]


## Roche-lobe overflow
Related to [[Compact objects - Questions#48|48]].