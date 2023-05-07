 ## 16
**Describe the spectral classification scheme for stars: O, B, A, F, G, K, M. What are the characteristic effective temperatures for stars of each class? What are the characteristic absorption lines observed in the spectra of stars of each class? What are the characteristic luminosities for main-sequence stars of each class? What are the approximate masses for stars in each class?**
See [[Spectra#Harvard Spectral Classification|Harvard spectral classification]] 


## 17
**Sketch the HR diagrams for a typical globular cluster and open cluster. Identify the various observed populations and interpret them on the basis of stellar evolution theory.**

1. [[Clustering#Globular Cluster|Globular cluster]] 
   The [[HR-diagram]] for a globular cluster is only evolved stars, so looks like the below (from Megan's notes). Note the [[Stellar classes#Blue straggler|blue stragglers]] at the end of the [[HR-diagram#Main sequence|main sequence]] and the instability gap due to [[Pulsating stars#RR-lyrae stars|RR-lyrae]] stars. See [this video](https://www.youtube.com/watch?v=wbvgjzW3Xz0) for an animation of how this changes with cluster age.
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
Gravothermal collapse is an instability arising from negative heat capacity of self-gravitating systems. !UNFINISHED (redo these notes with notebook summary in mind).

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
**Describe the various evolutionary phases of a low-mass (1 M☉) star and those of a high-mass (e.g. 12 M☉) star. Show the corresponding evolutionary tracks on an HR diagram.**

A summary of the stellar phases is shown below, where evolution takes place from left to right.

They also exhibit a common beginning, the [[Star formation]] stage, wherein a [[Star formation#Molecular cloud|molecular cloud]] collapses provided it is larger than the [[Jeans#Jeans mass|Jeans mass]] for that cloud.

Good estimate for the [[Jeans#Jeans length|Jeans length]] in the molecular cloud where they formed: 
- Distance to closest star is $\sim 1\,\pu{pc}$ (proxima cantauri)
- Lengths have expanded a factor of $\sim 4$ since redshift $\sim3$ (via [[FLRW#Friedmann equation|Friedmann eq]]) (might need to consiider volumes but all order-1 factors anyway)
- The Jeans length in the original cloud must have been $\lesssim 0.1 \,\pu{pc}$ 

1. Low-mass:
| Stage    | [[HR-diagram#Pre-main sequence\|Pre-MS]] | [[HR-diagram#Main sequence\|MS]]                   | [[HR-diagram#Subgiant branch\|Subgiant branch]] | [[HR-diagram#RGB\|RGB]] | Horizontal branch | AGB | [[Nebulae#Planetary nebula\|Planetary nebula]] | [[Stellar classes#White dwarf\|White dwarf]] |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Time in stage ($\pu{yr}$) | | $\sim10^{10}$ |  | $\sim10^{9}$ |  $\sim10^{8}$  | $\sim10^{6}$  |   $\sim10^{5}$    |             |

   which shows up on the HR diagram as (from Megan's notes)
   ![[evolution_HR.png|500]]


2. High-mass:
   The elements on the left represent what is currently being burned in the core, and each lobe on the top is basically the SGB-RBG-helium flash-horizontal branch evolution, but with a different cycle of burning a thing in the core and then shell burning.
| Stage    | [[HR-diagram#Pre-main sequence\|Pre-MS]] | [[HR-diagram#Main sequence\|MS]]  | maybe a blue loop | Red supergiant | [[Supernovae#Supernova\|Supernova]] | [[Neutron stars#Neutron stars\|NS]] or [[Black holes#Black hole\|BH]] |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Time in stage ($\pu{yr}$) | | $\sim10^{7}$ |  | $\sim10^{6}$ | |   |

   which shows up on the HR diagram as a 💩 on the supergiant branch (from Megan's notes)
   ![[evolution_HHR_highmass.png|500]]


## 23
**Describe the types of stellar evolution that lead to type Ia, type Ib and type II supernovae. What are the observational differences among these?**
See [[Supernovae#Supernova|supernovae]]. The primary observational signatures are:

Type 1a ([[Stellar classes#White dwarf|WD]] with mass $\sim 1.4\,M_\odot$)
- CO white dwarfs because they need to be relatively massive, imprint on spectra? no idea
- No Hydrogen lines
- A distinct Silicon II (singly-ionized) line that helps distinguish from 1b/c.

Type 1b ($\,\gtrsim 30\,M_\odot$)
- Core collapse of massive star, blew off its H envelope so again no H lines
- He lines from He envelope
- No silicon lines

Type 2 ($\,\gtrsim 8\,M_\odot$)
- massive stars (thus short lifetimes) so often found in star-forming regions
- H absorption lines
- Large variety of light curves due to variety of progenitors.


## 24
**What is a Cepheid variable? Explain the underlying stellar physics involved.**
See [[Pulsating stars#Cepheids|Cepheids]]. 

**What is the Leavitt Law? Over what range of distances do Cepheids play a major role in the “cosmic distance ladder”?**
Henrietta Swan Leavitt established a period-luminosity relation in Cepheids by studying thousands of stars in the [[Galaxy examples#Large Magellanic Cloud|LMC]] and [[Galaxy examples#Small Magellanic Cloud|SMC]]. Ths relationship was a simple power law $$M_V = -2.43\log P - 4.05$$where $M_V$ is the [[Magnitudes#UBVRI|V band]] [[Magnitudes#Absolute magnitude|absolute magnitude]]. This allowed the measurement of absolute magnitudes from pulse periods and thus, distances (by comparing with the [[Magnitudes#Apparent magnitude|apparent magnitude]]). This relationship was calibrated with Cepheids that had known distances via parallax. 

Biggest source of uncertainty is via metallicity dependence and obscuration via interstallar [[Dust#Dust|dust]]. Relatively local distance estimator since need to be able to resolve a single star and reliably measure period. Furthest such object is NGC 3370 at $\sim 29\,\pu{Mpc}$. 


## 25
**What are RR Lyrae stars, and how do they differ from Cepheids?**
See [[Pulsating stars#RR-lyrae stars|RR-lyrae]] stars.

Differences are that relative to [[Pulsating stars#Cepheids|cepheids]] these stars are
- Dimmer
- Shorter pulsation periods
- Lower mass
- Hard to calibrate the less consistent period-luminosity relationship


## 26
**What are the following objects and where are they found?**
**(i) HH objects?**
"Herbig Haro objects". Bright patches of emission from where the jet launched from protostars (like [[Stellar classes#T-tauri star|T-tauri stars]]) interact with and excite the surrounding material, a bit like an [[Nebulae#Emission nebula|emission nebula]]. In fact, the first one discovered was classified as an emission nebula rather than a distinct class of object.

- Typically found in [[Star formation#Molecular cloud|molecular clouds]] and other star forming regions
- When the excited gas relaxes/recombines, see strong emission lines in the [[Spectra#The electromagnetic spectrum|optical]]. 
- Jets moving at $\sim 100\,\pu{km s^{-1}}$ probably formed due to presence of an [[Accretion#Accretion disk|accretion disk]]
- Transient that lasts $\sim 10^4$ years, can change on month to year timescales as jet encounters new media
- First discovered in the orion nebula

![[HH_object.jpg|400]]

**(ii) T Tauri stars?**
See [[Stellar classes#T-tauri star|T-tauri stars]].

**(iii) Bipolar flows?**
Two-sided outflows launched by protostars (younger than [[Stellar classes#T-tauri star|T-tauri]] stars) or evolved post-[[HR-diagram#AGB|AGB]] stars.  Flow is driven by a dense, collimated jets, which can make the outflow difficult to observe directly. In the case of evolved stars, can find these flows in [[Nebulae#Planetary nebula|planetary nebulae]] with a jet driven by [[Accretion#Accretion disk|accretion]] from a [[Binaries|binary]] companion, whereas the accretion for a young star does not have a binary companion (similar to the HH object above).

![[boomerang_nebula_bipolar_flow.jpg|400]]

**(iv) OH masers?**
"Microwave amplification of stimulated emission of radiation". Objects with significant OH [[Emission & the ISM - Questions#88|stimulated emission]] in the [[Spectra#The electromagnetic spectrum|millimeter]] ($\sim 1.6 \,\pu{GHz}$). Objects with line intensities far above what would be expected of a blackbody. 

As with bipolar flows, also found near protostars or evolved post-[[HR-diagram#AGB|AGB]] stars.


## 27
**What is a planetary nebula? What is our current understanding of the formation of planetary nebulae?**
See [[Nebulae#Planetary nebula|planetary nebula]].


## 28
**What is a P Cygni line profile, and what does it signify?**
See [[Spectra#P Cygni Line Profile|P Cygni line profile]].


## 29
**Two stars are observed to have the same color and brightness. One of them is a giant at a greater distance than the other, which is a main sequence star. How could these be distinguished from spectroscopic measurements?**

Put another way, if two stars have the same surface temperature (~color), and the same [[Magnitudes#Apparent magnitude|apparent magnitude]] we cannot distinguish them according to the [[Spectra#Harvard Spectral Classification|Harvard spectral classes]]. We could thus have a very luminous but distant star and a very dim but nearby star of the same surface temperature, and we would classify them as the same object. To distinguish further we need the [[Spectra#Morgan-Keenan (MK or MKK) Luminosity Class|MK luminosity class]], which utilizes the difference in line broadening for different size objects to distinguish between such objects. 


## 30
**Write down and describe the four basic equations of stellar structure.**
See [[Stellar structure equations]]. 


## 31
**Make a dimensional analysis of the equation of hydrostatic equilibrium using a polytropic equation of state to find a general mass-radius relation for spherically-symmetric, self-gravitating bodies.**
Start with the [[Polytropes#Polytrope|polytrope]] equation of state $$P = \kappa \rho^{\gamma}$$Doing some very loose dimension-matching and dividing by $R$ we convert the polytrope equation to $$\frac{P_c}{R} = \frac{K\bar{\rho}^{\gamma}}{R}$$Using [[Stellar structure equations#Hydrostatic equilibrium|HSE]] we also have $$\frac{dP}{dr} = -\frac{GM_{<r}\rho}{r^2}$$Doing the same loose dimension matching for HSE we get $$\frac{P_c}{R} = -\frac{GM_{tot}\bar{\rho}}{R^2}$$Equating the two (and labelling the total mass as $M$) we get $$M \sim R\,\bar{\rho}\,{}^{\gamma - 1}$$Replacing $\bar{\rho}$ with $M/R^3$ this results in $$M\propto R^{\frac{4 - 3\gamma}{2 - \gamma}}$$
**For which two polytropic indices is the configuration unstable?**
- At $\gamma = 2$ the mass scales "infinitely quickly" with $R$
- At $\gamma = \frac{4}{3}$ the mass is independent of $R$ 


## 32
**Make a dimensional analysis of the equation of radiative diffusion in stars to show that the luminosity of a star scales as its mass cubed, if the opacity is taken to be a constant and assuming that radiative diffusion is the dominant mechanism for energy transfer.**

The [[Stellar structure equations#Energy transport|energy transport]] equation for radiation-dominated systems is $$\frac{dT}{dr} = -\frac{3\kappa}{16\pi a c}\frac{\rho L}{ r^2 T^3}$$forgetting constants (including the opacity) and replacing with some loose dimensional equivalents we have  $$\frac{T}{R} \sim \frac{\bar{\rho} L}{ R^2 T^3}$$and replacing $\bar{\rho}$ with $M/R^3$ this results in $$L \sim R^4 T^4 M^{-1}$$How do we eliminate $T$? Use ideal gas to get $$P \sim \frac{N}{V}T \sim \frac{\rho}{\mu m_p}T \sim \rho T$$where we assume the [[Mean molecular weight#Mean molecular weight|mean molecular weight]] is constant. Then replace $P$ via [[Stellar structure equations#Hydrostatic equilibrium|HSE]] $$\frac{P}{R} \sim \frac{M^2}{R^5} \implies P \sim \frac{M^2}{R^4}$$to get $$\frac{M^2}{R^4} \sim \rho T \implies T\sim \frac{M}{R}$$and so finally $$L \sim R^4 T^4 M^{-1} \sim R^4 \frac{M^4}{R^4} M^{-1}\sim M^3$$

## 33
**Use the known luminosity and mass of the Sun to estimate its nuclear lifetime.**
Luminosity of [[The Sun#The Sun|the Sun]] is about $L_\odot \simeq 10^{26}\,\pu{W}$. How long can the mass-energy of teh Sun power such a luminosity?

Not all the Suns mass will be converted to energy, the real number is actually the solar mass times the fraction of the Suns mass which is hydrogen $X \simeq 0.7$ times the fraction of this mass which will be burned $f\simeq 0.1$, times the energy efficiency of nuclear burning $\eta \simeq 0.007$. The mass energy which can go into producing light is thus $E = f \eta X M_\odot c^2$ and the [[Timescales#Main Sequence Timescale|Main sequence timescale]] for the sun is then $$\tau_{MS,\odot} = \frac{f \eta X M_{\odot} c^2}{L_{\odot}} \simeq 10\,\pu{Gyr}$$
**What is the current age of the sun, roughly?**
Best estimates for the age of the Sun are based on radioactive dating of meteorites and modelling of the solar spectrum, placing the age at about $4.5\,\pu{Gyr}$. 


## 34
**Describe the prominent neutrino producing reactions in the sun, and the experiments designed to detect them.**
Neutrinos are produced in large quantities in the [[The Sun#The Sun|Sun]] since lepton number is conserved in nuclear reactions in the Sun, and they very easily escape (with a mean free path of $\sim 10\,\pu{pc}$). This also means that we can directly probe the core of the Sun if we happen to detect neutrinos coming from there. 

The primary creation mechanism is via the [[#35|pp-chain]], for which we expect all to be electron neutrinos:
- The first step (PP1) results in about 90% of solar neutrinos. 
- The rest come from PP2 (~7%) and PP3 ($\lesssim$ 1%)

**What was the solar neutrino problem and how was it solved?**
The homestake experiment was a detector a mile underground that searched for neutrinos in the 1970s. It operated via the reaction $$\ce{^{37}Cl + \nu_e <-> ^{37}Ar + e^-}$$and one would examine the amount of argon present. 

The summary is they saw only one third of the neutrino flux they expected to detect ("solar neutrino problem"). Results confirmed with other experiments like Super-Kamiokande, SAGE and GALLEX. 

Resolution is either
1. We dont understand the Sun
2. Something happens to the neutrinos on their way from the Sun to us

The detectors are only sensitive to electron neutrinos, and so if they oscillate between the different flavours (electron, tauon, muon neutrinos) we would only see about 1/3 of the electron neutrino flux emitted by the Sun. Resulted in 2002 Nobel prize. Later confirmed by Solar Neutrino Observatory which could detect all 3 flavors and found about 1/3 of each, matching oscillation theory. 


## 35
**Write down the basic equations of the p-p chain that provides the Sun's nuclear power**

A mechanism to fuse hydrogen into helium. Below are the 3 branches of the pp-chain. In branch PP1 we effectively turn 4 protons (subtracting off the two left at the end) into:
- a helium nucleus
- a gamma ray
- a positron that will annihilate and create a second gamma ray
- an electron neutrino

In the diagram the lower number indicates the number of protons and is thus degenerate with the name of the element (ie you can ignore the lower numbers) and a proton is written as H so i think its assumed these things are all ionized. 
![[ppchain.gif]]
Note thatall branches just make helium nuclei (and release some neutrinos and photons), and ppII and ppIII are just getting from Beryllium 7 to 2 helium nuclei by going "down" and "up" an element on the periodic table, respectively. No RHS is a single thing unless its the final step (so if youve only written one thing, add a gamma).

[Source for image](http://burro.cwru.edu/academics/Astr221/StarPhys/ppchain.html) . The energy generated per unit volume in a general reaction $\ce{A + B -> C + D}$ is $$\epsilon = Q n_A n_B \langle \sigma v\rangle \left(\frac{1}{1 + \delta_{AB}}\right)$$where $v$ is the speed, $\sigma$ the cross section, and the parenthetical term halves the number to avoid double counting if $A$ and $B$ are the same thing. The energy output $Q$ is $$Q = \text{energy of RHS - energy of LHS}$$Evaluating this with some inspiration from nuclear physics, the Maxwell-Boltzmann distribution for the speeds, and expanding about the "Gamow peak" (not going into details) one ends up finding the energy generation is roughly $\epsilon \propto T^4$ at around $1.5\times 10^7\,\pu{K}$.


## 36
**How does the CNO cycle work?**
A mechanism to fuse hydrogen into helium. Discussing only CNO1 which is the branch that occurs 99.96% of the time, 3 others, some only really happening in very massive stars and[[Supernovae#Supernova|supernovae]]. 

A lot like [[#35|PP1]] in that it turns 4 protons into 
- A helium nucleus
- two positrons (which will end up annihilating into gamma rays)
- two electron neutrinos

but it is *catalytic*, meaning it doesnt use up some of the "inputs" like the carbon, nitrogen and oxygen over the whole cycle. They are used up in one step but regenerated in another. Can "start" looking at the reaction on the top right, noting that you need a carbon 12 atom around to get going
![[CNO_cycle.png|400]]
Actually remembering both the 1 and 2 branches simultaneously isnt that hard (see [[Mnemonics]]) ![[cno_panels.png|500]]

The pp-cycle is more efficient at the [[The Sun#The Sun|Suns]] temperature, as demonstrated below, where the y axis is a relative energy output: 
![[Nuclear_energy_generation_comparison.png|400]]

## 37
**Describe the internal structure of the sun**
See [[The Sun#The Sun|the Sun]] (but do not look at it directly unless you have the right eye protection). Why does the sun have a radiative zone outside the core and a convective zone outside that? Explained below.

**What is the Schwarzschild criterion for convective instability, and how does it delineate the convective and radiative zones in the sun?**
The summary is that <mark class="hltr-pink">a radiative zone forms where the material is stable against the formation of convective cells</mark> and the criteria for stability **against** this convection is $$\Bigg|\frac{dT}{dr}\Bigg| < \Bigg|\frac{dT}{dr}\Bigg|_{\text{adiabatic}} = \left(1-\frac{1}{\gamma}\right)\frac{T}{P}\frac{dP}{dr}$$where $\gamma$ is the assumed [[Polytropes#Polytrope|polytropic]] exponent and we take absolute values because those quantities are often negative. (Can also reframe this equation in terms of logarithmic derivatives since $(1/x)df/dx = d \ln(f)/dx$). 

- Small temperature gradient means radiative 
- large temperature gradient means convective

**More detail**:
The radiation zone is <mark class="hltr-pink">stable against formation of convection cells if the density gradient is high enough</mark>, so that an element moving upwards has its density lowered (due to adiabatic expansion) less than the drop in density of its surrounding, so that it will experience a net buoyancy force downwards. Like an air bubble rising out of water into helium gas, it will be pushed back toward the water. 

Making some assumptions about adiabatic evolution, [[Polytropes#Polytrope|polytropic]] equation of state, then also simultaneously using ideal gas law to eliminate $P$ in favor of $T$ (? Megans notes) and deriving the criteria from the density relationship mentioned above, one finds the above expression.

![[convective_radiative_layers.png]]

Let us examine the [[Stellar structure equations#Energy transport|radiative energy transport]] equation and look for what physics could lead to large temperature gradients, and thus convective zones: $$\Bigg|\frac{dT}{dr}\Bigg|_{\text{radiative}} = \frac{3\kappa}{16\pi a c}\frac{\rho L}{ r^2 T^3}$$Large (and thus convective) when 
- $\kappa$ large, $T$ low: as in the outer layers of sun-like stars
- $L/r^2$ large (a [[Units#Flux|flux]] roughly): like cores of very luminous stars
- $\gamma$ close to 1: as in low mass stars (see [[Polytropes#Polytrope|polytropes]])