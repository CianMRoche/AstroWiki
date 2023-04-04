## 72
**Discuss the various "phases" of gas in the interstellar medium. Are these phases in pressure equilibrium?**
Phases are summarized in [[Interstellar medium#ISM|this table]].

They are in pressure equilibrium if we assume no magnetic fields exist and if $n\propto T^{-1}$ for all phases (since that would imply $P$ is constant across phases by ideal gas law). Looking at the table above, we see that is approximately true, and so the phases are in pressure equilibrium.

Note that if they werent, pressure balance would cause the phases to blend into each other


## 73
**What is an HII region?**
A dense, hot region of ionized Hydrogen found around hot, young stars ([[Spectra#Harvard Spectral Classification|O and B]] stars). Properties also listed in [[Interstellar medium#ISM|this table]]. Ionized by the young star. Can be observed via the [[Spectra#H-alpha|H-alpha]] line.

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