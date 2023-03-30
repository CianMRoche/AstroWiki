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
**Give a qualitative description of the frequency and amplitude evolution of the gravitational wave signal from a binary compact star system**
Since energy and angular momentum are continuously carried away by gravitational radiation, the two masses in orbit spiral towards each other, thus increasing their orbital frequency $Ω$. The GW frequency $f = Ω/π$ and the GW amplitude $h$ are also increasing functions of time. We know the waves carry energy because of [[Gravitational waves#Sticky bead argument|sticky bead argument]]. 

Skipping the derivation ([source](https://link.springer.com/article/10.12942/lrr-2006-6#Sec3)), the frequency of the gravitational waves (assuming a Newtonian approximation for the orbit) are governed by the equation$$\frac{df}{dt} = \frac{96}{5}\pi^{8/3}\left(\frac{GM_c}{c^3}\right)^{5/3}f^{11/3} \simeq 2\times 10^{-57} M_c^{5/3}f^{11/3}$$ for the [[Gravitational waves#Chirp mass|chirp mass]] and frequency in SI units. We can integrate this to obtain $$f(t) = \frac{1}{2\pi} \left(\frac{256G^{5/3}M_c^{5/3}}{5c^5}\right)^{-3/8}(t_{coal} - t)^{-3/8}$$where $t_{coal}$ is the coalescence time and the expression diverges at coalescence. This may be a factor of 2 off, Meghans notes says $\omega = \pi f$ and not $2\pi f$ since radiation is quadrupolar Maybe thats just for identical sources. The average amplitude of a GW at a distance $r$ from the source over a period involves an average of the two polarization states ($+$ and $\times$) as $$h(f,M_c,r) = \left(\langle h_+^2\rangle + \langle h_\times^2\rangle\right)^{1/2} = \left(\frac{32}{5}\right)^{1/2} \frac{G^{5/3}}{c^4}\frac{M_c^{5/3}}{r}(\pi f)^{2/3}$$Putting this together we get something llike (from Meghans notes, $\tau_c = t_{coal}$) ![[GW_profiles.png|400]]

**Compute actual numbers for a 30-30$M_\odot$ binary black hole system**
[[Gravitational waves#Chirp mass|Chirp mass]] here is 26.12 $M_\odot$ but in order to calculate the frequency/amplitude evolution we would need to know the distance to the system.  Since its an equal mass system, the period is actually half of what one would infer from the above because we have to identical things making a half rotation brings us back to the intial configuration. We can work out the frequency at coalescence by assuming coalescence happens at a separation of the Schwarz schild radius $R_S = 2GM_c/c^2$ and thus via [[Binaries#Circular motion|circular motion]] approximation we have $$\omega_{coal} = \sqrt{\frac{GM_c}{R_S^3}} = \frac{c^3}{2^{3/2}GM_c}\simeq{1200\,\pu{rad\,s^{-1}}}$$for the chirp mass in question. Corresponds to a minimum linear frequency of $\sim 400\,\pu{Hz}$ since system is identical after a half rotation(?). We cant work out the amplitude without a distance, but for the closest plausible objects we would have $h\sim 10^{-21}$ strain, so for a $4\,\pu{km}$ arm length (as [[Observatories#LIGO|LIGO]] has) the distance change would be $0.04\,\pu{fm}$ and for comparison, a proton has a root mean square charge radius of $\sim 1\,\pu{fm}$


## 44
**A double neutron star system in M31 is about to merge. What is the approximate energy emitted
in gravitational radiation and what is the corresponding amplitude (strain) h observed here on
Earth?**
Im not sure how they realistically can ask this. Approximate as a common mass [[Neutron stars#Neutron stars|neutron star]] binary of $1.4 M_\odot$ each ($\implies M_c \simeq 1.2\,M_\odot$) and $\sim10\,\pu{km}$ radius each, so coalescence happens at a $\sim20\,\pu{km}$ separation. Thus as in [[#43]] the frequency is $$\omega_{coal}\simeq 4000\,\pu{rad\,s^{-1}} \implies f \sim 1\,\pu{kHz}$$and the gravitational energy emitted (a [[Units#Luminosity|luminosity]]) goes as $$L_{GW} = \frac{G}{5c^2}\left\langle\dddot{Q} \dddot{Q}\right\rangle = \dots = \frac{32}{5}\frac{G}{c^2}\mu^2R^4\omega^6 = \frac{32}{5}\frac{G^{7/3}}{c^5}\frac{(M_1 M_2)^2}{M_{tot}^{2/3}}\omega^{10/3}$$where $Q$ is the traceless moment of intertai tensor, $\mu$ is the reduced mass and $R$ is the separation and the last step comes from Keplers 3rd law + equating the energy lost in a virialized orbit as the radius decreases to the GW luminosity. Here $L_{GW}\sim 10^{46}\,\pu{W}$. Dont need to know that derivation. End up with total energy $\sim L_{GW} T_{merge}$ where $T_{merge}\sim 10\,\pu{ms}$ which comes to $E\sim10^{44}\,\pu{J}$ which is on the order of a supernova.

To calculate strain, distance to [[Galaxy examples#M31|M31]] is $\sim 800\,\pu{kpc}$ and so end up with $h\sim 10^{-20}$. 

**Would LIGO be able to detect it?**
This is well within the [[Observatories#LIGO|LIGO]] sensitivity at a frequency of $1\,\pu{kHz}$ 

![[GW_strain_sensitivity_curves.png|600]]


## 45
**Besides the merger of two compact objects, what other sources of gravitational waves are
expected (though maybe not yet detected)?**
Any accelerating mass with a quadrupole moment. 

Detected binary sources:
- Binary stellar-mass [[Black holes#Black hole|black holes]]
- Binary [[Neutron stars#Neutron stars|neutron stars]]
- Neutron star - BH mergers

Not yet detected binaries:
- [[Stellar classes#White dwarf|WD]] - WD binary, WD - NS, WD - BH
- Supermassive black hole binaries ([[Observatories#LISA|LISA]] or [[Pulsar timing]], see [[Gravitational waves#Spectrum|GW spectrum]])
- Extreme mass-ratio inspiral (EMRI; [[Observatories#LISA|LISA]])

**Other potential sources**:
- Isolated [[Neutron stars#Neutron stars|NS]] with asymetry and rotation (eg. "mountains" on the surface)
	- Why no detection yet? Very weak signal
	- Will be continuous signal of roughly constant frequency
- [[Supernovae#Supernova|Supernovae]] or long [[GRBs#GRB|GRBs]]. 
	- Cant be spherically symmetric
	- GW signal from such sources currently unclear, but probably bursty
- Primordial GWs (fluctuations near big bang)
	- Analogous to CMB in that it is stochastic background on whole sky
	- More likely to detect via [[Pulsar timing#Pulsar timing|PTAs]]. GW signal will be correlated across pulsar signals, but noise will not be.


## 46
**How does the orbital frequency of the innermost stable circular orbit around a black hole scale
with its (i) mass? (ii) spin?**
For BH of mass $M$, orbital frequency (via [[Binaries#Circular motion|circular motion]]) is $$\Omega_{\rm{ISCO}}^2 = \frac{GM}{R_{\rm{ISCO}}^3}$$And the radius goes as (See [[Black holes#ISCO|ISCO]] for helpful plot at a particular mass)$$R_{\rm{ISCO}} = \alpha \frac{GM}{c^2}$$where $\alpha$ is a spin-dependent factor that has the following limiting cases: $$a = \cases{-1&\text{(retrograde, maximal)} \\ 
~0&\text{(Schwarzschild)} \\ 
+1&\text{(prograde, maximal)}} \implies \alpha = \cases{9 \\ 6 \\ 1}$$so $\alpha$ and thus $R_{\rm{ISCO}}$ decreases as relative spin (so retrograde is considered "less spin") is increased. Since $$\Omega_{\rm{ISCO}} \sim \frac{1}{\alpha^{3/2}M}$$ we have that:
- Relative spin $\uparrow$ $\implies$ $\Omega_{\rm{ISCO}}$ $\uparrow$ 
- Mass $\uparrow$ $\implies$ $\Omega_{\rm{ISCO}}$ $\downarrow$ 


## 47
**What is the Eddington limit and how is it manifested in (i) ordinary stars? (ii) accreting X-ray
sources?**
Eddington limit is the maximum [[Units#Luminosity|luminosity]] a body of mass $M$ can have when gravity and radiation pressure are balanced. To derive the limit, assume all the matter is ionized Hydrogen but for now write the density as $\rho$, and consider the Euler equation in hydrostatic equilibrium: $$\frac{dP_g}{dr} = -\frac{GM}{r^2}\rho$$Then consider the radiation pressure (the derivation seems fairly involved, skipping)$$\frac{dP_{rad}}{dr} = -\frac{\kappa\rho}{c}F = -\frac{\sigma_T\rho}{m_p c} \frac{L}{4\pi r^2}$$where $F$ is the [[Units#Flux|flux]], $\kappa$ is the [[Optical depth#Opacity|opacity]] (dimensions cross section per mass) and we have approximated that for pure ionized Hydrogen, the opacity comes entirely from [[Scattering#Thomson scattering|Thomson scattering]] so that $\kappa = \sigma_T / m_p$ which we assume to be constant. Equating the two, we find in terms of [[The Sun#The Sun|solar]] parameters $$L_{Edd} = \frac{4\pi G M c}{\kappa} = \frac{4\pi G M m_p c}{\sigma_T} = 3.2\times 10^4 \left(\frac{M}{M_\odot}\right)L_\odot$$**In ordinary stars**:
When a star exceeds Eddington limit, radiation pressure drives significant stellar winds in the outer layers, leading to significant mass loss.
- Only happens in most massive stars, since $L\sim M^{3.5}$ (for [[Spectra#Main sequence|MS]] stars) and $L_{Edd} \sim M$ eventually as mass increases the luminosity overtakes the Eddington limit and the star begins to blow out mass.
- Increased opacity increases radiation's effect on the star (via more interactions, perhaps via [[Dust]]) and thus lowers the Eddington luminosity
- Massive stars are Eddington-limited in post-[[Spectra#Main sequence|MS]] evolution, and thus travel *horizontally* on the [[Spectra#Hertzsprung-Russel diagram|HR diagram]].
- Derivation assumes spherical symmetry, and thus limit can be exceeded in asymmetric systems

**In X-ray sources**:
Source is via accretion onto a compact object like a [[Black holes#Black hole|black hole]]
- Accretion liberates gravitational potential energy as gas loses angular momentum + falls onto the compact object $L = \eta \dot{M} c^2$ (energy radiated per time = efficiency $\times$ mass-energy gained per time). The accretion efficiency $\eta$ is about 6% for Schwarzschild and 40% for a maximally spinning BH. Estimating as 0.1 is fine.
- Accreting sources can also be Eddington-limited like stars, in that:
	- For $L/L_{Edd} \lesssim 0.5$ have standard thin, radiatively efficient accretion disk
	- For $L/L_{Edd} \gtrsim 0.5$ have a puffed-up disk since the radiation pressure increases the height to radius ratio, which leads to radiatively inefficient accretion flow
- Lack of spherical symmetry here even moreso allows for super-Eddington luminosity.


## 48
**What is the Roche potential in a binary system?**
In a binary system with a circular orbit, it is often useful to describe the system in a coordinate system that rotates along with the objects. In this non-inertial frame, one must consider centrifugal force in addition to gravity. The two together can be described by a potential (the Roche potential), so that, for example, the stellar surfaces lie along equipotential surfaces. Close to each star, surfaces of equal gravitational potential are approximately spherical and concentric with the nearer star. Far from the stellar system, the equipotentials are approximately ellipsoidal and elongated parallel to the axis joining the stellar centers. A critical equipotential intersects itself at the L1 [[Methods#Space-based detector orbits|Lagrange point]] of the system, forming a two-lobed figure-of-eight with one of the two stars at the center of each lobe. This critical equipotential defines the Roche lobes. For the situation when an object has a radius equal to or greater than the size of its hosting lobe, see [[Binaries#Roche-lobe overflow|Roche-lobe overflow]].
![[roche_potential.png]]
Above is the derived potential (skipping the derivation, though not too long, see Megans notes) and its corresponding stationary points called the [[Methods#Space-based detector orbits|Lagrange points]]. 

**Describe carefully the assumptions that go into deriving it.**
1. Nonrelativistic
2. Where matter moves relative to the co-rotating frame it will seem to be acted upon by a Coriolis force. This is not derivable from the Roche lobe model as the Coriolis force is a non-conservative force (i.e. not representable by a scalar potential)
3. Synchronous orbits (same rotation period of each individual orbit)
4. Objects are point sources

**Define the Roche limit**
The Roche limit, sometimes referred to as the Roche radius, is the distance within which a celestial body, held together only by its own gravity, will disintegrate due to a second celestial body’s tidal forces exceeding the first body’s gravitational self-attraction. A property of a two-body system, any smaller separation than the Roche limit leads to disruption of smaller body. Essentially, L1 moves to within the radius of the second body.

Inside the Roche limit, orbiting material will tend to disperse and form rings, while outside the limit, material will tend to coalesce.

Derivation: find the distance from a larger body of mass $M$ at which, for a smaller body of mass $m$ and radius $R$, the tidal forces due to the larger body exceed the self-gravity of the smaller body that holds it together (equivalent to the "L1 moving inside radius of smaller body" idea). End up with $$d_{Roche} = \alpha \left(\frac{m}{M}\right)^{1/3}R$$where $\alpha = 2^{1/3} \simeq 1.3$ in the simple derivation but accounting for fluid mechanics we have $\alpha \simeq1.4$ which is larger because disruption of a fluid body rather than a rigid body is "easier" and can take place at greater distances.
![[roche_limit_deform.jpg|500]]


## 49
**What is the Shakura-Sunyaev (alpha-disk) model for accretion disks?**
This is a relatively simple model for an accretion disk that is essentially parameterized by one parameter $\alpha$  which encodes our ignorance of the details of viscosity physics. Typically $0 < \alpha < 1$

Based on the concept that the net angular momentum of the disk itself should be conserved (see [[Accretion#Accretion disk|accretion disk]]) and when matter close to the center falls onto the body (losing angular momentum) there should be a comensurate gain in angular momentum out in the disk. That is, <mark class="hltr-pink">angular momentum is tranfserred from inner to outer parts of the disk if accretion is to occur</mark>. (Why doesnt the material just speed up and conserve angular momentum that way? I dont know). The mechanism for this transport is the viscosity, but phenomenologically we need turbulence-enhanced viscosity to explain what we see, though the microphysics is not understood.

Disk viscosity $\nu = \alpha c_s H$

The **$\mathbf{\alpha}$-disk model** is a steady-state model with fixed mass using a geometrically thin accretion disk. This results in at least 6 equations which can be solved to yield a model of the accretion disks <mark class="hltr-pink">temperature, pressure and density profiles</mark>. These are:
- Conservation of mass
- $3\times$ conservation of momentum equations (force balance)
- Conservation of energy (power generation)
- Radiative transport

Can infer more about the disk with the 2 additional equations:
- Equation of state (pressure or radiation dominated, see [[Equations of state]])
- Opacity law

Accretion assumes infalling objects start at rest and <mark class="hltr-pink">convert gravitational potential energy into luminosity</mark>. Explicitly, the change in potential energy and corresponding luminosity for an infalling mass $m$ at a distance $R$ from a central mass $M$ is $$\Delta E = \frac{GMm}{R}\quad\implies\quad L = \frac{GM\dot{M}}{R} $$**What are the assumptions that go into its derivation?**
1. Subsonic turbulence
2. Geometrically thin
3. Optically thick
4. Local thermodynamic equilibrium
5. Efficiently radiates its heat
6. Steady state (constant $\dot{M}$)
7. Self-gravity of disk neglected

where 4 and 5 relate to treating the disk as many local [[Blackbody radiation#Blackbody radiation|blackbodies]].


## 50
**Write down the fluid equations for conservation of mass and momentum that would describe a
spherically symmetric, expanding supernova remnant**

Fluid equations:
- Continuity of mass: $\frac{\partial \rho}{\partial t} + \nabla \cdot (\rho\vec{v}) = 0$
- Momentum conservation,  $\frac{\partial \vec{v}}{\partial t} + (\vec{v}\cdot\nabla)\vec{v} + \frac{1}{\rho}\nabla P = \frac{1}{\rho}\vec{f}$  where $P$ is the pressure, $\vec{f}$ is any external force, such that for gravity we have $\vec{f}_{grav} = -\nabla\Phi$ for $\Phi$ the gravitational potential
- (Not asked for) There is also energy conservation which amounts to $\frac{\partial \epsilon}{\partial t} + \nabla \cdot \left[(\epsilon + P)\vec{v}\right] = 0$ where $\epsilon = \frac{1}{2}\rho |v|^2 + \frac{3}{2}nk_BT + \rho \Phi_g$ 

Apply spherical symmetry to these equations, that is $\vec{v} = v\,\hat{r}$ and $\vec{f} = f\,\hat{r}$ to get:
- Mass: $\frac{\partial \rho}{\partial t} + \frac{1}{r^2} \frac{\partial}{\partial r}(r^2\rho v) = 0$
- Momentum $\frac{\partial v}{\partial t} + v\frac{\partial v}{\partial r} + \frac{1}{\rho}\frac{\partial P}{\partial r} = \frac{1}{\rho}f$
- Energy similar to mass
  
**How would you derive the "jump conditions" for a strong adiabatic shock?**

Basically by making simplifying assumptions and treating the problem in the frame of the moving shock discontinuity. A simplified picture of a shock is as follows, ie a rise in density up to a particular point and a discontinuity, due to the fact that the shock overdensity is moving more quickly than the medium can respond.
![[shock.png|400]]

In a frame moving with the shock front (ie moving at a speed $v_{shock} =: v_s$) we assume
- The dynamics are steady-state in this frame: $\partial/\partial t = 0$
- The radial derivativessimplify to 1D Cartesian derivatives: $\frac{1}{r}\frac{\partial}{\partial r}(r^2\,\cdot) \rightarrow \frac{d}{d x}(\cdot)$ 
- Ignore gravity and external forces: $f = 0$
- Approximate the medium past the shock front as being at rest, so in the shock front frame is moves with speed $v_{s}$ 

With this, we obtain the "Rankine–Hugoniot jump conditions":
1. From mass conservation, obtain $\frac{d}{d x}(\rho v) = 0 \implies \rho v = \text{const}$
2. From momentum conservation, obtain $\rho v \frac{d v}{d x} + \frac{d P}{d x} = 0 = \frac{d}{d x}(\rho v^2 + P) \implies \rho v^2 + P = \text{const}$
3. From energy conservation, obtain $(\epsilon + P)v = \text{const}$ 

We can do more with these but thats enough for now (see Megan and Xiaowei's notes).


## 51
**Describe the various stages of evolution of a supernova remnant. What are the relevant physical  
processes during each phase? Explain why in the Sedov-Taylor phase of a supernova remnant, the  
radius expands at $t^{2/5}$**

Basic picture is below, from Geoffrey's notes
![[sne_expansion_phases.png]]

**(1) Free expansion phase**:  |  $R\propto t$  |  lasts $\sim 100-200$ years  |  $v$ constant 
- When [[Supernovae#Supernova|SN]] first explodes, material ejected at supersonic speeds
- [[Interstellar medium#ISM|ISM]] pressure is negligible, no deceleration $\implies v=\text{const} \implies R = vt \propto t$ 
- Shock waves sweeps up and collects material from the ISM, eventually slowing down
- Expansion continues until the mass collected from ISM is about equal to the initial mass of the ejecta
- Ejected gas is [[Optical depth#Optical thickness|optically thick]] and kept hot by radioactive decay of isotopes created by the supernova.

**(2) Sedov-Taylor phase**:  |  $R\propto t^{2/5}$  |  lasts $\sim 10^4$ years  |  $E$ constant
- Ejecta is "out of steam" kinetically, expansion now an adiabatic expansion driven by thermal pressure of the hot gas
- Ejecta itself is heated by the [reverse shock](https://ned.ipac.caltech.edu/level5/March05/Dwek/Dwek3_3.html)
- Very hot ionized gas cannot efficiently radiate away energy since cooling time $\gg$ dynamical time (such that radiated heat gets absorbed and equilibriated into the system before it escapes) and therefore the expansion is at roughly constant energy (<mark class="hltr-pink">adiabatic</mark>)
- Lets derive the time-dependence of the radius in terms of the parameters $E \,(const), \rho, R,t$. 
- We could start with energy conservation, looking at the swept up ISM energy (for an ISM of constant density $\rho$) $$E_{kin} = \frac{1}{2} M v^2 = \frac{1}{2} \frac{4}{3}\pi R^3 \rho v^2$$ and the thermal energy (assuming ideal monatomic gas) where we will need the momentum conservation equation of the [[#50|Rankine–Hugoniot jump conditions]] $P\propto \rho v^2$ to obtain $$E_{th} = \frac{3}{2}Nk_B T = \frac{3}{2}PV \propto R^3 \rho v^2$$We can already see the time-dependence in both of these equations. If $R^3 v^2 \propto E/\rho = \text{const}$ then since $R^3 v^2 = R^3 \dot{R}^2 = \text{const}$ then assuming $R = t^q$ we must have that $3q + 2(q-1) = 0 \implies q=2/5$ 
- We could also note that by dimensional analysis, by using an ansatz of a "self-similar" solution (see Geoffrey's notes).

**(3) Snowplow phase**:  |  $R\propto t^{1/4}$  |  lasts $\sim 10^5$ years  |  $P$ constant 
- Ejecta and swept up mass expands and cools until [[Recombination#Recombination|recombination]] can occur between the electrons and protons to form Hydrogen ($10^6\,\pu{K}$)
- Since now more transparent to light, energy is lost to radiation and the thermal pressure decreases, slowing the expansion
- Momentum conserved (since no thermal expansion) as shock wave collects more material from ISM $p = Mv = \frac{4}{3}\pi R^3 \rho \dot{R} = \text{const} \implies R\propto t^{1/4}$ (calculation as in last part of (2) above)

**(4) Merger phase**:  |  $R\propto \text{const}$  |  End-state |  $R$ constant  
- Eventually enough ISM mass is swept up and instabilities in the gas lead to the ejecta breaking up and dissipating into the ISM. This is the stage of becoming indistinguishable from ISM material


## 52
**What is a white dwarf star?**
See [[Stellar classes#White dwarf|white dwarf]]. 

**Why is the radius of a white dwarf a decreasing function of its mass?**
We proceed via an energy minimization argument. Consider a unit mass near the radius of a WD of mass $M$ and radius $R$. Its gravitational potential energy per unit mass will be $$E_g = -\frac{GM}{R}$$and its  *non-relativistic* kinetic energy per unit mass will primarily come from the motion of electrons $$E_k = N_e\frac{p^2}{2m_e}$$where $N_e$ is the number of electrons per unit mass in this matter (there are $N_eM$ electrons in total in the WD, related to the [[Definitions - Plasma#Mean molecular weight|mean weight]] per electron via $N_e \simeq 1/(\mu_e m_H)$ where $m_H$ stands in for 1 [[Units#amu|amu]]). Since the matter is degenerate, we can take the momentum $p$ to be roughly given by the uncertainty in the momentum $\Delta p = \hbar / \Delta x$ (via Heisenberg's uncertainty principle). The quantity $\Delta x$ will be on the order of the separation between electrons, which is $n_e^{-1/3}$ for $n_e$ the number density of electrons. Since there are $N_eM$ electrons in the WD and the volume $V\propto R^3$ we have that $n_e = N_e M / V \sim N_e M/R^3$ and thus $$E_k \simeq N_e \frac{\hbar^2 n_e^{2/3}}{2m_e} \simeq M^{2/3}N_e^{5/3}\frac{\hbar^2}{2m_e R^2}$$The total energy is zero when $E_k + E_g = 0$ which yields $R \propto M^{-1/3}$, that is larger masses yield smaller radii. A rough interpretation of this is that since there is no mechanism such as fusion which can support the WD more as the mass grows, larger masses simply "push more" against the electron degeneracy pressure which is eventually overcome at the Chandrasekhar mass ($\sim 1.4\,M_\odot$) we will describe now.

<mark class="hltr-pink">The Chandrasekhar limit</mark>
As the mass of a model white dwarf increases, the typical energies to which degeneracy pressure forces the electrons (ie how far up the Fermi level is pushed) are no longer negligible relative to their rest masses. The velocities of the electrons approach the speed of light, and special relativity must be taken into account. The *relativistic* limit of the kinetic energy per unit mass is $E_{k,rel} = N_e pc$ such that via the same procedure as before one finds$$E_{k,rel} = M_{rel}^{1/3}N_e^{4/3}\frac{\hbar c}{R}$$and equating as before with the gravitational energy we find $R$ drops out completely and the relativistic limit mass, $M_{rel}$ is forced to be $$M_{rel} \simeq N_e^2\left(\frac{\hbar c}{G}\right)^{3/2} = \left(\frac{1}{\mu_e m_H}\right)^2\left(\frac{\hbar c}{G}\right)^{3/2} \simeq 1.8\, M_\odot$$To interpret this result, observe that as we add mass to a white dwarf, its radius will decrease, so, by the uncertainty principle, the momentum, and hence the velocity, of its electrons will increase. As this velocity approaches $c$, the extreme relativistic analysis becomes more exact, meaning that the mass $M$ of the white dwarf must approach this limiting mass $M_{rel}$ above. Therefore, no white dwarf can be heavier than this limiting mass, which can be evaluated via more rigorous means to be slightly lower at about $1.4\,M_\odot$, known as the Chandrasekhar limit.

| Dominant elements | Progenitor mass| Resulting WD mass | 
|:------------: | :------------: | :------------: |
|$\ce{He}$ | $0.05-1.5\,M_\odot$ | $0.1-0.4\,M_\odot$ |
|$\ce{CO}$ | $1.5-8\,M_\odot$ | $0.5-1.3\,M_\odot$ |
|$\ce{ONeMg}$ | $6-8\,M_\odot$ | $1-1.3\,M_\odot$ |






















