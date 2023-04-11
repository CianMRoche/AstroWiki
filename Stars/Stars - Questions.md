## 16
**Describe the spectral classification scheme for stars: O, B, A, F, G, K, M. What are the characteristic effective temperatures for stars of each class? What are the characteristic absorption lines observed in the spectra of stars of each class? What are the characteristic luminosities for main-sequence stars of each class? What are the approximate masses for stars in each class?**
See [[Spectra#Harvard Spectral Classification|Harvard spectral classification]] 


## 17
**Sketch the HR diagrams for a typical globular cluster and open cluster. Identify the various observed populations and interpret them on the basis of stellar evolution theory.**

1. [[Clustering#Globular Cluster|Globular cluster]]
   The [[HR-diagram]] for a globular cluster is only evolved stars, so looks like the below (from Megan's notes). Note the [[Stellar classes#Blue straggler|blue stragglers]] at the end of the [[HR-diagram#Main sequence|main sequence]] and the instability gap due to [[Pulsating stars#RR-lyrae stars|RR-lyrae]] stars. 
   ![[globular_HR.png|500]]
   The observed <mark class="hltr-pink">turn-off point of the main sequence can be used to estimate the cluster's age, since as a cluster ages, the turn off-point migrates down the HR diagram</mark>. Since a star existing in what has been labelled the blue straggler area will only be able to survive on the main sequence for a certain amount of time before turning into a red giant. A star just past the turnoff could stay on the main sequence for about 3 billion years, but a star far past could only fuse helium for about 50 million years before becoming a red giant. If the turning point is at a very high temperature and luminosity, this means the cluster is very young and those stars havent had the chance to become red giants yet, but over time the population migrates to red giants and the turn-off point moves down along the main sequence.

2. [[Clustering#Open cluster|Open cluster]]
   An open cluster is young, so we dont see any post-main sequence evolutionary phases.
   ![[open_hr.png|400]]

**How would you go about constructing lines of constant stellar radius on the diagram?**
Assume [[Blackbody radiation#Blackbody radiation|blackbody]] and thus via [[Blackbody radiation#Stefan-Boltzmann Law|Stefan-Boltzmann law]] have $$\log L = \log(4\pi\sigma) + 2\log R + 4\log T$$that is for a given $R$ we have a power law, which appears as a line on teh log-log plot. Since $T$ increases to the left (😱) this amounts to a line with negative appearing slope, with vertical offset scaling with $R$ 


## 18
**From a physics perspective, how does the quantity (B-V) help to determine a star's effective (surface) temperature?**
If we assume the surface of the star is emitting as a [[Blackbody radiation#Blackbody radiation|blackbody]], then by [[Blackbody radiation#Wien's displacement law|Wien's law]] we know hotter blackbodies peak earlier. As a result, taking a measurement in say the B and V bands, then taking their difference, one obtains a crude estimate of the slope of the distribution which is correlated with the temperature. 

See below (from Megan's notes) that for a $6000\,\pu{K}$ blackbody, $\rm{B-V}$ is small because the slope is small, but at $3000\,\pu{K}$ it is large. Thus $\rm{B-V}$ <mark class="hltr-pink">scales inversely with surface temperature</mark>. This $\rm{B-V}$ color appears for example on the [[HR-diagram#Hertzsprung-Russel diagram|HR-diagram]] as an alternative temperature axis (but increasing the opposite way to temperature).

![[color_temperature.png|500]]

From the definition of [[Magnitudes#Apparent magnitude|apparent magnitude]] one can also interpret this difference as a ratio of fluxes in the following manner, where $m_B$ is written in place of $B$ to make explicit that we are talking about the magnitude observed in this band $$m_B - m_V = -2.5\log _{10}\left(\frac{F_B}{F_V}\right)$$

## 19
**What are stellar populations?**
See [[Stellar classes#Pop N|Pop N]]. 

**Give several examples of Pop. I and Pop. II objects in our galaxy.**
- Pop 1: [[The Sun#The Sun|the Sun]], stars in the spiral arms and disk, any star-forming regions
- Pop 2: [[Milky Way#Milky Way|Milky Way]] bulge, globular clusters, stellar halo
- Pop 3: nowhere.


## 20
**What is the "mass-function" of a binary star system and how is it determined?**
Consider a [[Binaries|binary]] between objects of mass $M_1$ and $M_2$ on effectively circular orbits in which we can observe [[Spectra|spectra]] of the bright object $1$ but cannot observe object $2$. For observations at an inclination angle $i$, the quantity $$\frac{M_2\sin(i)}{(M_1+M_2)^{2/3}}$$is called the "binary mass function". It is an observable in the radial velocity of object $1$ (obtained via redshifting of spectra) which tells us the mass of object 2. The derivation and the full expression for the radial velocity are in [[Exoplanets - Questions#8|Q8]].


## 21
**What is meant by the "gravothermal collapse" of a globular cluster, and what can save the cluster
from complete collapse?**
Gravothermal collapse is an instability arising from negative heat capacity of self-gravitating systems. 

1. Negative heat capacity:
  Assuming 3 degrees of freedom and ideal gas, can write for the average particle $$\rm{KE} = \frac{1}{2}m\bar{v}^2 = \frac{3}{2}kT$$and thus the total kinetic energy is $\frac{3}{2}NkT$. From the virial theorem we know $$E = -\, \langle\rm{KE}\rangle = -\frac{3}{2}NkT$$making clear that $\partial E/\partial T < 0$ ie a negative heat capacity. Thus when the system loses energy, the temperature increases and it gets hotter (to what systems does this <mark class="hltr-pink">not</mark> apply?).

2. In a [[Clustering#Globular Cluster|globular cluster]]:
  Imagine a cluster with two components, a dense core and an extended halo. 
  - If energy is transferred from the core to the halo (eg by radiation), the core heats up (by negative heat capacity).
  - Since again by the virial theorem $E\sim \frac{1}{2}U \sim GM^2/R$ and the mass stays roughly constant, the core also shrinks
  - Increases temperature and density of core leads to greater energy losses
  - Process repeats in a runaway manner unless some energy is injected into the core

3. How to prevent:
   The complete collapse can be prevented by scattering of a binary system by a third object. Basic idea is energy is taken out of the orbits of binaries and injected into the KE of other stars, or that 3-body interactions form binaries and again increase the KE of the third object. Exact mechanism for the scattering that leads to injection of KE into stars via these mechanisms I wont write down.


## 22
**Describe the various evolutionary phases of a low-mass (1 M☉) star and those of a high-mass
(e.g. 12 M☉) star. Show the corresponding evolutionary tracks on an HR diagram.**

A summary of the stellar phases is shown below, where evolution takes place from left to right, excluding the [[Star formation]] stage wherein a [[Star formation#Molecular cloud|molecular cloud]] collapses provided it is larger than the [[Star formation#Jeans mass|Jeans mass]] for that cloud.

1. Low-mass:
| Stage    | [[HR-diagram#Pre-main sequence\|Pre-MS]] | [[HR-diagram#Main sequence\|MS]]                   | Subgiant | RGB | Horizontal branch | AGB | [[Nebulae#Planetary nebula\|Planetary nebula]] | [[Stellar classes#White dwarf\|White dwarf]] |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Time in stage ($\pu{yr}$) | | $\sim10^{10}$ |  | $\sim10^{9}$ |  $\sim10^{8}$  | $\sim10^{6}$  |   $\sim10^{5}$    |             |

   which shows up on the HR diagram as (from Megan's notes)
   ![[evolution_HR.png|500]]


2. High-mass:
| Stage    | [[HR-diagram#Pre-main sequence\|Pre-MS]] | [[HR-diagram#Main sequence\|MS]]  | maybe a blue loop | Red supergiant | [[Supernovae#Supernova\|Supernova]] | [[Neutron stars#Neutron stars\|NS]] or [[Black holes#Black hole\|BH]] |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Time in stage ($\pu{yr}$) | | $\sim10^{7}$ |  | $\sim10^{6}$ | |   |

   which shows up on the HR diagram as a 💩 on the supergiant branch (from Megan's notes)
   ![[evolution_HHR_highmass.png|500]]