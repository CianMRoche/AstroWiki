Some good notes [here](http://spiff.rit.edu/classes/phys440/lectures/opacity/opacity.html). "Bound" and "free" refer to being either in an atomic configuration or not, respectively (I think).


## Compton scattering
The scattering of a high frequency photon after an interaction with a charged particle, usually an electron, which decreases the photon energy (otherwise [[#Inverse-Compton scattering]]), since part of the energy of the photon is transferred to the recoiling electron.
![[compton.jpg]]

The energies of the photon and electron (which sum to a constant) as a function of angle from initial photon direction is as follows, showing that there is essentially no energy is lost by photons which remain travelling in the same direction (makes sense) but a large transfer of energy for those photons scattered back in the direction they came from.
![[compton.png]]


## Inverse-Compton scattering
When a low-energy photon is scattered to a higher energy by a high-energy electron, complementary to [[#Compton scattering]]. The cause of the following astrophysical effects:

- Sunyaev-Zeldovich effect in [[Galaxy clusters|galaxy cluster]] studies, whereby photons from the [[CMB#CMB|cosmic microwave background]] move through the hot gas surrounding a galaxy cluster, and are inverse Compton upscattered to higher energies.
- The [[Accretion#Accretion disk|accretion disk]] surrounding a [[Black holes#Black hole|black hole]] is presumed to produce a thermal spectrum. The lower energy photons produced from this spectrum are scattered to higher energies by relativistic electrons in the surrounding corona. This is surmised to cause the power law component in the X-ray spectra (0.2–10 keV) of accreting black holes, as in [[Compact objects - Questions#71|Q71]].
- The gamma-ray emission in [[GRBs#GRB|gamma-ray bursts]] is also hypothesized to result from upscattering within the ultrarelativistic jet. See [[Compact objects - Questions#67|Q67]].


## Thomson scattering
AKA "electron scattering" or [[#Compton scattering]] at low energies. It is the elastic scattering of electromagnetic radiation by a free charged particle, as described by classical electromagnetism (not necessarily an electron).

A single, isolated electron cannot absorb a passing photon (see [[#No isolated emission]]), but it can scatter it into some other direction. 

This classical treatment of the electron-photon scattering makes the following assumptions:
- Elastic scattering
- The photon energy is much smaller than the mass-energy of the particle
- Equivalently, the wavelength of the light is much greater than the Compton wavelength of the particle.

**Cross section**:
Important feature is that cross section is independent of frequency, and is given by $$\sigma_T = \frac{8\pi}{3}\left(\frac{q^2}{4\pi\epsilon_0 m c^2}\right)^2 = \frac{8\pi}{3}\left(\frac{\alpha \lambda_c}{2\pi}\right)^2$$where $\alpha \simeq 1/137$ is the fine-structure constant  and $\lambda_c$ is the Compton wavelength of the particle.


## Free-free emission
Also called [[Bremsstrahlung]] emission. An electron passing close to an ion feels an acceleration. An accelerating charge produces radiation. 

Important at high temperatures, where the plasma is highly ionized.

![[bremsstrahlung.png|250]]


## Free-free absorption
A free electron can *gain* energy during a collision with an ion by absorbing a photon, complementary to [[#Free-free emission]].

**Examples**: 
- Electron scattering: photons scatter off free electrons. 
  This is called [[#Thomson scattering]] for low energies, and [[#Compton scattering]] at high energies.


## Bound-free absorption
"Ionizing absorption". If a photon has enough energy, its absorption can knock an electron free from an atom and send it off with the leftover energy in kinetic form. Partially responsible for the [[Spectra#Balmer jump]].


## Bound-bound absorption
An atom absorbs a photon and enters an excited state, but is not ionized as it is for [[#Bound-free absorption]].


## No isolated emission
An isolated particle with no internal structure cannot spontaneously emit or absorb a photon, as one cannot do so while conserving both energy and momentum.

Not typing the math here yet. The algebra is [here](https://physics.stackexchange.com/questions/225522/free-electron-cant-absorb-a-photon) for example.