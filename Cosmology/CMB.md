## CMB
"Cosmic microwave background". [[Spectra#The electromagnetic spectrum|Microwave]] radiation that fills all space. It is a remnant from the epoch of [[Recombination#Recombination|recombination]] when photons in the early universe plasma could stream freely, as opposed to being [[Scattering#Thomson scattering|Thomson scattered]] by free electrons as they were before this epoch. With a standard optical telescope, the background space between stars and galaxies is almost completely dark. However, a sufficiently sensitive radio telescope detects a faint background glow that is almost uniform and is not associated with any star, galaxy, or other object. This glow is strongest in the microwave region of the radio spectrum.
![[cmb.png]]


## CMB power spectrum
We see small deviationsacross the sky ($\Delta T/T \sim 10^{-5}$) of the [[CMB#CMB|CMB]] from a perfect blackbody which result from matter under and over-densities in the early universe. To study the angular scales of these fluctuations one decomposes the Temperature signal$^1$ on the 2D sky into spherical harmonics$^2$ as in quantum mechanics when treating the hydrogen atom. 

To calculate the coefficients of the signal $\delta T = \Delta T/T$ in this basis, proceed as follows: $$\begin{align}
\delta T(\theta,\phi) = \sum_{l=0}^{\infty}\sum_{m=-l}^{+l} a_{ml} Y_{ml}(\theta,\phi)\\
a_{ml} = \int_{\rm{sky}} d\Omega\, Y_{ml}^\star(\theta,\phi)\, \delta T(\theta,\phi)
\end{align}$$Then from the orthogonality of the basis we have $$\langle a_{ml} \, a_{m'l'}^\star\rangle = \delta_{ll'}\delta_{m m'} C_l$$which can be recast as an expression for the coefficient $C_l$ for a givel $l$ averaged over the index $m$ by summing over both $l'$ and $m'$ $$C_l = \frac{1}{2l+1}\sum_{m=-l}^{+l}\langle |a_{ml}|^2 \rangle$$Making a plot of the quantity $l(l+1)C_l/2\pi$ versus $l$ (this normalization chosen just so the low $l$ side where the Sachs-Wolfe effect takes over is flat), and so the acoustic peaks are emphasized visually) we obtain the <mark class="hltr-pink">CMB power spectrum</mark>. Schematically, our measurements look like this, from Megan's notes 
![[cmb_power_spectrum_schematic.png|500]]

$^1$ The signal *after* subtracting the monopole signal arising from the motion of your detector relative to the CMB, which effectively amounts to the relative motion of the [[Galaxy groups#Local Group|local group]] relative to the rest frame of the CMB. Interestingly, fitting the CMB monopole direction (the direction we are moving in relative to CMB rest frame) gives a very different answer than other measurements, treated as another [[LCDM#LCDM|LCDM]] tension.

$^2$ Loosely, we have a discrete basis because compact spaces like the 2D sphere on the sky admit discrete decompositions, as with the spin operator in QM.


## SZ effect
[[Scattering#Inverse-Compton scattering|ICS]] of [[CMB#CMB|CMB]] photons by high-energy electrons (eg in [[Cluster media#ICM|ICM]] of a [[Galaxy clusters#Galaxy cluster|cluster]]). Only applied at very small scales (large $l$).

Two types:
- Thermal SZ: from $e^-$ temp
- Kinetic: from bulk $e^-$ motion
