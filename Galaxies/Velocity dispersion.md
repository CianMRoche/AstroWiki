
## Velocity dispersion
A series of relationships derived from the virial theorem, relating velocity dispersion to the mass of the system. In the simplest case, the relation looks something like $$M = \frac{v^2r}{G} \simeq \frac{3}{2}\frac{\sigma^2R}{G}$$where $\sigma$ is the 1D velocity dispersion (radial typically) we can actually measure. Relationship reliable up to an order $\sim 1-10$ factor

**Derivation**
The speeds of the objects in the galaxy have two components
1. The center of mass motion of the whole cluster of objects
2. The relative motion within the cluster of objects

Thus if we measure the speeds of many objects, we should see a mean speed (corresponding to the center of mass motion) and some slower, some faster, corresponding to the relative motion within that object. Lets pretend that shape is a Gaussian, then the standard deviation of that Gaussian describes the speed of a typical star within that cluster (without considering the net motion of the cluster). 

The virial theorem $\langle T\rangle = \frac{1}{2} \langle U\rangle$ for a gravitational system says that for a star of mass $m$, speed $v$ and distance $r$ from the center of a spherical mass distribution of mass $M$ we have $$\frac{1}{2}mv^2 \simeq \frac{1}{2}\frac{GMm}{r}$$Lets estimate $v$ and $r$ :
- If the system is isotropic then $\sigma_x = \sigma_y = \sigma_z$ and the total velocity dispersion is $\sigma_{\rm{3D}} = \sqrt{\sigma_x^2 + \sigma_y^2 + \sigma_z^2} = \sqrt{3}\,\sigma_{\rm{1D}}$. Note that if we make an observation, we really measure a 1-dimensional dispersion (toward us and away from us, denoted $\sigma_r$ for radial). A good estimate for the 3D speed of a star is then $v^2 \simeq 3\sigma_r^2$. 
- A reasonable estimate for the radial location of the average star is $r\simeq R/2$ 

Putting these estimates into the virial theorem and rearranging, we have $$M = \frac{v^2r}{G} \simeq \frac{3}{2}\frac{\sigma^2R}{G}$$This result however is only valid up to an order $\sim 1-10$ factor.


## M-sigma relation
A mass-velocity dispersion relation for material circling [[Black holes#Black hole|supermassive black holes]].


## Faber-Jackson relation
For elliptical galaxies


## Tully-Fisher relation
For spiral galaxies. A relationship between rotational velocity (isnt this also just dispersion?) and luminosity, $$L\propto v^4$$**Assumptions**:
- Galaxy radiates as a thin disk
- Virialized
- Assume that a simple mass to light ratio applies to all spiral galaxies (therefore this relation doesnt apply across different environments? See [[Galaxies - Questions#107|Q107]])

**Derivation**
Virial theorem or [[Binaries#Circular motion|circular motion]] $\implies v^2 = GM/R$. 

Furthermore, let $\Gamma = M/L$ be the mass to light ratio, and assume a disk shape (since talking about spiral galaxies) $L = (2\pi R^2) (4\pi I_0)$ where $J_0$ is the [[Units#Intensity|mean surface brightness]] (ie assuming isotropic). This can be rearranged to $R = \sqrt{L/2\pi J_0}$. Then $$v^4 = \left(\frac{GM}{R}\right)^2 = \frac{\left(G\Gamma L\right)^2}{R^2} = (G^2 \Gamma^2 2\pi J_0) L$$and we recover the proportionality above.