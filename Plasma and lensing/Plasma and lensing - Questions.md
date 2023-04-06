## 91
**What is "Faraday rotation"?**
When the presence of a magnetic field (along the direction of propagation) causes the polarization vector of light to rotate. 

A schematic for the effect is as follows, where the rotation angle $\beta$ of the polarization vector depends on both $d$ and $B$ as $\beta \propto B d$  
![[faraday_rotation.png|400]]
The Faraday effect is caused by left and right circularly polarized waves propagating at slightly different speeds, a property known as "circular birefringence". Since a linear polarization can be decomposed into the superposition of two equal-amplitude circularly polarized components of opposite handedness and different phase, the effect of a <mark class="hltr-pink">relative phase shift</mark>, induced by the Faraday effect, is to rotate the orientation of a wave's linear polarization.

**How is it used in astronomy?**
We can use this to measure astrophysical <mark class="hltr-pink">magnetic fields</mark> in the following way: First define a "rotation measure" $\mathcal{R}$ by $$\mathcal{R} = \frac{e^3}{8\pi^2 \epsilon_0 m_e^2 c^4} \int_0^d dz \,n_e(z) B_{||}(z)$$in SI units, where $z$ is the coordinate along the direction of propagation, $n_e$ is the electron density and $B_{||}$ is the component of the magnetic field along $\hat{z}$. Then $\beta$ is relates to $\mathcal{R}$ via $$\beta = \mathcal{R}\lambda^2$$that is, it is a wavelength-dependent effect, having the largest effect at large wavelengths like [[Spectra#The electromagnetic spectrum|radio]] waves, and so this is often used in studies of [[FRBs]] and [[Pulsars#Pulsar|pulsars]]. The polarization angles $\theta$ we measure as a function of wavelength are then $$\theta (\lambda) = \theta_{\text{intrinsic to source}} + \mathcal{R}\lambda^2$$As a result, we can use measurements of $\theta(\lambda)$ at many frequencies and do something like a parametric fit to determine the intrinsic polarization and quantities like $B_{||}$ or $n_e$. In fact we can use it to constrain $B$ more reliably, since $n_e$ can be determined from the *dispersion measure* (see [[#92|Q92]]).


## 92
**What is “dispersion measure” for electromagnetic waves in a plasma?**
A basic overview is:
- Ionized material along the direction of propagation of light will change the refractive index. 
- This refractive index is frequency-dependent (some details in [[#93|Q93]]).
- If we shine a spectrum of many frequencies through an ionized region, the light which experiences a lower refractive index will exit first (speed is $v = c/n$ for refractive index $n$).
- This leads to a frequency-dependent time delay between light of different frequencies, and the further the light travels through an ionized medium, or the denser the medium, the greater the effect.
- The <mark class="hltr-pink">dispersion measure</mark> quantifies this dispersion of light by integrating the free electron density along the direction of propagation, and thus is effectively a column density.

We define it as $$\rm{DM} = \int_0^d dz\, n_e(z)$$and the time delay as a function of frequency of light can be derived from the group velocity (relates to [[#93]] but details skipped here, derivation in Megans notes if anyone wants to copy it in) $$t(\nu) = \rm{DM} \frac{\rm{k}_{\rm{DM}}}{\nu^2}$$where we have defined the dispersion constant $$\rm{k}_\rm{DM} = \frac{e^2}{2\pi m_e c} \simeq 4.15 \,\pu{GHz^2 pc^{-1} cm^3 ms}$$That is, <mark class="hltr-pink">a higher frequency will be delayed less, and a lower frequency delayed more</mark>. The delay between a high frequency $\nu_{high}$ and a low frequency $\nu_{low}$ and is $$\Delta t = t(\nu_{low}) -t(\nu_{high})  = \rm{k_{DM}\,DM}\left(\frac{1}{\nu_{low}^2} - \frac{1}{\nu_{high}^2}\right)$$**How is it used in astronomy?**
The problem is we usually dont know when all the light was emitted, so we cant measure a single time delay. Instead we use the differences in arrival times $\Delta t$ between two frwquencies, and use that to determine the electron density $n_e$ (or really the column density).

Has been used in [[FRBs#FRB|FRBs]] to demonstrate they must be extragalactic. shape of galactic "cone" thingy just because moving away from latitude 0 is moving out of the disk, so less material, so dispersion measure gets smaller. This shows a stark difference between FRB dispersion measures and things we see out of the disk in the [[Milky Way]]. Note that knowing the distance to a galactic pulsar (blue below) we can get an estimate of the column density, or vice versa.
![[frb_dm.jpg]]


## 93
**What is the physical significance of the plasma frequency?**
The plasma frequency is the most fundamental time-scale in plasma physics. <mark class="hltr-pink">It sets the timescale over which charges in a plasma relax</mark>. If light enters a plasma and has a frequency much slower than the plasma frequency, the plasma has enough time to react and the light will be reflected by the plasma. Similarly if the light is much higher frequency than this timescale, the plasma cant keep up, and the light passes unattenuated.

There is a different plasma frequency for each species. However, the relatively fast electron frequency is, by far, the most important, and references to "the plasma frequency'' typically mean the electron plasma frequency. $$\omega_p = \sqrt{\frac{ne^2}{\epsilon_0 m}}$$**Derivation**
This can be derived from Maxwell's equations, or by considering the restoring force when displacing a charge species in a plasma. Take a cubic slab of area $A$ on each side, composed of positive charges and negative charges, each with a number density $n$. Displace one species by a distance $\delta x$ in the $x$ direction and you'll end up with a net negative charge on one side $$Q = \frac{\text{charge}}{\text{particle}}\frac{\text{particles}}{\text{volume}}\text{volume} = q\,n\, (A\delta x)$$And thus a surface charge density $$\sigma = \frac{Q}{A} = q\,n\,\delta x$$We will have an equal but opposite surface charge density on the other side. We have effectively made the classic "two charged parallel plates" of electromagnetism, the electric field between which is $$E = -\frac{\sigma}{\epsilon_0}$$Then just look at Newton's second law to get $$m\frac{d^2 (\delta x)}{dt^2} = q E = -m\,\omega_p^2\,\delta x$$where we strategically define the *plasma frequency* $\omega_p$ as above. This is just a simple harmonic oscillation for the displacement of charges from quasi-neutrality at a frequency $\omega_p$. We can thus think of this frequency as the (inverse) timescale over which charges in a perturbed quasi-neutral plasma return themselves to quasi-neutrality.

**Interaction with electromagnetic waves**
The nature of electromagnetic waves in a plasma is made precise by the dispersion relation $$\omega^2(k) = \omega_p^2 + c^2 k^2$$whose derivation we will skip, and which results in the group velocity for EM waves $$v_g := \frac{d\omega}{dk} = \dots = c\sqrt{1 - \left(\frac{\omega_p}{\omega}\right)^2}$$which is imaginary (attenuation) for $\omega < \omega_p$ and approaches $c$ for $\omega \gg \omega_p$.


## 94
**What are the three types of MHD waves in a magnetized plasma?**
For derivation of dispersion relation in idealized MHD (magnetohydrodynamics) can see Megan's notes. 

1 & 2: <mark class="hltr-pink">Magnetosonic waves</mark>
Can think of as sound waves (longitudinal) in the density of magnetic field lines. Has two versions:
- Fast magnetosonic - when plasma pressure and magnetic field are <mark class="hltr-grey">in phase</mark>
- Slow magnetosonic - when plasma pressure and magnetic field are <mark class="hltr-grey">out of phase</mark>

Would look something like (Geoffrey's notes)
![[magnetosonic.png|]]

3: <mark class="hltr-pink">Alfvén waves</mark> 
A transverse wave in the magnetic field (ie propagates in the direction of the magnetic field) whose restoring force is magnetic tension (a restoring force that serves to straighten out bent magnetic field lines). 

Would look something like (Megan's notes)
![[alfven.png|300]]

**Are magnetic fields important in the propagation of waves in the interstellar medium? In a star?**
- [[Interstellar medium#ISM|ISM]]: Yes $\rightarrow$  mainly due to [[#91|Faraday rotation]] 
- Stars: Yes $\rightarrow$  Alfvén waves are primary mechanism for heating of stellar corona and accelerating stellar winds.Have also been seen in shockwaves in [[Supernovae#Supernova|SNe]] remnants.