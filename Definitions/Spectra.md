
## The electromagnetic spectrum
- Quick conversion: $hc = 1240\,eV\,nm$ so roughly 1keV ~ 1nm since $E=hc/\lambda$
- Could also think of it as $hc \simeq 10^{-6}\,eV\,m$
 ![[EMSpectrum.png]]
 - Visible light [380,750] nm. 
 - ROY G. BIV to remember in order of increasing energy
![[opticalSpectrum.jpeg|350]]


## Redshift
$$1 + z = \frac{\lambda_{obs}}{\lambda_{emit}} = \frac{\nu_{emit}}{\nu_{obs}}$$


## Blackbody radiation
Black body spectral power density [interactive](https://phet.colorado.edu/sims/html/blackbody-spectrum/latest/blackbody-spectrum_en.html) with units power/(surface area of "emitter" $\cdot$ solid angle of "detector" $\cdot$ frequency) $\pu{J s^{-1}Hz^{-1}m^{-2}}$
$$B_\nu(\nu\,;T) = \frac{2h\nu^3}{c^2}\frac{1}{e^{\frac{h\nu}{kT}} - 1}$$
But can also reforumulate in terms of wavelength. To do the conversion, need to remember that this is a density and perform a change of variables under the integral sign. 
$$\int d\nu B_\nu(\nu;T) = \int d\lambda \underbrace{\frac{d\nu}{d\lambda}}_{= \frac{d}{d\lambda}\frac{c}{\lambda} = -\frac{c}{\lambda^2}}B_\nu(\nu;T) \implies B_\lambda(\lambda;T) = \frac{c}{\lambda^2}B_\nu\left(\frac{c}{\lambda};T\right)$$
where we drop the minus sign because we integrate in the opposite direction for $\lambda$ so the definition of $B_\lambda$ is nice. 

**When redshifted**:
Effective temperature gets redshifted as $$T_{obs} = \frac{T_{emit}}{1+z}$$Why? When you redshift the blackbody spectrum in a constantly proportional way $\nu_{emit} \rightarrow \nu_{obs} = c\nu_{emit}$ for all $\nu$ (here $c = (1+z)^{-1}$, see [[Spectra#Redshift|redshift]]) it has the effect of introducing an effective temperature $T_{eff} = T_{emit}/(1+z)$ so redshifts maintain the BB spectrum form with a different temperature $$\mathrm{BB}\sim\exp\left(\frac{h\nu}{kT}\right) \longrightarrow \exp\left(\frac{h\nu}{k(1+z)T}\right)$$ where the RHS is what we observe. $$\implies (1+z) T_{obs} = T_{emit}$$
**Wien's displacement law**:
The wavelength at which the spectrum has its peak is inversely proportional to temperature
$$\lambda_{peak} \propto \frac{1}{T}$$
but the constant of proportionality depends on the solution of an implicit equation. A good reference point is $$\lambda_{peak} \simeq \frac{3}{T\,[K]}\,\pu{mm}$$
such that at room temp, peak is at ~10 microns. 

**Stefan-Boltzmann Law**:
Obtained by integrating over solid angle, area and frequency, $L$ in units of $\pu{W} = \pu{J s^{-1}}$
$$L = \underbrace{\frac{2\pi^5 k^4}{15 h^3 c^2}}_{\colon = \sigma} A T^4$$
where we have defined the Stefan-Boltzmann constant $\sigma$


## Hertzsprung-Russel diagram
This diagram demonstrates the clustering between the [[HarvardSpectralClassification.png|color]] (temperature) of stars to their intrinsic luminosity ([[Magnitudes#Absolute magnitude|absolute magnitude]])
![[HRDiagram.png|]]


## Main sequence
A line (and thus, evolutionary track) that can be identified on the [[#Hertzsprung-Russel diagram]] which comprises ~90% of known stars, including the [[Objects#The Sun|Sun]]. 


## OII doublet
Traces cool, ionized gas. Has been used to trace [[Object Types#CGM|CGM]]. Ratio of two lines depends on the temperature


## H$\alpha$
Atomic hydrogen Balmer line, _n_ = 3 to _n_ = 2 transition. Wavelength 650 nm ~ 2eV

Emitted by many [[Object Types#Emission Nebula|emission nebulae]] and can be used to observe features in the [[Objects#The Sun|Sun]]'s atmosphere, including solar prominences and the chromosphere


## Molecular hydrogen
H doesnt have a rotational dipole, only a vibrational. Finding H2 was usually done by measuring CO with millimeter telescopes and then constraining the CO H2 correllation. Now with JWST this can be done better, since we have a mid IR IFU in space.

Doesnt have a Balmer series equivalent because the binding energy of molecular hydrogen is about 4eV, so those energies would just unbind the molecule.


## P Cygni Line Profile
Spectroscopic feature with both a blueshifted absorption line and a broadened rest wavelength emission line arising from an expanding envelope around an ionized source
![[PCygniLineProfile.png|400]]


## Harvard Spectral Classification
- Classifies stars into spectral type based on temperature 
- Originally classes A-Q based on strength of hydrogen lines in spectra, but found that there was lots of overlap amongst categories (and also they were in the wrong order for other properties)
- Cannot distinguish between same color, same apparent magnitude, but different luminosity stars (need [[Spectra#Morgan-Keenan (MK or MKK) Luminosity Class|MK Luminosity Classification]])
![[HarvardSpectralClassification.png]]
- Oh Be A Fine Goat Kick Me (OBAFGKM). Note the hydrogen line strength is a gaussian at "A", mass, radius and lunimosity all decrease, and fraction of [[#Main sequence]] stars increases. 
 ![[OBAFGKM.jpeg|250]]


## Morgan-Keenan (MK or MKK) Luminosity Class
Stellar classification based on spectral line widths to distinguish between stars with the same color/temperature and apparent magnitude, but different luminosities/distances
- denser objects have broader spectral lines due to increased pressure/collisional broadening and higher surface gravity
- complementary to [[Spectra#Harvard Spectral Classification|Harvard Spectral Classification]]
![[MK.png]]


## Radio source
Atmosphere not too problematic, can perform radio observations even on cloudy days

**Solar system**:
- The [[Objects#The Sun|Sun]] 
- Jupiter 

**Galactic**:
- Galactic center


## X-ray background
**Sources**:
- Focused onto detector - Diffuse hot gas from Milky Way + unresolved point sources. Below 1-2keV, XRB dominates signal
- Particle BG - cosmic rays
- Unfocused cosmic hard X-ray background, constant in time

Eric Miller(?MIT?) - Model your Xray BG, dont subtract it.