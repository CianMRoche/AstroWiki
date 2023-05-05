## CMB
"Cosmic microwave background". [[Spectra#The electromagnetic spectrum|Microwave]] radiation that fills all space. It is a remnant from the epoch of [[Recombination#Recombination|recombination]] when photons in the early universe plasma could stream freely, as opposed to being [[Scattering#Thomson scattering|Thomson scattered]] by free electrons as they were before this epoch. With a standard optical telescope, the background space between stars and galaxies is almost completely dark. However, a sufficiently sensitive radio telescope detects a faint background glow that is almost uniform and is not associated with any star, galaxy, or other object. This glow is strongest in the microwave region of the radio spectrum.
![[cmb.png]]


## CMB power spectrum

**Math**
We see small deviations across the sky ($\Delta T/T \sim 10^{-5}$) of the [[CMB#CMB|CMB]] from a perfect blackbody which result from matter under and over-densities in the early universe. To study the angular scales of these fluctuations one decomposes the Temperature signal$^1$ on the 2D sky into spherical harmonics$^2$ as in quantum mechanics when treating the hydrogen atom. 

To calculate the coefficients of the signal $\delta T = \Delta T/T$ in this basis, proceed as follows: $$\begin{align}
\delta T(\theta,\phi) = \sum_{l=0}^{\infty}\sum_{m=-l}^{+l} a_{ml} Y_{ml}(\theta,\phi)\\
a_{ml} = \int_{\rm{sky}} d\Omega\, Y_{ml}^\star(\theta,\phi)\, \delta T(\theta,\phi)
\end{align}$$Then from the orthogonality of the basis we have $$\langle a_{ml} \, a_{m'l'}^\star\rangle = \delta_{ll'}\delta_{m m'} C_l$$which can be recast as an expression for the coefficient $C_l$ for a givel $l$ averaged over the index $m$ by summing over both $l'$ and $m'$ $$C_l = \frac{1}{2l+1}\sum_{m=-l}^{+l}\langle |a_{ml}|^2 \rangle$$Making a plot of the quantity $l(l+1)C_l/2\pi$ versus $l$ (this normalization chosen just so the low $l$ side where the Sachs-Wolfe effect takes over is flat), and so the acoustic peaks are emphasized visually) we obtain the <mark class="hltr-pink">CMB power spectrum</mark>. Schematically, our measurements look like this, from Megan's notes (see [[Cosmology - Questions#129|this question]] for details of $\Omega_i$ effects on peaks)
![[cmb_power_spectrum_schematic.png|500]]

where the $l$ of the first peak is calculated in [[#Sound horizon size]] to be $l\sim 220$ (ie $1^\circ$) and real measurements from [[Observatories#Planck|Planck]] look like the following:
![[planck_PS.png|500]]
$^1$ The signal *after* subtracting the monopole signal arising from the motion of your detector relative to the CMB, which effectively amounts to the relative motion of the [[Galaxy groups#Local Group|local group]] relative to the rest frame of the CMB. Interestingly, fitting the CMB monopole direction (the direction we are moving in relative to CMB rest frame) gives a very different answer than other measurements, treated as another [[LCDM#LCDM|LCDM]] tension.

$^2$ Loosely, we have a discrete basis because compact spaces like the 2D sphere on the sky admit discrete decompositions, as with the spin operator in QM. In fact, depending on the paper they may may decompose into lagrange polynomials rather than spherical harmonics.


**Origin of the peaks and the sound horizon**
[source](http://background.uchicago.edu/~whu/intermediate/acoustic.html)
-   Gravity tries to compress the fluid in potential wells set by dark matter.
-   Photon pressure resists compression resulting in acoustic oscillations
-   System is equivalent to a mass on a spring falling under gravity

1. Can think of the "starting point" as at rarefaction, then gravity compresses the plasma into a gravitational potential well set by dark matter. Then the photon pressure pushes the material back out, oscillating back to the starting rarefaction point as follows
   ![[acoustic_CMB.gif|300]]
   You can think of the two balls as representing mass for springs, and as representing energy density for the early universe fluid. 
   
2. Looking at a bigger picture with multiple wells (seeded by quantum fluctuations during inflation) we have
   ![[acoustic_CMB_multiple.gif]]

3. It is also the case that it takes half as long for the fluid to compress into a potential of half the length scale, leading to oscillations twice as fast (bottom mode below). We have different modes of oscillation over different length scales which looks like 
   ![[acoustic_CMB_modes.gif]]

4. Now we can understand the power spectrum peaks:
   -   Oscillations are frozen in at [[Recombination]]
   -   Modes (and therefore length scales) caught at extrema of their oscillation represent peaks - characteristic scales with enhanced temperature fluctuations
   -   The wavenumbers (or spatial frequency) of the peaks are harmonically related to the fundamental scale - the distance sound can travel by recombination

   The scale (mode) which can reach maximum compression exactly when recombination occurs will show up as a scale over which we see large temperature fluctuations, this length scale is the **sound horizon** and its angular size sets the position of the first peak of the CMB power spectrum. See [[#Sound horizon size]] for the calculation of the size.

   Because a scale half the size oscillates twice as fast, if the sound horizon scale $l_H$ reaches exactly first compression in the time it takes to reach recombination, then $2 l_H$ will reach exactly its first rarefaction by recombination (it will reach first compression in half the time to recombination). The hormonics of $l_H$ continue in this manner, leading to the following scales observed as being those with greatest temperature fluctuation relative to the mean:
   ![[cmb_compress_rarefact.png|500]]

5. A nice way to think about this is as resonant frequencies/wavelengths in a cavity/pipe. The scale of the effective cavity $L$ is set by the time to recombination and the sound speed as $L = t_{recomb}\,v_s$, and the size admits a fundamental frequency/wavelength $\lambda_0 = 2L$  and harmonics of that frequency (unclear the exact nature of factors of 2 here). 
   ![[sound_cavity_harmonics.png|400]]

## Sound horizon size
Calculation of the size of the sound horizon relating to the [[#CMB power spectrum]]. Before [[Recombination]], the fluid pressure is dominated by [[Stars/Equations of state#Radiation pressure|Radiation pressure]] (but not necessarily a radiation-dominated universe) and so the sound speed is $$P_{rad} = \frac{1}{3}\rho c^2 \implies c_s = \sqrt{\frac{\partial P}{\partial \rho}} = \frac{c}{\sqrt{3}}$$but in fact this ignores a factor of the ratio of baryon and radiation energy densities that makes it really $\sim c/\sqrt{6}$. We can estimate the [[Distances#Comoving distance|comoving size]] of the sound horizon $\chi_s$ by the distance that sound can travel from the big bang $t = 0$ to recombination at time $t_{rc}$ $$\chi_s \simeq \int_0 ^{t_{rc}}\frac{dt}{a(t)} \, c_s \simeq \int_0 ^{t_{rc}}\frac{dt}{a(t)} \, \frac{c}{\sqrt{3}} = \frac{d_H}{\sqrt 3} \int_{z_{rc}}^\infty \frac{dz}{E(z)}$$in the language of the [[FLRW#Friedmann equation|Friedmann equation]]. If we assume matter-dominated early universe, this results in a comoving size of the sound horizon of $$\chi_s \simeq \frac{d_H}{\sqrt 3} \int_{z_{rc}}^\infty \frac{dz}{\sqrt{\Omega_M}}(1+z)^{-3/2} = \frac{2 d_H}{\sqrt{3\Omega_M}}(1 + z_{rc})^{-1/2}$$And the proper length of the sound horizon at recombination is $$L_s(z_{rc}) = a(z_{rc})\chi_s(z_{rc}) = \frac{2 d_H}{\sqrt{3\Omega_M}}(1 + z_{rc})^{-3/2}$$ the angular size of this length scale that we would measure now at $z=0$ is given in terms of the [[Distances#Angular diameter distance|angular diameter distance]] as $$\theta_s = \frac{L_s}{d_A(z_{rc})} = \frac{L_s (1+z_{rc})}{d_{sls}}$$where $d_{sls}$ is the [[Distances#Comoving distance|comoving distance]] to the surface of last scattering at $z_{rc}$  $$d_{sls}(z_{rc}) =  \frac{c}{H_0} \int_0^{z_{rc}} \frac{dz}{E(z)}$$Finally the angular size will be (see [this](https://physics.stackexchange.com/questions/54124/relation-between-multipole-moment-and-angular-scale-of-cmb) for relationship between $l$ and $\theta$)$$l_{s} \sim \frac{\pi}{\theta_s} \sim (\text{a number less than})~ 220\, $$making the assumption of a flat and matter-dominated universe. [Source](https://ned.ipac.caltech.edu/level5/Sept02/Reid/Reid5_2.html) (which doesnt have the factor of $\pi$, and has confusing notation). The reason we get a wrong answer is that our $c_s$ was too big, thus our $L_s$ and thus $\theta_s$. This leads to a "too small" $l_s$. The right answer is about $220$, see [this stackoverflow answer](https://physics.stackexchange.com/questions/450517/how-did-the-planck-study-calculate-the-angular-size-of-the-sound-horizon)


## SZ effect
[[Scattering#Inverse-Compton scattering|ICS]] of [[CMB#CMB|CMB]] photons by high-energy electrons (eg in [[Cluster media#ICM|ICM]] of a [[Galaxy clusters#Galaxy cluster|cluster]]). Biggest effect at small scales (large $l$), since this happens due to the passing of CMB photons through something like a galaxy cluster, and the  angular size of that is very small. This causes a deficit in the expected CMB signal at these scales, since the photons arent CMB [[Blackbody radiation#Blackbody radiation|blackbody]] energies anymore.
![[sz.png|500]]

Two types:
- Thermal SZ: from $e^-$ temp
- Kinetic: from bulk $e^-$ motion


1. Thermal SZ-effect
   Upscattering of [[CMB#CMB|CMB]] photons by electrons in hot, ionized gas (eg in [[Cluster media#ICM|ICM]] of a [[Galaxy clusters#Galaxy cluster|galaxy cluster]]) by [[Scattering#Inverse-Compton scattering|inverse-Compton scattering]]. Results in $\nabla T / T_{CMB}\simeq 10^{-3}$ and is redshift-independent, making it easy to detect galaxy clusters via this method for example with [[Observatories#SPT|SPT]], and can also be used to estimate cluster masses and pressure profiles. The shift moves the spectrum to higher frequencies as follows (from Megans notes)
   ![[thermal_SZ.png]]

2. Kinetic SZ-effect
   For electrons moving relative to the CMB rest frame, when they scatter as with the thermal SZ, the doppler shift due to relative motion induces a much smaller change in power (decrease in image below because the cluster is assumed to be moving away from us even beyond the Hubble flow, but can also be positive). In principle can determine peculiar velocities of the galaxy clusters; peculiar meaning 'with respect to the CMB rest frame'.
   
   Magitude of the effect is $$\frac{\nabla T}{T} = - \frac{v_p}{c}\tau$$where $v_p$ is the peculiar velocity and $\tau$ is the [[Optical depth]].

Bad quality image with some useful features:
![[kinetic_SZ.gif]]



## CMB Polarization
An overview of the polarization of CMB photons we measure
- Density perturbations ("scalar perturbations" arise from energy density fluctuations, see [these pages](https://w.astro.berkeley.edu/~mwhite/polar/node4.html) for overview) in the early universe produce **E modes** in the [[#CMB]] polarization map. Arise naturally from [[Scattering#Thomson scattering|Thomson scattering]] in a heterogeneous plasma. 
- There are also **B modes** in the CMB polarization map ("tensor perturbations" which are essentially gravitational waves). They can be created by two mechanisms: 
  1. [[Lensing#Lensing|Lensing]] of E-modes, which has been measured by the [[Observatories#SPT|SPT]] in 2013
  2. [[Gravitational waves]] arising from cosmic inflation
  
  Detecting the B-modes is extremely difficult, particularly as the degree of foreground contamination is unknown, and the weak gravitational lensing signal mixes the relatively strong E-mode signal with the B-mode signal

The names derive from an analogy to the decomposition of a vector field into curl-less  $\nabla \times \mathbf{E} = 0$ (here "E" for electric field) and divergence-less $\nabla \cdot  B = 0$ ("B" for magnetic field) components. The vector field of CMB polarization vectors on the sky is a vector field, and we decompose it (see Helmholtz decomposition) into curl-less and divergence-less components:
![[E_B_modes.png|300]]
Performing this decomposition on the CMB polarization map gives us two panels, a mock map would look like the following, where red is CMB temperature hotspots and blue is cold spots.
![[e-mode-b-mode_measurement.png]]

(Very) loosely, the B modes couple to gravitational waves because they have a quadrupole moment, but the E modes are too symetric.  