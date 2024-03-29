
## The electromagnetic spectrum
- Quick conversion: $hc = 1240\,eV\,nm$ so roughly 1keV ~ 1nm since $E=hc/\lambda$
- Could also think of it as $hc \simeq 10^{-6}\,eV\,m$
 ![[EMSpectrum.png]]
 - Visible light [380,750] nm. 
 - ROY G. BIV to remember in order of increasing energy
![[opticalSpectrum.jpeg|350]]

See [[Bonus#Observing the EM spectrum|Observing EM spectrum]] for the telescopes that can observe all this.


## Redshift
$$1 + z = \frac{\lambda_{obs}}{\lambda_{emit}} = \frac{\nu_{emit}}{\nu_{obs}}$$


## OII doublet
Traces cool, ionized gas. Has been used to trace [[Cluster media#CGM|CGM]]. Ratio of two lines depends on the temperature


## H-alpha
Atomic hydrogen Balmer line, _n_ = 3 to _n_ = 2 transition. Wavelength 650 nm ~ 2eV

Emitted by many [[Nebulae#Emission nebula|emission nebulae]] and can be used to observe features in the [[The Sun#The Sun|the Sun]]'s atmosphere, including solar prominences and the chromosphere. Also by [[Emission & the ISM - Questions#73|HII regions]].

Traces star formation.


## 21cm line
Spin flip of ground state neutral hydrogen, hyperfine transition. Corresponding energy $\sim 6\, \mu \pu{eV}$ or about $1.4\,\pu{GHz}$. From Megans notes:
![[spin_flip.png|400]]
The degeneracy of the anti-aligned state is 1 since the total spin quantum number is $S = 0$ and the degeneracy is $2S+1$. For the aligned state, $S=1$ and so degeneracy is $3$.

**Observational characteristics**:
- Transition is very rare and happens on a timescale of $\sim 10\,\pu{Myr}$, but observable for very large amounts of neutral $H$ (low density to avoid collisional de-excitation) 
- Can be used to map neutral hydrogen in the "dark ages" between $z=1100$ and $z=6-20$ (ie the times between recombination and reionization) in radio wavelengths. 
- [[Observatories#CHIME|CHIME]] can observe it at low redshifts, [[Observatories#MEERKAT|MEERKAT]] also did this recently. [[Observatories#SKA|SKA]] will observe out to $z=27$ 
- Can map neutral hydrogen in spiral arms of a galaxy, and can therefore use to constrain rotation curves.
- Comes from cold gas $\implies$ little thermal broadening.
- At microwave wavelengths which pass mostly unobstructed through the atmosphere, therefore suitable for ground-based astronomy.


## Lyman-alpha forest
- Lyman series is transitions of atomic hydrogen to $n=1$ 
- Lyman-$\alpha$ is the first one ($n=2$ to $n=1$) and is $120\,\pu{nm}$
- Strong absorbtion in air, so usually done in space. Highly-redshifted sources can penetrate though

The **Lyman-$\mathbf{\alpha}$ forest** is a series of absorption lines corresponding to the absorbtion of distant background light by gas clouds at different redshifts, each absorbing at the Lyman-$\alpha$ transition in their own rest frames. In principle, the absorbtion spectrum in this case is a map of the gas between the observer and the source, including redshift information.

Each cloud absorbs the line at a wavelength $\lambda = (1+z) \lambda_0$. We corrected back to emitted wavelength in the plot below, rather than observed.

Lyman limit is the wavelength at which the hydrogen will just become ionized. 

In the below images one can see that for a close-by source, very few of the emitted wavelengths have absorption lines, but for something far away many of the wavelengths of the original spectrum will be absorbed by the time the light reaches us. (Both shown on axes of the wavelengths that they were emitted at, by dividing wavelength numbers by $1+z$)

![[Lya-forest-60.gif|400]]
![[Lyman-alpha_forest.gif]]

The Gunn-Peterson trough appears for sources which are at redshifts between [[Reionization]] and [[Recombination]], since in that period there was a lot of neutral H and all the emission is fully absorbed. 

![[gunn-peterson.jpg|350]]


## Molecular hydrogen
H doesn't have a rotational dipole, only a vibrational. Finding H2 was usually done by measuring CO with millimeter telescopes and then constraining the CO H2 correlation. Now with JWST this can be done better, since we have a mid IR IFU in space.

Doesn't have a Balmer series equivalent because the binding energy of molecular hydrogen is about 4eV, so those energies would just unbind the molecule.


## Fe k-alpha line
Fe-K$\alpha$ line (6.4 keV) AGN shows up in x-ray spectrum


## P Cygni Line Profile
Spectroscopic feature with both a blue-shifted absorption line and a broadened rest wavelength emission line arising from an expanding envelope around an ionized source
![[PCygniLineProfile.png|400]]
![[cygni.png]]


## Harvard Spectral Classification
Classifies stars into spectral type based on temperature 
- See [this page](http://astro.vaporia.com/start/spectraltype.html) for even more detail on letters that people add to spectral classes.
- Originally classes A-Q based on strength of hydrogen lines in spectra, but found that there was lots of overlap amongst categories (and also they were in the wrong order for other properties)
- Cannot distinguish between same color, same apparent magnitude, but different luminosity stars (need [[Spectra#Morgan-Keenan (MK or MKK) Luminosity Class|MK Luminosity Classification]] to distinguish between such stars)
![[HarvardSpectralClassification.png]]
- Oh Be A Fine Goat Kick Me (OBAFGKM). Note the hydrogen line strength is a gaussian at "A", mass, radius and lunimosity all decrease, and fraction of [[HR-diagram#Main sequence|MS]] stars increases. 
 ![[OBAFGKM.jpeg|250]]
 - Prominent (non-Hydrogen) spectral features of each type:

|  | O | B | A | F | G | K | M |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Prominent features | ionized $\ce{He}$ lines| neutral $\ce{He}$ lines | mostly $\ce{H}$ | metal $\ce{Ca}$ lines | strong metal lines | strong metal lines| Molecular lines, neutral metal lines |

 - Each spectral type which is further divided into 10 sub-classes depending on the absorption features present in the spectrum with 0 (hottest) through 9 (coolest). For example, the Sun has a temperature of about 5,700 Kelvin and is classified as a G2 star.


## Morgan-Keenan (MK or MKK) Luminosity Class
Stellar classification based on spectral line widths to distinguish between stars with the same color/temperature and apparent magnitude, but different luminosities/distances
- Denser objects have broader spectral lines due to increased pressure/collisional brooadening and higher surface gravity $\Delta \nu \propto n^{-1/3} =: d$ ie the interparticle separation (really some power of the interparticle separation  $\Delta \nu \propto d^{\alpha}$, and with $\alpha = 2$ the broadening is due to the coulomb field of an ionized atom or electron; this is the linear Stark effect. With $\alpha = 3$ the interaction is between neutral atoms of the same type)
- Complementary to [[Spectra#Harvard Spectral Classification|Harvard Spectral Classification]], <mark class="hltr-pink">simply adds a letter (or a few) to the existing letter-number harvard classification</mark>
![[MK.png]]
So the Sun is a **G2V** star


## Radio source
Atmosphere not too problematic, can perform radio observations even on cloudy days

**Solar system**:
- [[The Sun]]
- Jupiter 

**Galactic**:
- Galactic center
- [[Pulsars]]

**Extragalactic**
- [[Galaxies#Radio galaxy|Radio galaxies]]
- [[FRBs]] 


## X-ray background
**Sources**:
- Focused onto detector - Diffuse hot gas from Milky Way + unresolved point sources. Below 1-2keV, XRB dominates signal
- Particle BG - cosmic rays
- Unfocused cosmic hard X-ray background, constant in time

Apparently better to model your Xray background rather than to subtract it.


## Balmer Jump
Large jumps in some spectra, caused by the following pair of effects:

- [[Scattering#Bound-bound absorption|Bound-bound absorption]] transitions occur only for photons with exactly the right amount of energy
- [[Scattering#Bound-free absorption|Bound-free absorption]] transitions can absorb ANY photon with more than a critical amount of energy (ionizing energy).

Therefore, the [[Optical depth#Opacity|opacity]] of a material will increase at wavelengths shorter than one of these critical edges. That is, if we have a source light behind some material, and a particular wavelength can ionize the material, you wont see much of that light on the other side. For bound-bound though, we would just see lines.

Related to (but distinct from) the **Lyman limit**, which occurs at the wavelength which will just ionize a hydrogen atom from its ground state.


## Relativistic Doppler shift
For $\beta = v/c$ and a speed $v$ light is red or blue shifted according to: $$\frac{f_0}{f_{obs}} = \frac{\lambda_{obs}}{\lambda_0} = \sqrt{\frac{1+\beta}{1-\beta}}\simeq 1+\beta + \mathcal{O}(\beta^2)$$also implies, to first order, $$\Delta f = f_{obs} - f_0 = - \beta f_0$$meaning if the observer and source are getting closer together ($v>0$) we have that the frequency increases, and that the frequency decreases for moving away. Similarly $\Delta \lambda = \lambda_{obs} - \lambda_0 = \beta \lambda_0$ 