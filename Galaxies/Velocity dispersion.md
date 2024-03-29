
## Velocity dispersion
A series of relationships derived from the virial theorem, relating velocity dispersion to the mass of the system. In the simplest case, the relation looks something like $$M = \frac{v^2r}{G} \simeq \frac{3}{2}\frac{\sigma^2R}{G}$$where $\sigma$ is the 1D velocity dispersion (radial typically) we can actually measure. This applies to systems that are approximately isotropic, that is a disked galaxy with a net rotation wont have $v\sim \sigma$ since the distribution will be bimodal. In such a case one would be better off using the dispersion of $|\vec{v}|$ to infer the rotational velocity, or just use $v_{circ}$ explicitly. Relationship reliable up to an order $\sim 1-10$ factor

**Derivation**
The speeds of the objects in the galaxy have two components
1. The center of mass motion of the whole cluster of objects
2. The relative motion within the cluster of objects

Thus if we measure the speeds of many objects, we should see a mean speed (corresponding to the center of mass motion) and some slower, some faster, corresponding to the relative motion within that object. Lets pretend that shape is a Gaussian, then the standard deviation of that Gaussian describes the speed of a typical star within that cluster (without considering the net motion of the cluster). 

The virial theorem $\langle T\rangle = -\frac{1}{2} \langle U\rangle$ for a gravitational system says that for a star of mass $m$, speed $v$ and distance $r$ from the center of a spherical mass distribution of mass $M$ we have $$\frac{1}{2}mv^2 \simeq \frac{1}{2}\frac{GMm}{r}$$Lets estimate $v$ and $r$ :
- If the system is isotropic then $\sigma_x = \sigma_y = \sigma_z$ and the total velocity dispersion is $\sigma_{\rm{3D}} = \sqrt{\sigma_x^2 + \sigma_y^2 + \sigma_z^2} = \sqrt{3}\,\sigma_{\rm{1D}}$. Note that if we make an observation, we really measure a 1-dimensional dispersion (toward us and away from us, denoted $\sigma_r$ for radial). A good estimate for the 3D speed of a star is then $v^2 \simeq 3\sigma_r^2$. 
- A reasonable estimate for the radial location of the average star is $r\simeq R/2$ 

Putting these estimates into the virial theorem and rearranging, we have $$M = \frac{v^2r}{G} \simeq \frac{3}{2}\frac{\sigma^2R}{G}$$This result however is only valid up to an order $\sim 1-10$ factor.


## M-sigma relation
A mass-velocity dispersion relation between the mass of [[Black holes#Black hole|supermassive black holes]] and the speeds of stars in the [[Galaxies#Galaxy|galactic]] bulge. One version was called "the [[#Faber-Jackson relation]] for black holes". Relationship is $$M\propto \sigma^n$$and measurements place $n$ at about 5 (originally thought to be closer to 4). Summarized as $$\frac{M}{M_\odot} \simeq2\times 10^8 \left(\frac{\sigma}{200\,\pu{km s^{-1}}}\right)^{5.1}$$
- Predictive power important since measuring black hole masses is hard and velocity dispersions arent
- Implies galaxies and their SMBH coevolve. Measurements of $\sigma$ come from well outside the sphere of influence of the SMBH, so the galaxy and BH must coevolve

Before the M–σ relation was discovered in 2000, a large discrepancy existed between black hole masses derived using three techniques: 
- direct, or dynamical, measurements based on the motion of stars or gas near the black hole seemed to give masses that averaged ≈1% of the bulge mass (the "Magorrian relation"). 
- Two other techniques—[[Methods#Reverberation mapping|reverberation mapping]] in [[AGN]], and the Sołtan argument, which computes the cosmological density in black holes needed to explain the quasar light—both gave a mean value of $M/M_{bulge}$ that was a factor ≈10 smaller than implied by the Magorrian relation. 
The M–σ relation resolved this discrepancy by showing that most of the direct black hole masses published prior to 2000 were significantly in error, presumably because the data on which they were based were of insufficient quality to resolve the black hole's dynamical sphere of influence. The mean ratio of black hole mass to bulge mass in big early-type galaxies is now believed to be approximately 1 : 200, and increasingly smaller as one moves to less massive galaxies. 


## Faber-Jackson relation
For elliptical galaxies (same derivation as [[#Tully-Fisher relation]])$$L\propto \sigma^4$$but not very well calibrated.


## Tully-Fisher relation
For spiral galaxies. A relationship between circular velocity and luminosity: $$L\propto v^4$$**Assumptions**:
- Galaxy radiates as a thin disk
- Virialized
- Assume that a simple mass to light ratio applies to all spiral galaxies (therefore this relation doesnt apply across different environments? See [[Galaxies - Questions#107|Q107]])

**Derivation**
Virial theorem or [[Binaries#Circular motion|circular motion]] $\implies v^2 = GM/R$. 

Furthermore, let $\Gamma = M/L$ be the mass to light ratio, and assume a disk shape (since talking about spiral galaxies) $L = (2\pi R^2) (4\pi J_0)$ where $J_0$ is the [[Units#Intensity|mean surface brightness]]. This can be rearranged to $R = \sqrt{L/2\pi J_0}$. Then $$v^4 = \left(\frac{GM}{R}\right)^2 = \frac{\left(G\Gamma L\right)^2}{R^2} = (G^2 \Gamma^2 8\pi^2 J_0) L$$and we recover the proportionality above.

**Bonus**
- The Tully-Fisher relation can be used to get approximate distances from circular velocities (via redshift measurements on each side) and thus can play a role in the [[Cosmology - Questions#134|distance ladder]] 
- These days however, its moreso used as a consistency check for simulations along with the Schechter luminosity function (if they reproduce these relations theyre doing an ok job)
- The Tully-Fisher relation exhibits more scatter (making a plot of $L$ and $v_{circ}$) when measuring in blue filters than in red. This is because young, blue stars contribute most of the light of a spiral galaxy, but the larger red stars contribute most of the mass. Thus if we measure $L$ from the blue stars which dont reflect well the total mass of the system, the mass to light ratio wont accurately describe the mass of the system. As a result, better to measure $L$ in the [[Spectra#The electromagnetic spectrum|NIR]]. 