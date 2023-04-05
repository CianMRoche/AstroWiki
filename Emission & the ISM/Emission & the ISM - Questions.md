## 72
**Discuss the various "phases" of gas in the interstellar medium. Are these phases in pressure equilibrium?**
Phases are summarized in [[Interstellar medium#ISM|this table]].

They are in pressure equilibrium if we assume no magnetic fields exist and if $n\propto T^{-1}$ for all phases (since that would imply $P$ is constant across phases by ideal gas law). Looking at the table above, we see that is approximately true, and so the phases are in pressure equilibrium.

Note that if they werent, pressure balance would cause the phases to blend into each other


## 73
**What is an HII region?**
A dense, hot region of ionized Hydrogen (HII = $\ce{H^+} \neq \ce{H_2}$) found around hot, young stars ([[Spectra#Harvard Spectral Classification|O and B]] stars). Properties also listed in [[Interstellar medium#ISM|this table]]. Ionized by the young star. Can be observed via the [[Spectra#H-alpha|H-alpha]] line.

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
- Ionizing rate = $N$
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
As described (poorly) in [[Magnetobremsstrahlung#Synchrotron radiation|synchrotron radiation]] the energetic processes in these nonthermal plasmas happen in a manner proportional to some power of the energy while accelerations are happening. Since energy losses are proportional to some power of the energy !UNFINISHED (i dont get this, see geoffrey 136)


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