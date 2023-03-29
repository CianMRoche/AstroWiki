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
For BH of mass $M$, orbital frequency (via [[Binaries#Circular motion|circular motion]]) is $$\Omega_{\rm{ISCO}}^2 = \frac{GM}{R_{\rm{ISCO}}^3}$$And the radius goes as (See [[Black holes#ISCO|ISCO]] for helpful plot at a particular mass)$$R_{\rm{ISCO}} = \alpha \frac{GM}{c^2}$$where $\alpha$ is a spin-dependent factor that has the following limiting cases: $$a = \cases{-1\quad\text{(retrograde, maximal)} \\ 0\quad\text{(Schwarzschild)} \\ +1\quad\text{(prograde, maximal)}} \implies \alpha = \cases{9 \\ 6 \\ 1}$$so $\alpha$ and thus $R_{\rm{ISCO}}$ decreases as relative spin (so retrograde is considered "less spin") is increased. Since $$\Omega_{\rm{ISCO}} \sim \frac{1}{\alpha^{3/2}M}$$ we have that:
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


## 49
**What is the Shakura-Sunyaev (alpha-disk) model for accretion disks?**


**What are the assumptions that go into its derivation?**











## 71
**Sketch the frequency distribution of the emission of a typical QSO from radio to X-ray frequencies.**

