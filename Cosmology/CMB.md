## CMB
"Cosmic microwave background". [[Spectra#The electromagnetic spectrum|Microwave]] radiation that fills all space. It is a remnant from the epoch of [[Recombination#Recombination|recombination]] when photons in the early universe plasma could stream freely, as opposed to being [[Scattering#Thomson scattering|Thomson scattered]] by free electrons as they were before this epoch. With a standard optical telescope, the background space between stars and galaxies is almost completely dark. However, a sufficiently sensitive radio telescope detects a faint background glow that is almost uniform and is not associated with any star, galaxy, or other object. This glow is strongest in the microwave region of the radio spectrum.
![[cmb.png]]


## CMB power spectrum

**Math**
We see small deviations across the sky ($\Delta T/T \sim 10^{-5}$) of the [[CMB#CMB|CMB]] from a perfect blackbody which result from matter under and over-densities in the early universe. To study the angular scales of these fluctuations one decomposes the Temperature signal$^1$ on the 2D sky into spherical harmonics$^2$ as in quantum mechanics when treating the hydrogen atom. 

To calculate the coefficients of the signal $\delta T = \Delta T/T$ in this basis, proceed as follows: $$\begin{align}
\delta T(\theta,\phi) = \sum_{l=0}^{\infty}\sum_{m=-l}^{+l} a_{ml} Y_{ml}(\theta,\phi)\\
a_{ml} = \int_{\rm{sky}} d\Omega\, Y_{ml}^\star(\theta,\phi)\, \delta T(\theta,\phi)
\end{align}$$Then from the orthogonality of the basis we have $$\langle a_{ml} \, a_{m'l'}^\star\rangle = \delta_{ll'}\delta_{m m'} C_l$$which can be recast as an expression for the coefficient $C_l$ for a givel $l$ averaged over the index $m$ by summing over both $l'$ and $m'$ $$C_l = \frac{1}{2l+1}\sum_{m=-l}^{+l}\langle |a_{ml}|^2 \rangle$$Making a plot of the quantity $l(l+1)C_l/2\pi$ versus $l$ (this normalization chosen just so the low $l$ side where the Sachs-Wolfe effect takes over is flat), and so the acoustic peaks are emphasized visually) we obtain the <mark class="hltr-pink">CMB power spectrum</mark>. Schematically, our measurements look like this, from Megan's notes 
![[cmb_power_spectrum_schematic.png|500]]

And real measurements from [[Observatories#Planck|Planck]] look like 
![[planck_PS.png|500]]
$^1$ The signal *after* subtracting the monopole signal arising from the motion of your detector relative to the CMB, which effectively amounts to the relative motion of the [[Galaxy groups#Local Group|local group]] relative to the rest frame of the CMB. Interestingly, fitting the CMB monopole direction (the direction we are moving in relative to CMB rest frame) gives a very different answer than other measurements, treated as another [[LCDM#LCDM|LCDM]] tension.

$^2$ Loosely, we have a discrete basis because compact spaces like the 2D sphere on the sky admit discrete decompositions, as with the spin operator in QM.


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

   The scale (mode) which can reach maximum compression exactly when recombination occurs will show up as a scale over which we see large temperature fluctuations, this length scale is the **sound horizon** and its angular size sets the position of the first peak of the CMB power spectrum.

   Because a scale half the size oscillates twice as fast, if the sound horizon scale $l_H$ reaches exactly first compression in the time it takes to reach recombination, then $2 l_H$ will reach exactly its first rarefaction by recombination (it will reach first compression in half the time to recombination). The hormonics of $l_H$ continue in this manner, leading to the following scales observed as being those with greatest temperature fluctuation relative to the mean:
   ![[cmb_compress_rarefact.png|500]]

5. A nice way to think about this is as resonant frequencies/wavelengths in a cavity/pipe. The scale of the effective cavity $L$ is set by the time to recombination and the sound speed as $L = t_{reion}\,v_s$, and the size admits a fundamental frequency/wavelength $\lambda_0 = 2L$  and harmonics of that frequency (unclear the exact nature of factors of 2 here). Then $\lambda_0$ is 
   ![[sound_cavity_harmonics.png|400]]



## SZ effect
[[Scattering#Inverse-Compton scattering|ICS]] of [[CMB#CMB|CMB]] photons by high-energy electrons (eg in [[Cluster media#ICM|ICM]] of a [[Galaxy clusters#Galaxy cluster|cluster]]). Only applied at very small scales (large $l$).

Two types:
- Thermal SZ: from $e^-$ temp
- Kinetic: from bulk $e^-$ motion


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