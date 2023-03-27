## 38
**What do we know about the masses and spins of (i) stellar mass black holes and (ii) supermassive
black holes, and how do we know these things?**

1. **Stellar mass black holes**
   **Masses**:
   The masses as determined by [[Observatories#LIGO|LIGO]] and other GW observatories are summarized by the following, where EM typically refers to [[Binaries#X-ray binary|x-ray binary]] measurements. Note most BHs here are ~10s of stellar masses but we still consider them as "stellar mass black holes" here. Below, we discuss how these masses are obtained. One can see the proposed "lower" mass gap from 2-5 solar masses (based on the lack of observed candidates predicts the gap), and the "upper" mass gap from 50-150 (for which it is suggested gravitational collapse cannot directly produce a BH) appears to largely be the result of mergers. In both cases the objects detected in that range may be the result of mergers.![[BH_masses.jpg]]
   - For the EM observations, we determine the mass in the following way: Via the same derivation as the end of [[Exoplanets - Questions#8|8]] we have $$v_{1,r} = \left(\frac{2\pi G}{P}\right)^{1/3}\frac{M_2\sin(i)}{(M_1+M_2)^{2/3}} \frac{1}{\sqrt{1-e^2}}$$ and vice-versa for 2. Therefore we can constrain the total mass and therefore the mass of the compact object if we have radial velocity measurements.
   - The mass of a black hole has also been inferred by X-ray [[Methods#Reverberation mapping|reverberation mapping]], which uses the time lags between correlated X-ray signals to infer information about the environment very close to a black hole. This can then be used to infer properties of the black hole. Eg (Cygnus X-1, Mastroserio+19). 
   - For the LIGO observations, use frequency and duration of binary merger expression$$\omega^{-8/3} \propto M_c^{5/3}t$$where $\omega$ is the gravitational wave frequency, $M_c$ is the [[Gravitational waves#Chirp mass|chirp mass]], and $t$ is the time to chirp (merger). Assuming coalescence happens at $r = 2GM/c^2$ where $M$ is total mass, the frequency at coalescence is $$\omega_c = \frac{c^3}{\sqrt{8} G M}$$so in this way we can find both $M$ and $M_c$ and combine them to obtain the individual masses. 

   **Spins**:
   Due to angular momentum conservation of the progenitor star, its expected that stellar mass BHs are spinning. [[Binaries#X-ray binary|X-ray binaries]] (XRBs) are rapidly spinning. LIGO has discovered many slowly-spinning BHs with $\chi_{\rm{eff}}\simeq 0$ (the [[Gravitational waves#Mass-weighted effective spin|mass-weighted effective spin]]). Now we describe how these are measured. [Source](https://www.annualreviews.org/doi/abs/10.1146/annurev-astro-112420-035022) 
   
   - Method 1 for XRBs: can use **reflection spectroscopy** which is using the shape of spectral lines emitted in the [[AGN#AGN|corona]] and reflected off the accretion disk to constraing $R_{\rm{ISCO}}$ (the location of the [[Black holes#ISCO|ISCO]]) which is related to the spin $a$. Key feature in the spectrum to measure this feature is the [[Spectra#Fe k-alpha line|Fe k-alpha line]] which will look like the below picture, where the two dotted lines' spectra are shown with various effects included. Dotted lines are thin annuli on a nonrelativistic disk. Shape of resulting line constrains GR effects and thus $R_{\rm{ISCO}}$ 
   ![[lineshape_effects.png|300]]
   - Method 2 for XRBs: **Thermal continuum fitting**. Spin influences temperature of inner disk by changing $R_{\rm{ISCO}}$ such that: Higher spin $\implies$ smaller $R_{\rm{ISCO}}$ $\implies$ more gravitational PE converted to KE $\implies$ hotter temperature of inner accretion disk. Requires good understanding of disk modelling and radiative transfer modelling of XRBs.
   - For LIGO: constrain using matched filtering techniques applied to the GW waveform at inspiral and merger. Constrain $a$ via [[Gravitational waves#Mass-weighted effective spin|mass-weighted effective spin]] and [[Gravitational waves#Effective precession spin|effective precession spin]]. If we only constrain $\chi_{\rm{eff}}$ there is a degeneracy due to the projection along direction of orbital angular momentum. Can be broken by knowing $\chi_p$ but that can only be constrained for unequal mass ratio binaries.

2. **Supermassive black holes**
   Masses measured to be $10^{6} - 10^{10}\,M_\odot$. How do we measure?
   **Mass**:
   - Special case: In the Milky Way we can resolve individual stellar orbits around the BH [[AGN examples#Sagittarius A|Sag A]] and infer the mass from the dynamics. Found $M\sim4\times 10^6\,M_\odot$ 
   - The M-$\sigma$ relation between mass and velocity dispersion. See [[Galaxies - Questions#124|124]]. Essentially mass of BH is related to velocity dispersion of stars in the bulge. Can measure $\sigma$ from line widths and then infer a mass.
   - [[Methods#Reverberation mapping|Reverberation mapping]] in [[AGN#AGN|AGN]]. 
   - [[Observatories#EHT|EHT]] measurements via [[Methods#Long baseline interferometry|(very) long baseline interferometry]]. Size of BH shadow depends on mass.

   **Spin**:
   These appear to be very high on average. In general, (coherent) accretion important means population has $\sim$ high spins, and mergers important means $\sim$ low spins. Seems like for the biggest of the big, mergers are important. Image below shows that assuming an underlying population of black holes that has equal numbers as a function of spin parameter, we are biased toward measuring high-spin BHS. this makes the downward trend more convincing.
   ![[smbh_spin_mass.png]]
   Spins typically measured by X-ray reflection method in XRBs, but cant use thermal continuum fitting because $kT \lesssim 0.05\,\pu{keV}$ for SMBHs $\implies$ much of the disk [[Blackbody radiation#Blackbody radiation|blackbody radiation]] is absorbed and inaccessible. 


## 39
**What properties of supermassive black holes correlate with properties of the host galaxy?**
- The M-$\sigma$ relationship (see [[#38]] and [[Galaxies - Questions#124|124]])
- BH mass scales with stellar velocity of the galaxy / galactic bulge
- Velocity dispersion $\sigma$ correlated with bulge mass and luminosity, and therefore black hole mass.
- **Feedback**: The stellar formation rate of the galaxy also correlates with the activities of the suoermassive black holes. Most galaxies tend to fall into two types: a "red sequence" and a "blue cloud". Red sequence galaxies are generally non-star-forming elliptical galaxies with little gas and dust, while blue cloud galaxies tend to be dusty star-forming spiral galaxies. The process of which star formation is turned off is called “quenching,” and one way to explain it is through AGN feedback. Simulations have shown that gas accreting onto supermassive black holes in galactic centers produces high-energy jets; the released energy can expel enough cold gas to quench star formation.


## 40
**It is believed that most stars leave a collapsed remnant at the end of their evolution. What stars leave (i) white dwarfs? (ii) neutron stars? (iii) black holes?**
Exact numbers of below are not known. Can find sources with $\pm$ 25%  on each number
$$M_{*, initial} = \cases{\lesssim0.08 \\0.08 - 0.8M_\odot \\0.8 - 8M_\odot \\ 8-20 M_\odot \\ \gtrsim 20 M_\odot} \implies \cases{\text{brown dwarf} \\ \text{MS ``forever"} \\ \text{white dwarf} \\ \text{neutron star} \\ \text{black hole}} \implies \cases{\text{same} \\\text{same} \\0.4 - 1M_\odot \\ 1.5-2 M_\odot \\ \gtrsim 3 M_\odot} = M_{*,final}$$
Why?
- In massive stars, strong winds drive major mass loss
- Chandrasekhar mass ($\sim 1.4 M_\odot$, see [[#52]] for derviation) dictates how large a core can get under degenerate conditions
	- When the core exceeds this, is unstable and will collapse on itself 
	- This happens for stars with $M\gtrsim 8M_\odot$ and thus those stars form [[Neutron stars#Neutron stars|neutron stars]] and [[Black holes#Black hole|black holes]]. 
	- During collapse, gets hot enough to fuse heavier elements
- Once burning reaches Fe, no more elements will undergo fusion
	- Only remaining source of stabilizing pressure is neutron degeneracy pressure
	- Maximum mass for this is an area of active research, but close to 2 or 3 $M_\odot$. 
	- Anything larger than this will collapse into a BH. (see RHS of cases above for final masses) 


## 41
**What is a neutron star?**
See [[Neutron stars#Neutron stars|neutron stars]].

**What assumptions and inputs go into determining the upper mass limit for a neutron star?**
Analogous to the Chandrasekhar limit for white dwarf stars, the mass limit for neutron stars is called the *Tolman-Oppenheimer-Volko limit* (or TOV limit), but the accurate value is not known because the equations of state for extremely dense matter are not well known (for deriving the degeneracy pressure due to electrons, we use the Fermi-Dirac statistics, which tacitly assumes that the particles are non-interacting; this is not bad an assumption for the electron gas inside a white dwarf, but when neutrons are packed to densities close to the density inside atomic nucleus, the neighbouring neutrons interact with each other through nuclear forces and it is no longer justified to treat them as non-interacting particles). The limit is generally held to be around $2.1\,M_\odot$, but a recent estimate puts the upper limit at $2.16\,M_\odot$. The maximum observed mass of neutron stars is about $2.14\,M_\odot$ for PSR J0740+6620 discovered in September, 2019.

**What is the approximate ratio of neutrons to protons (and electrons) in the interior
of a neutron star?**
Dictated by $\beta$ decay versus electron capture rates:

- $\beta$ decay: $n \rightarrow p + e^- + \bar{\nu}_e$
- $e^-$ capture: $p + e^- \rightarrow n + \bar{\nu}_e$

Then ratio is roughly given by ratio of Boltzmann factors for the neutron and the (proton + electron) systems $$\frac{n}{p} \sim \exp\left(-\frac{(m_n - m_p - m_e)c^2}{kT}\right) \sim \exp\left(-\frac{0.8\,\pu{MeV}}{kT}\right) \sim \exp\left(-\frac{10^{10}}{T [K]}\right)$$so at temperatures ~ $10^{10}\,\pu{K}$ we have 3 times more $p$ than $n$ but above this the exponent becomes closer to 0 and the best we can do is go to 1?? I think maybe that is flawed and should include a term for the fermi level so that the exponent can become positive(?)


## 42
**Why can we not have monopole and dipole terms in gravitational radiation (within Einstein's
GR)?**
We’ll start with electromagnetic radiation, and expand in moments. 
- For a charge density $ρ_e(r)$, the monopole moment is $∫ρ_e(r)d^3r$. This is simply the total charge Q, which cannot vary, hence there is no electromagnetic monopolar radiation. 
- The next static moment is the dipole moment, $∫ρ_e(r) r d^3r$. There is no applicable conservation law, so electric dipole radiation is possible. 
- One can also look at the variation of currents. The lowest order such variation (the “magnetic dipole”) is $∫ρ_e(r) r × v(r)d^3r$. Once again this can vary, so magnetic dipole radiation is possible. The lower order moments will typically dominate the field unless their variation is reduced or eliminated by some special symmetry.

Now consider gravitational radiation. 
- Let the mass-energy density be ρ(r). The monopole moment is $∫ρ(r)d^3r$, which is simply the total mass-energy. This is constant, so there cannot be monopolar gravitational radiation. 
- The static dipole moment is $∫ρ(r) r d^3r$. This, however, is just the center of mass-energy of the system. In the center of mass frame, therefore, this moment does not change, so there cannot be electric dipolar radiation in this frame (or any other, since the existence of radiation is frame-independent). 
- The equivalent of the magnetic dipolar moment is $∫ρ(r) r × v(r)d^3r$. This, however, is simply the total angular momentum of the system, so its conservation means that there is no magnetic dipolar gravitational radiation either. 
- The next static moment is quadrupolar: $I_{ij} =∫ρ(r)r_i r_j d^3r$. This is not conserved, therefore there can be quadrupolar gravitational radiation

As a result spherically symmetric variations cannot produce GWs and axisymmetric rotation does not produce GWs.

[Source](https://www.astro.umd.edu/~miller/teaching/astr498/lecture24.pdf )


## 43 
**Give a qualitative description of the frequency and amplitude evolution of the gravitational wave
signal from a binary compact star system**
Since energy and angular momentum are continuously carried away by gravitational radiation, the two masses in orbit spiral towards each other, thus increasing their orbital frequency $Ω$. The GW frequency $f = Ω/π$ and the GW amplitude $h$ are also increasing functions of time.








## 71
**Sketch the frequency distribution of the emission of a typical QSO from radio to X-ray frequencies.**

