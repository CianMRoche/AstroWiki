## 72
**Discuss the various "phases" of gas in the interstellar medium. Are these phases in pressure equilibrium?**
Phases are summarized in [[Interstellar medium#ISM|this table]].

They are in pressure equilibrium if we assume no magnetic fields exist and if $n\propto T^{-1}$ for all phases (since that would imply $P$ is constant across phases by ideal gas law). Looking at the table above, we see that is approximately true, and so the phases are in pressure equilibrium.

Note that if they werent, pressure balance would cause the phases to blend into each other


## 73
**What is an HII region?**
A dense, hot region of ionized Hydrogen (HII = $\ce{H^+} \neq \ce{H_2} =$ [[Spectra#Molecular hydrogen|molecular H]]) found around hot, young stars ([[Spectra#Harvard Spectral Classification|O and B]] stars). Properties also listed in [[Interstellar medium#ISM|this table]]. Ionized by the young star. Can be observed via the [[Spectra#H-alpha|H-alpha]] line.

In galaxies, HII regions are found in:
- the arms of spiral galaxies
- chaotically in irregular galaxies
- nowhere in elliptical galaxies

**Estimate how the Stromgren radius scales with the luminosity of the ionizing source and with the ambient density**
The Stromgren radius is the radius at which the ionization rate due to the star is equal to the recombination rate. Use the following notation:
- $N$ = the number of ionizing photons produced per second by the source (units $\pu{s^{-1}}$)
- $n_x$ = number density of species $x$ (units $\pu{cm^{-3}}$)
- $\alpha$ = recombination coefficient. Quantum in nature, (units $\pu{cm^{3} s^{-1}}$ so that $\alpha\, n_1 n_2$ gives the generation rate of a neutral species from species 1 and 2 per unit volume, units $\pu{cm^{-3} s^{-1}}$). Note that this should not include contributions from recombinations to the ground state, as this will release a photon that can again ionize another H atom.
- $R_s$ = Stromgren radius

Then, assuming the source has no volume, that all gas is hydrogen (so that $n_e = n_H = n$), that $\alpha$ is a constant and considering a sphere of radius $R_s$
- Ionizing rate = $N$ (really I think this should be something like $Ne^{-R_S/l}$ where $l$ is the [[Optical depth#Mean free path|mean free path]] and $N$ is the rate of ionizing photons coming from the source but maybe we take a simple case)
- Recombination rate = $\alpha n^2 \, \frac{4}{3}\pi R_s^3$

Equating the two gives $$R_s = \left(\frac{3N}{4\pi \alpha n^2}\right)^{1/3}$$Now relate $N$ to the ionizing luminosity via the [[Units#Luminosity|specific luminosity]] $L_\nu$ and the energy of a photon of frequency $\nu$ (which is $h\nu$) $$N = \int_{13.6\,\pu{eV}}^{\infty}d\nu\, \frac{L_\nu}{h\nu}$$where the lower limit is the ionization energy of hydrogen, since any photon of energy lower than this will not contribute to our analysis. Assuming we have some luminosity $L$ we can identify $N\propto L$ and thus $R_s \propto L^{1/3}$.


## 74
**Explain what bremsstrahlung radiation is Draw a typical bremsstrahlung spectrum**
See [[Bremsstrahlung]] (and [[Scattering#Free-free emission|free-free emission]], which is another name for the same thing)

**From what kinds of astrophysical objects is such radiation observed?**
X-ray Sources:
- [[Galaxy clusters#Galaxy cluster|Galaxy clusters]] and the [[Cluster media#ICM|ICM]] at $T\sim 10^{7-8}\,\pu{K}$
- Coronal gas in the [[Interstellar medium#ISM|ISM]] $T\sim 10^{6}\,\pu{K}$
- [[The Sun#The Sun|Solar]] corona $T\sim 10^{6}\,\pu{K}$

Also see [[#73|HII regions]] in optical to radio bremsstrahlung.


## 75
**What is synchrotron radiation? Draw a typical synchrotron spectrum**
See [[Magnetobremsstrahlung#Synchrotron radiation|synchrotron radiation]].

**From what kind of astrophysical objects is such radiation observed?**
- Jets in [[Binaries#X-ray binary|XRBs]] and [[AGN#AGN|AGN]] (apprently seen in radio?)
- [[Supernovae#Supernova|SNe]] remnants
- [[Pulsars#Pulsar|Pulsar]] wind [[Nebulae]]
- Galactic [[Interstellar medium#ISM|ISM]] 
- Sunspots
- [[GRBs#GRB|GRBs]] 

**How can the synchrotron spectrum be used to constrain the age of the source?**
[[Magnetobremsstrahlung#Synchrotron radiation|Synchrotron radiation]] from a many-particle system with some power law distribution of particle energies will have a roughly power-law shape. Since the power emitted for the higher-energy particles is larger than that for lower-energy ($dE/dt \propto E^2$), unless energy is injected into the system, an old synchrotron source will have a break at large energies, and an even older source will have a break at lower energies. From Megan's notes:

![[synchrotron_age.png]]


## 76
**What is meant by "free-free" absorption? How is this different from electron scattering?**
See [[Scattering#Free-free absorption|free-free absorption]]. 

Difference from electron scattering (which is [[Scattering#Compton scattering|Compton scattering]] at high energies and [[Scattering#Thomson scattering|Thomson scattering]] at low energies) is that in this scenario a photon is "lost" whereas in electron scattering it's just "redirected".


## 77
**What is the Saha equation and how is it used in stellar structure calculations?**
See [[Saha equation]]. 

Use in stellar structure:
- We know the spectrum of a star is directly related to the relative numbers of atoms and ions it contains because each atom or ion can absorb or emit radiation of a particular set of wavelengths. 
- Saha equation tells us the relative populations of ionization levels, and for the simplest inference, what fraction of atoms are not ionized
- Ratio of Boltzmann factors for energy levels of the unionized species tell us relative populations of those energy levels
- A spectrum has absorption and emission lines depending on composition, and the strength of those lines is strongly dependent on temperature since the relative populations of levels depends on temperature. 
- As a result, the presence and strength of lines used to [[Spectra#Harvard Spectral Classification|classify stars]] are effectively a classification of composition and temperature.


## 78
**Explain, from a statistical mechanics point of view, why the Balmer lines are most prominent in A stars with an effective temperature of 10$^4\,\pu{K}$**
Big picture: 
- Balmer series (transitions to first excited ($n=2$) state of atomic Hydrogen) most strongly seen in [[Spectra#Harvard Spectral Classification|A-type]] stars ($7500-10000\,\pu{K}$) because:
- Using the Saha equation we can work out how many atoms are unionized as a function of $T$
- Using ratios of Boltzmann factors, we can work out how many atoms are in the $n=1,2,3,\dots$ states
- It turns out that as a function of temperature, the fractional occupancy of the $n=2$ energy level spikes at $10^4\,\pu{K}$, meaning at this temperature we see the most transitions to this level.
- Intuitively, above this temperature the Hydrogen is mostly ionized (since ionization energy is just above the $n=2$ energy level) and below this temperature most things are in the ground state ($n=1$), so Lyman lines, not Balmer.

Basically $$\text{Balmer lines} \propto \frac{n_{\text{energy level } 2}}{n_{\text{total}}} = \underbrace{\frac{n_{\text{energy level } 2}}{n_{\text{unionized}}}}_{\text{Boltzmann factor}}  \underbrace{\frac{n_{\text{unionized}}}{n_{\text{total}}}}_{\text{Saha}} $$
Calculation:
- Hydrogen only has a single ionzed level (since it only has one electron to "give"). $n_{total} = n_{I} + n_{II}$ where the roman subscripts refer to $\rm{HI}$ and $\rm{HII}$, the unionized and singly-ionized states of Hydrogen, respectively. Using the simplified Saha equation defined [[Saha equation|here]] for a single-ionization, we have $$\frac{n_e^2}{n - n_e}=\frac{2}{\lambda^3} \frac{g_1}{g_0} \exp \left[-\frac{\epsilon}{k_B T}\right]$$Identifying $n_e = n_{II}$ and $n = n_{total}$ and using the linked table for the degeneracies, this simplifies to $$\frac{n_{II}^2}{n_{tot} - n_{II}}=\frac{1}{\lambda^3}\exp \left[-\frac{\epsilon}{k_B T}\right]$$Skipping the algebra, this gives us the ratio of ionized to total ($n_{II}/n_{tot}$ RHS above in "basically..."), and unionized ratio $n_I/n_{tot}$ is just $1-n_{II}/n_{tot}$.
- $n_{I}$ can be broken down into $n_I = n_1 + n_2 + \dots$ where the subscript refers to the energy level. Using that $E_j = E_0 / j^2 = (-13.6\,\pu{eV})/j^2$ and $g_j = 2j^2$ (2 spin states, $j^2$ states per spin due to degeneracy in other quantum numbers) for atomic Hydrogen, the relative population of level $2$ to level $j$ is $$\frac{n_2}{n_j} = \frac{g_2}{g_j}e^{\frac{-(E_2 - E_j)}{kT}}$$We can then calculate the population of energy level 2 to all other energy levels (we are essentally calculating the boltzmann factor) $$\frac{n_2}{n_{tot}} = \left[\frac{n_{tot}}{n_{2}}\right]^{-1} = \left[\sum_{j=1}^\infty\frac{g_j}{g_2}e^{\frac{-(E_j - E_2)}{kT}}\right]^{-1}$$Putting this together with the above gives us an expression for how many hydrogen atoms we have in the energy level 2 as a function of temperature, which ends up looking like this:
  
![[balmer_fraction.png|300]]


## 79
**Explain how interstellar dust grains can result in linear polarization of transmitted light. How is the direction of polarization related to the average direction of the interstellar magnetic field (as projected on the plane of the sky)?**
- [[Dust]] grains are not all spherical, and therefore can a nonzero average alignment due to an external magnetic field. This alignment will be "long axis $\perp$ $B$" since as the grain rotates, it will have an effective dipole moment, see diagram below. This dipole moment will align with the external field over time, the energy dissipation mechanism being a subject of much work. Review [here](https://ntrs.nasa.gov/api/citations/20200001522/downloads/20200001522.pdf)
  ![[grain_align.png]]
- This alignment is <mark class="hltr-pink">paramagnetic</mark> (the net alignment of independent random spins with an external magnetic field) not ferromagnetic, since the inter-spin interctions are very weak. 
- The grains will then be preferentially aligned to have their long axis perpendicular to the external magnetic field.
- Light passing through a cloud of such dust will be preferentially absorbed along the long axes of the grains, and since those long axes are aligned perpendicular to the external field. Thus, the light coming out the other side will be polarized in the direction of the magnetic field (since the component orthogonal to that will be largely attenuated).
![[dust_polarization.jpg]]
- This absorption heats up the (on average aligned) dust grains and they will then emit a polarized [[Blackbody radiation#Blackbody radiation|blackbody]] spectrum 

**What major discovery in 2014 was derailed by this phenomenon?**
The [[Observatories#BICEP|BICEP2]] team claimed they had measured B-mode polarization in the [[CMB#CMB|CMB]] (evidence for primordial gravitational wave signals during inflation), but further analysis (for example by [[Observatories#Planck|Planck]]) and data revealed that the signal could be entirely produced by polarized thermal emission from [[Milky Way]] dust.

For dust at $\sim 20\,\pu{K}$ via [[Blackbody radiation#Wien's displacement law|Wiens law]] we have $\lambda_{peak} = 150\,\mu\pu{m}$ ([[Spectra#The electromagnetic spectrum|infrared]]). Apparently the BICEP signal was at $150 \,\pu{GHz} \sim 2\,\pu{mm}$ so by Wiens law this would correspond to a temperature on the order of $1\,\pu{K}$? There is some $\sim 1-10\,\pu{K}$ dust in the Milky Way but its mostly between $20$ and $200\,\pu{K}$. !UNFINISHED


## 80
**Explain the physics of 21 cm radio emissions from neutral hydrogen atoms.**
See [[Spectra#21cm line|21cm line]]. 


## 81
**Qualitatively describe the "equipartition energy" of a synchrotron source**
In a [[Magnetobremsstrahlung#Synchrotron radiation|synchrotron]] source (ie relativistic charged particles in an approximately uniform magnetic field) there are two relevant energy densities, that of the particles $U_E$ (synchrotron emission mostly in relativistic electrons, but other species also contribute to this energy density) and that of the magnetic field $U_B$. 

The idea here is that the equipartition principle suggests that the lowest energy configuration for the system is to "distribute its energy equally across all degrees of freedom", that is roughly speaking, to have equal energy densities in both the magnetic field and the particles. 

Lets look at both in the context of their dependence on the magnetic field $B$. The magnetic energy density is fairly straight-forward as $$U_B = \frac{B^2}{2\mu_0}$$for $\mu_0$ the permeability of free space. The particle energy density is a bit more involved. Consider the minimum magnetic field necessary to produce a synchrotron spectrum of a given [[Units#Luminosity|luminosity]] $L$. Skipping the [math (section 5.4.1)](https://www.cv.nrao.edu/~sransom/web/Ch5.html) we get for the energy density of the electrons which produced this synchrotron radiation only: $$U_e \propto L B^{-3/2}$$The total energy density of the particles is then $U_E = (1+\eta)U_e$ where $\eta$ is the ion/electron energy ratio ($\eta\simeq 40$ for cosmic rays collected near Earth). The total energy as a function of magnetic field then looks like a very sharp drop toward the $B$ where both energy densities take approximately the same value (doing the math the minimum is at $U_E/U_B = 4/3$).
![[equipartition.png|450]]

**What can we learn about cosmic rays from this?**
See [[Cosmic rays#Cosmic rays|cosmic rays]] for definition.

Radio astronomers often assume [[Magnetobremsstrahlung#Synchrotron radiation|synchrotron]] sources are in equipartition because:
- It is physically plausible; systems with interacting components often tend toward equipartition
- Via the math we skipped, if one knows the luminosity of a synchrotron source we can obtain an estimate of the magnetic field. If we know that, then via equipartition we can obtain an estimate of the magnetic and particle energy densities of the source, in the end resulting in an estimate of the cosmic ray energy (even if we dont know $\eta$ very well, can get within an order of magnitude or two).
- There is an "energy problem" for large extragalactic radio sources which would require enormous total energies to explain their luminosities (eg [[Lightning round#168|Cyg A]]). The "least bad" this problem can be is when equipartition is assumed, at which the total energy for a givem $L$ is minimized.


## 82
**What kinds of sources are detected at TeV energies?**
See Xiaowei's notes for much more detail.
1. [[AGN#AGN|AGN]] and [[AGN#Blazar|blazars]] (some similar mechanisms in [[Binaries#X-ray binary|XRBs]])
   In jets electrons are accelerated and can spiral around internal magnetic field lines, creating [[Magnetobremsstrahlung#Synchrotron radiation|synchrotron]] radiation which is then [[Scattering#Inverse-Compton scattering|inverse Compton-scattered]] to higher and higher energies
2. [[GRBs#GRB|GRBs]]
   Details in [[Compact objects - Questions#67|Q67]] but basically the same mechanism as in point 1.
3. [[Supernovae#Supernova|Supernova]] remnants
   Shock fronts in SN explosions are efficient particle accelerators (thought to be main source of [[Cosmic rays#Cosmic rays|cosmic rays]]). [[Scattering#Inverse-Compton scattering|Inverse Compton-scattering]] again. Similar mechanisms in [[Pulsars#Pulsar|pulsar]]-wind [[Nebulae#Nebula|nebulae]] like in the Crab nebula (see [[Compact objects - Questions#62|Q62]], some of that energy accelerates particles in the nebula)
4. [[Galaxies#Starburst galaxy|Starburst galaxies]]
   Stars in these galaxies have relatively short lifetimes, lots of supernovae, ideal environment for cosmic ray production

**What is the “cosmic gamma ray horizon”?**
TL;DR it's the energy and redshift-dependent [[Optical depth#Mean free path|mean free path]] for cosmic rays due to background light in the universe. About $2\,\pu{Gpc}$ away from us.

- The light emitted by stars and Active Galactic Nuclei that permeates the Universe constitutes the <mark class="hltr-pink">Extragalactic Background Light</mark> (EBL). It is a sea of photons that were emitted by these sources and reprocessed by the interstellar medium (gas and dust) of the host galaxy.  
- When a high energy photon coming from a source far away traverses the EBL, there is some probability that it will interact with EBL photons through a process called two-photon pair-production, the annihilation of the two photons and subsequent production of a pair of particle-antiparticle. This means that some of those energetic photons will not arrive at our telescopes, i.e., the high-energy photon flux from distant sources is attenuated by the EBL. 
- Because the density of EBL photons depends on [[Spectra#Redshift|redshift]] (the average rate of star formation is different at different epochs in the Universe), the probability of pair-production depends on redshift. It also depends on energy of the photon: the total energy must surpass the rest energy of the particles created. The easiest barrier to surpass is the rest mass of an electron-positron pair, since these have tiny masses. Because photons in the EBL typically have lower energies than the electro-positron rest mass, you need a very high energy photon to interact with a low-energy photon from the EBL to produce one such pair.
- Given the probability of interaction, there will be a maximum effective distance that a high-energy photon can travel before before it encounters an EBL photon. That is, the universe will have some [[Optical depth]] for such high energy photons due to the EBL $$I_{out} = I_{in} e^{-\tau}$$The cosmic γ-ray horizon (CGRH) is the energy/distance at which the optical depth $\tau$ is equal to unity and it is a function of redshift and energy. That is, it's the energy and redshift-dependent [[Optical depth#Mean free path|mean free path]] for cosmic rays due to background light in the universe.
 - Current measurements place it at $z\simeq 0.5$ away from us ($\sim 2\,\pu{Gpc}$)


## 83
**Why is the gas in the interstellar medium largely transparent at visible wavelengths? How does the transparency of the ISM depend on wavelength in the optical and near-IR, and why?**
The [[Optical depth#Opacity|opacity]] of the [[Interstellar medium#ISM|ISM]] has many sources, ignoring emissions from the ISM we have
- [[Scattering#Bound-bound absorption|Bound-bound absorption]] which leads to absorption lines at specific energies, but does not attenuate the whole continuum
- [[Scattering#Bound-free absorption|Bound-free absorption]] from the ionization of primarily hydogen, leading to absorption lines at $\sim 13.6\,\pu{eV}$ which is in the [[Spectra#The electromagnetic spectrum|UV]] 
- [[Scattering#Free-free absorption|Free-free absorption]] and [[Scattering#Electron scattering|electron scattering]] which both require ionized gas to occur (such as that in the hot coronal [[Interstellar medium#ISM|ISM]] component) but the density of this component is too low to contribute significantly to opacity.
- $\rm{H}^-$ opacity (when a Hydrogen picks up another electron to fill its 1s orbital) requires neutral $\rm{H}$ and free electrons, which can happen with partially ionized metals in a solar atmosphere.

But overall not much opacity in the ISM, except for [[Dust#Dust|dust]] which absorbs in the optical/UV and re-emits thermally in the IR. The wavelength dependence of the optical depth is (from Megans notes, actually unclear if $\lambda$ increases to the left or right, or if the labels are in the right places).

![[extinction_ISM.png]]


## 84
**Sketch a typical cooling function L(T) for diffuse interstellar gas and identify its prominent features, spanning from IR to X-ray. Overplot a hypothetical heating curve and show how to identify points of thermal equilibrium and their stability.**

Cooling takes place via (for example)
- Collisionally excited line emission
- Recombination
- Thermal [[Bremsstrahlung#Bremsstrahlung|bremsstrahlung]]

The <mark class="hltr-pink">cooling function</mark> $\Lambda (T)$ in units of $[\pu{J m^3 s^{-1}}]$ is such that $R = n^2 \Lambda$ is the energy per volume per time released by gas cooling where $n$ is the number density.

The cooling curve from Megan's notes: (units are $\pu{erg cm^3 s^{-1}}$ (?) but i think some negatives are missing and im not sure about the $n_H$s)
![[cooling_vs_T.png]]

There is also a <mark class="hltr-pink">heating function</mark> labelled $\Gamma(T)$ in units of $[\pu{J s^{-1}}]$ such that $n\Gamma (T)$ is the energy injected into the ISM per volume per time. Why defined with different units? Not sure. The sources are 
- [[Cosmic rays]] 
- photoionization 
- photoelectric heating from [[Dust]] grains

![[heating_vs_T.png]]

Thermal equilibrium is then defined by the zeros of the generalized loss function$$\mathcal{L}(T) =  n^2\Lambda (T) - n\Gamma(T) = 0$$and stability of a particular equilibrium point (red and blue below) depends on the derivative at those points
- If you perturb temperture a bit to the left (lower temp) from the blue dots below, $\mathcal{L}$ is negative and thus more heating than cooling, $T$ returns back to where it was. Same thing on the right but for heating, therefore they're stable
- If you do this for the red point, going a little left means $\mathcal{L}$ positive and thus more cooling than heating, and thus temperature continues to decrease. Same on right side
![[ISM_stability.png|600]]
- Therefore stability determined by sign of derivative of $\mathcal{L}$ via$$\begin{align}\frac{\partial \mathcal{L}}{\partial T}\Big\vert_{\text{equilibrium point}} >0 \quad &\implies \quad \text{stable} \\ \frac{\partial \mathcal{L}}{\partial T}\Big\vert_{\text{equilibrium point}} <0 \quad &\implies \quad \text{unstable}\end{align}$$

## 85
**What is "brightness temperature"?**
Brightness temperature is the temperature at which a [[Blackbody radiation#Blackbody radiation|blackbody]] would be reproduce the observed [[Units#Intensity|specific intensity]]. Rearranging the blackbody spectrum to get $T$ and labelling it $T_\nu$ (and using the label $I_\nu$ instead of $B_\nu$ to emphasize that the system is not a perfect blalckbody) we have $$T_\nu = \frac{h\nu}{k_B\ln\left(1+\frac{h\nu^3}{c^2I_\nu}\right)}$$in terms of the "blackbody" specific intensity $I_\nu$. This measure of specific intensity is commonly used in radio astronomy (low-frequency or "Rayleigh-Jeans" limit) wherein the blackbody spectrum reduces to $$I_\nu \simeq \frac{2\nu^2k_B T}{c^2} \implies T_\nu \simeq \frac{c^2I_\nu}{2k_b \nu^2}$$**What is a “Jansky”? How are these different?**
A Jansky is a unit of  [[Units#Flux|specific flux]] (that is, not per steradian as for a brightness temperature).

If you measure a specific flux $F_\nu$ (which can be expressed in Janskys) with your detector that has a field of view of $\Omega$ steradians, then $F\nu / \Omega$ is a brightness temperature.


## 86
**Make a simple, classical argument to show that the spectrum of radiation from monoenergetic electrons with a speed v impinging on ions at an impact parameter b would be roughly flat up to a frequency ~ v/b.**

Consider the acceleration of a nonrelativistic charge $q$ with mass $m$ scattering from an ion (labelled "nucleus" here but means an ion assumes to have charge $-q$, though not a necessary assumption)
![[ion_scatter.png|500]]
The [[Magnetobremsstrahlung#Larmor formula|Larmor formula]] tells us the power emitted due to the acceleration, which varies, so the power will also vary, but we assume the speed is $v$ uniform in the region of interest where most power is emitted (near closest approach) $$a(r) = \frac{F(r)}{m} = \frac{q^2}{m\,4\pi \epsilon_0 r^2} = \frac{q^2}{m\,4\pi \epsilon_0}\frac{1}{(vt)^2 + b^2} = \frac{q^2}{m\,4\pi \epsilon_0 b^2}\left[1+\left(\frac{t}{\tau}\right)^2\right]^{-1}$$where $r$ is the distance between the particles and $\tau = b/v$. Thus the power is $$P = \frac{q^2a^2}{6\pi \epsilon_0 c^3}  \propto \left[1+\left(\frac{t}{\tau}\right)^2\right]^{-2} $$Timescale over which we emit radiation is $\tau = b/v$, in that faster electrons give a shorter pulse of radiation, and so too does a closer approach. This is really the smallest timescale since $\tau \downarrow \implies P \downarrow$ and there arent really charges moving here on timescales smaller than this. (if you dont like this argument, see the explicitly calculated fourier transform below).

The spectrum (loosely energy per frequency, really a distribution) is the Fourier transform of the power (energy per time). A minimum timescale corresponds to a maximum frequency, which here will be $\nu = v/b$ above which the spectrum (fourier transform of the power) will drop to zero. One can actually calculate the Fourier transform to be more precise and get something like $$\rm{FT}[P(t)] = P(\omega) \propto e^{-\tau \omega}$$in the region of validity near $\omega = 2\pi\nu = 2\pi/\tau$ . So once we get to a frequency of $1/\tau$ the spectrum decays exponentially. This however doesnt explain why its flat before that !UNFINISHED


## 87
**If a typical interstellar dust grain is 0.2 microns in size, and starlight suffers an extinction of 1 magnitude per kpc, estimate the space density of dust grains.**

Assume only absorption and no emission, so that via the [[Optical depth#Mean free path|Lambert-Beer law]] light is attenuated as it passes through medium as $F = F_0e^{-\tau}$ via some [[Optical depth#Optical depth|optical depth]] $\tau$. [[Magnitudes#Apparent magnitude|Apparent magnitude]] differences due to differences in observed [[Units#Flux|flux]] $F$ between emission at "$0$" and observation at a distance $d$ are given by $$\begin{align}\Delta m = m_d - m_0 &= -2.5\log _{10}\left(\frac{F_d}{F_0}\right) \\ &= -2.5\log _{10}\left(e^{-\tau}\right)\\ &= -2.5\log _{10}\left(e^{-n\sigma d}\right)\\ &= -2.5 \left({-n\sigma d}\right)\log _{10}(e)\end{align}$$Where we choose to write $n\sigma d$ in place of $N\sigma$ as in [[Optical depth#Optical depth|optical depth]] since we are interested in getting a volume density, not a column density, and we assume the material is uniform over the distance $d$. If we rearrange we can get $$n = \frac{\Delta m}{2.5\,\sigma d \log_{10}(e)}$$We know that for $d=1\,\pu{kpc}$ we have $\Delta m = 1$. We can approximate the scattering cross section $\sigma$ as completely classical scattering if the wavelength of light is much smaller than the size of the grain. With this $$n = \frac{1}{2.5\,\pi(0.2\,\pu{\mu m})^2 (1\,\pu{kpc}) \log_{10}(e)}\sim 10^{-12}\,\pu{cm^{-3}}$$

## 88
**What are the Einstein A and B coefficients for a spectral line, and what are the relationships
among them?**
The Einstein coefficients are a measure of the probability that an atom/molecule/ion will undergo emission or absorption.
| Atomic Process | Reaction | Einstein coefficient | Units |
| --- | ----------- | -------------| -------------|
| Spontaneous emission |  $E_2 \rightarrow E_1 + h\nu$ | $A_{21}$ | $\pu{s^{-1}}$ |
| Absorption | $h\nu + E_1 \rightarrow E_2$ | $B_{12}$ | $\pu{s^{-1}\,(\text{specific intensity})^{-1}}$ |
|Stimulated emission | $h\nu + E_2 \rightarrow E_1 + 2h\nu$ | $B_{21}$ | $\pu{s^{-1}\,(\text{specific intensity})^{-1}}$ |

Note the units of [[Units#Intensity|specific intensity]] since those processes depend on the photon "density". We break them up into $A$ and $B$ coefficients via
- $A$ doesnt depend on what light is around
- $B$ does

Then $A_{21} n_2$ (for $n_2$ the volume number density of particles in energy state $E_2$) is the transition rate for spontaneous emission per unit volume, and for [[Units#Intensity|specific mean intensity]] $J_\nu$ the transition rate per volume for absorption is $B_{12}n_1 J_\nu$ (similar for stimulated emission). Putting this together we have in thermal equilibrium that transitions into second level should equal transitions down to first, ie $$\begin{align}
\text{transitions } \uparrow \quad &=\quad \text{transitions } \downarrow \\
B_{12}n_1 J_\nu \quad &= \quad B_{21}n_2 J_\nu + A_{21} n_2
\end{align}$$We can obtain relative populations of excited states by ratios of Boltzmann factors $$\frac{n_2}{n_1} = \frac{g_2}{g_1}e^{\frac{-(E_2 - E_1)}{kT}}$$Combining the balance equation (divided across by $n_1$) with the Boltzmann factor above and solving for $J_\nu$ one finds $$J_\nu = \frac{\left(\frac{A_{21}}{B_{21}}\right)}{\left(\frac{g_1B_{12}}{g_2B_{21}}\right)e^{\frac{h\nu}{kT}} - 1}$$For a thermal process we have that $J_\nu$ is the [[Blackbody radiation#Blackbody radiation|blackbody]] spectrum (labelled $B_\nu$ in reference to emphasize that its for a blackbody, and isotropic so $J_\nu = I_\nu$) $$J_\nu(\nu\,;T) = \frac{\mathcal{F}(\nu)}{e^{\frac{h\nu}{kT}} - 1}\quad,\quad\mathcal{F}(\nu):= \frac{2h\nu^3}{c^2}$$
Matching these two equations we get $$\frac{A_{21}}{B_{21}} = \mathcal{F}(\nu)\quad,\quad \frac{B_{12}}{B_{21}} = \frac{g_2}{g_1}$$which are known as the <mark class="hltr-pink">Einstein relations</mark> that guarantee if we know one of the numbers, we know all 3. Note that the resulting equations hold even out of equilibrium, but since we derived them using thermal equilibrium I am confused.


## 89
**Explain quantitatively why stimulated emission is important and spontaneous emission is usually ignored in the radio domain, whereas the reverse is true in the optical domain.**

Compare the rates of stimulated and spontaneous emission. Using [[#88|Q88]] we have $$R = \frac{\text{stimulated rate per volume}}{\text{spontaneous rate per volume}} = \frac{B_{21}n_2J_\nu}{A_{21}n_2} = \frac{c^2}{2h\nu^3}J_\nu$$If we assume a [[Blackbody radiation#Blackbody radiation|blackbody]] this reduces to $$R = \left(e^{\frac{h\nu}{k T}} - 1\right)^{-1}$$For [[Spectra#The electromagnetic spectrum|radio]] wavelengths, for a blackbody with peak in the radio at $1\,\pu{m}$ we have $T\sim \pu{mK}$ via [[Blackbody radiation#Wien's displacement law|Wiens law]] and so $kT\sim 10^{-7}\,\pu{eV}$ and $h\nu \sim 10^{-6}\,\pu{eV}$. Therefore via $e^x \simeq 1 + x$ for $x$ small we have $R = kT/h\nu \gg 1$ and thus stimulated is dominant over spontaneous. 

For [[Spectra#The electromagnetic spectrum|optical]] wavelengths ($\nu$ large, similar argument) so $R \simeq e^{-h\nu/kT} \ll 1$ and thus spontaneous is dominant over stimulated. 

**Given a thermal spectrum at some temperature T, at what frequency would the two emission rates be equal?**
Equal contributions means $R=1$ and so$$R = 1 \implies e^{\frac{h\nu}{kT}} = 2 \implies \nu = \frac{kT}{h}\ln(2)$$

## 90
**Name five molecules found in the interstellar medium and comment on how they are detected. What limits our ability to directly detect the most common molecules in the ISM?**

Detection mechanisms: lines in spectra
- Rotational transitions which produce emission/absorption lines, mostly in [[Spectra#The electromagnetic spectrum|microwave/radio]]. Dipole transitions are low-energy.
- Vibrational transitions which do the same, mostly in [[Spectra#The electromagnetic spectrum|mid to far-IR]]  

1. $\ce{H_2}$ ([[Spectra#Molecular hydrogen|molecular hydrogen]], vibrational) is the most abundant molecule, but is symmetric and has no rotational modes and doesnt have emission/absorption lines  in [[Spectra#The electromagnetic spectrum|optical or radio]] at the typical temperatures in the [[Interstellar medium#ISM|ISM]] where it is found, so we almost never detect this directly. It does have lines in the UV, which have been observed by a spectrograph on a rocket. Instead, the ratio between $\ce{CO}$ luminosity and $\ce{H_2}$ mass is thought to be constant, so we infer its presence from the next molecule:
2. $\ce{CO}$ (carbon monoxide, rotational transitions) is next most abundant by a factor of $\sim 10^4$. Because of its asymmetry, this polar molecule produces far brighter spectral lines than the hydrogen molecule, making $\ce{CO}$ much easier to detect. It is now used as a tracer of interstellar gas in [[Galaxies]]
3. $\ce{CH_4}$ (methane, vibrational)
4. $\ce{NH_3}$ (ammonia, vibrational)
5. $\ce{H_2O}$ (water, vibrational)
6. About 50 other detected molecules, including $\ce{HCN, H_2CO}$ (formaldehyde) $\ce{OH}$ etc...