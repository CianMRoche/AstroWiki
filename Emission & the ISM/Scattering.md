Some good notes [here](http://spiff.rit.edu/classes/phys440/lectures/opacity/opacity.html). "Bound" and "free" refer to being either in an atomic configuration or not, respectively (I think). A highly detailed overview of all this in [this article](https://arxiv.org/pdf/1202.5949.pdf) (radiative processes in high energy astrophysics by Ghisellini)


## Electron scattering
Eslastic scattering of a photon by an electron. [[#Thomson scattering]] when non-relativistic and non-quantum, [[#Compton scattering]] otherwise


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
- The photon energy is much smaller than the mass-energy of the particle (Equivalently, the wavelength of the light is much greater than the Compton wavelength of the particle, so quantum effects can be ignored).
- Additionally, it is non-relativistic.

**Cross section**:
Important feature is that cross section is independent of frequency, and is given by $$\sigma_T = \frac{8\pi}{3}\left(\frac{q^2}{4\pi\epsilon_0 m c^2}\right)^2 = \frac{8\pi}{3}\left(\frac{\alpha \lambda_c}{2\pi}\right)^2$$where $\alpha \simeq 1/137$ is the fine-structure constant  and $\lambda_c$ is the Compton wavelength of the particle.


## Free-free emission
Also called [[Bremsstrahlung]] emission. An electron passing close to an ion feels an acceleration. An accelerating charge produces radiation. 

Important at high temperatures, where the plasma is highly ionized.

![[bremsstrahlung.png|250]]


## Free-free absorption
A free electron can *gain* energy during a collision with an ion by absorbing a photon, complementary to [[#Free-free emission]].

Must occur in presence of an ion due to [[#No isolated emission]].


## Bound-free absorption
"Ionizing absorption". If a photon has enough energy, its absorption can knock an electron free from an atom and send it off with the leftover energy in kinetic form. Partially responsible for the [[Spectra#Balmer jump]].


## Bound-bound absorption
An atom absorbs a photon and enters an excited state, but is not ionized as it is for [[#Bound-free absorption]].


## No isolated emission
An isolated particle with no internal structure cannot spontaneously emit or absorb a photon, as one cannot do so while conserving both energy and momentum.

Explanation:
- A photon has (1D) momentum $p = \hbar k = h/\lambda$
- A photon has energy $E = h\nu = hc/\lambda = pc$
- If we start with no photon and an electron of energy $E_e$ and momentum $p_e$ then working in a frame where the electron is initially at rest, using primes to denote "after collision" by energy and momentum conservation: $$\begin{align} E_e = m_ec^2 &= E_e' + |\vec{p}|c \\ \vec{p}_e = 0 &= \vec{p}_e{}' + \vec{p} \end{align}$$ we see the electron and photon after collision have equal and opposite momenta in this frame $\vec{p}_e{}' = -\vec{p}$ and $|p_e{}'| = |p|$. Which implies $$ E_e' = m_ec^2 - |\vec{p}_e{}'|c$$Filling in the relativistic kinetic energy $E_e' = c\sqrt{|\vec{p}_e{}'|^2 + m_e^2c^2}$ we get $$\sqrt{|\vec{p}_e{}'|^2 + m_e^2c^2} = m_ec - |\vec{p}_e{}'|$$This equation is $\sqrt{x^2 + y^2} = y - x$ which cannot be true for $x$ and $y$ positive by the triangle inequality (unless $|\vec{p}_e{}'| = 0$ in which case so too is the photon momentum, and nothing happens). That is, this process cannot occur if both energy and angular momentum are conserved.


## Mie scattering
Scattering of EM radiation from quasi-spherical particles where <mark class="hltr-pink">the size of the scattering particles is comparable to the wavelength of the light</mark>, rather than much smaller or much larger.

Takes place in the lower 4,500 m (15,000 ft) of the atmosphere, where many essentially spherical particles with diameters approximately equal to the wavelength of the incident ray may be present.


## Rayleigh scattering
The elastic scattering of light by spheres that are <mark class="hltr-pink">much smaller than the wavelength of light</mark>. The difference between this and [[#Thomson scattering]] is that Rayleigh scattering is scattering from polarizable entities. The incident light induces a dipole moment, which re-radiates. Thomson scattering is scattering from free unbound charged "unpolarizable" particles.

The [[Units#Intensity|intensity]] of scattered light is$$
I_\lambda(\theta)=I_0\left(\frac{1+\cos ^2 \theta}{2 R^2}\right)\left(\frac{2 \pi}{\lambda}\right)^4\left(\frac{n^2-1}{n^2+2}\right)^2\left(\frac{d}{2}\right)^6 \propto \frac{1}{\lambda^4}
$$where $I_0$ is the light intensity before the interaction with the particle, $R$ is the distance between the particle and the observer, $\theta$ is the scattering angle, $\lambda$ is the wavelength of light under consideration, $n$ is the refractive index of the particle, and $d$ is the diameter of the particle.

![[rayleigh_sunset.jpg|300]]
The change of sky colour at sunset (red nearest the sun, blue furthest away) is caused by Rayleigh scattering by atmospheric gas particles, which are much smaller than the wavelengths of visible light (since $\lambda_{blue} < \lambda_{red}$ so scattering for blue is much stronger, so the red light makes it trhough and theblue is scattered off in other directions. Also why we see blue baove us preferentially, since light passing though will be preferentially scattered down to us if its blue, largely unrelated to $\theta$-dependence). The grey/white colour of the clouds is caused by [[#Mie scattering]] by water droplets, which are of a comparable size to the wavelengths of visible light.