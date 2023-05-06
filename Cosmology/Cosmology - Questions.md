The start of cosmology is super super dense. I recommend reviewing [[FLRW]] first, and keep in mind that the order of the questions is a bit backwards in places. You will find that the answer to question $n$ often depends on something like $n+2$ and $n+5$, and in such a case its personal preference whether you go in order or jump around as needed.


## 126
**Summarize the state of the experimental field of 21cm cosmology and what it hopes to accomplish.**

See [[Spectra#21cm line|21cm line]] for explanation of line physics. 

What is the use of this line in studying cosmology? 
- Can use this transition to map the fraction of Hydrogen which is neutral over cosmic time, which tells us about the [[Reionization#Epoch of reionization|epoch of reionization]]. ![[neutral_hydrogen.png|500]]
- As [[CMB#CMB|CMB]] photons pass through a neutral hydrogen region, those photons near $21\,\pu{cm}$ wavelengths can be absorbed by neutral hydrogen. See [these slides](https://www2.yukawa.kyoto-u.ac.jp/~ppp.ws/PPP2015/slides/takahashi.pdf).

What experiments can do this?
- [[Observatories#CHIME|CHIME]]. Also can measure [[BAO#BAO|BAO]] signal with these measurements. Has only observed the 21cm cosmological signal when temperature maps are correlated with [[AGN#Quasar|quasar]] maps and the CHIME images stacked to increase signal to noise.
- [[Observatories#HERA|HERA]]. Can allow us to study first stars and epoch of reionization. Will place limits on 21cm power spectrum and thus our understanding of how ionized bubbled form and evolve. More robust against astrophysical foreground, but still need accurate foreground models in all cases to see any signal at all
- [[Observatories#MWA|MWA]] and [[Observatories#SKA|SKA]] similar.

For all these, the astrophysical foreground (eg [[Magnetobremsstrahlung#Synchrotron radiation|synchrotron]] from galactic sources like jets in [[Binaries#X-ray binary|XRBs]] and [[AGN]], [[Supernovae#Supernova|Sne]] remnants, [[Nebulae#Pulsar wind nebula|pulsar wind nebulae]], galactic [[Interstellar medium|ISM]] and [[GRBs]]) is orders of manitude bigger than the cosmological signal, makes for very, very hard post-processing. Haochen Wang here at MKI does this.


## 127
**Summarize the state of the experimental CMB field and what it hopes to accomplish.**
A brief history of [[CMB#CMB|CMB]] observation is as follows:

1965 
- Penzias and Wilson discover the CMB as a $4.2\,\pu{K}$ excess antenna temperature
- Had been predicted by Alpher and Herman in 1948 but didnt gain much traction
- Won 1978 Nobel prize

1980
- Some limits placed on CMB inhomogeneities in part by soviet experiment RELKIT-1

1992
- NASA launches [[Observatories#COBE|COBE]] which measured CMB anisotropy at $\Delta T/T \simeq 10^{-5}$ 
- Essentially measured the low-$l$ (Megan's notes says high $l$? unclear, below image suggests low $l$ is correct) flat part of the [[CMB#CMB power spectrum|CMB power spectrum]]
- Won 2006 Nobel prize

2001
- NASA launches [[Observatories#WMAP|WMAP]] which measured out to the third peak of the [[CMB#CMB power spectrum|CMB power spectrum]]

2013
- NASA launches [[Observatories#Planck|Planck]] which had better angular resolution than any previous instrument, lead to extremely precise power spectrum.

2014
- [[Observatories#BICEP|BICEP2]] announces detection of B mode [[CMB#CMB Polarization|CMB polarization]] and claim this is evidence of inflationary gravitational waves. Later revealed that [[Dust#Dust|dust]] was the real culprit, see [[Emission & the ISM - Questions#79|Q79]].

There has been a number of ground-based and balloon experiments since, but the main results are summarized below. 

![[cmb_comparison.png]]

The best measured quantities today are:
1. The almost perfect CMB [[Blackbody radiation#Blackbody radiation|blackbody]] spectrum which has peak at $T=2.73\,\pu{K}$. The anisotropies are on the order of $\Delta T/T \sim 10^{-5}$ which corresponds to temperature differences of about $30\,\pu{\mu K}$ that result from matter under and over-densities in the early universe.
2. The [[CMB#CMB power spectrum|CMB power spectrum]] 

Whats left to measure: Primarily actual detection of the B-mode [[CMB#CMB Polarization|polarization]], which informs primordial [[Gravitational waves]] from the big bang. 


## 128
**What are the anisotropies in the CMB? How do their amplitudes depend on angular scale?**

The anisotropy, or directional dependency, of the [[CMB#CMB|cosmic microwave background]] signal is divided into two types: **primary anisotropy**, due to effects that occur at the surface of last scattering (the spherical shell on the sky so photons are now received that were originally emitted at [[Recombination#Recombination|recombination]]) and before; and **secondary anisotropy**, due to effects such as interactions of the background radiation with intervening hot gas or gravitational potentials, which occur between the last scattering surface and the observer. These effects have an impact on the shape of the [[CMB#CMB power spectrum|CMB power spectrum]].

Explaining the <mark class="hltr-pink">primary anisotropies</mark>: 
1. Non-integrated Sachs-Wolfe effect ($l\lesssim 100$)
   - Photons in a grav. well get redshifted climbing out of it (sort of like [[Galaxies - Questions#113|violent relaxation]])
   - Caused by gravitational [[Spectra#Redshift|redshift]] occurring at the surface of last scattering. 
   - The effect is not constant across the sky due to differences in the matter/energy density at the time of last scattering, such that deeper potential wells lead to more reddened photons, and thus apparently lower [[Blackbody radiation#Blackbody radiation|blackbody]] peak temperaure via [[Blackbody radiation#Wien's displacement law|Wien's law]] (can also think of the peak wavelength being redshifted to longer values). 
   - From Tegmark (1995): potential well also leads to time dilation, and so photons from deeper wells are actually from earlier times and therefore hotter (bluer). On larger scales this effect is proportional to the time of last scattering gravitational potential.

2. Acoustic oscillations ($100\lesssim l\lesssim 1000$)
   See [[BAO#BAO|BAO]].

3. Silk damping ($l\gtrsim 1000$)
   "photon diffusion damping" which washes out scales smaller than $l=1000$ ($\lesssim 0.1^\circ$, around the third acoustic peak)
   - [[Recombination#Recombination|Recombination]] $\implies$ photons can "suddenly" travel much farther
   - These photons carry energy from the hot regions and diffuse to the cold regions, also dragging baryons around, such that any anisotropy on a very small scale is quickly washed out. Effect is strongest for smallest scales (largest $l$)
   - The *silk scale* is distance scale over which photon diffusion is important at $z=1100$, so about $3\,\pu{Mpc}$ when using an angular scale measured now of $0.1^\circ$. The mass contained within the scale is the *Silk mass* which we estimate to be $\sim 10^{13}\,M_\odot$, i.e. about the mass of a [[Galaxies#Galaxy|galaxy]] today 😱. Smaller scales (and smaller masses) are washed out.
   - There also exists electron diffusion damping for the same reasons but it is far weaker since the electrons couldnt diffuse nearly as far.

Explaining the <mark class="hltr-pink">secondary anisotropies</mark>: 
1. Integrated Sachs-Wolfe effect
   Same thing as non-integrated but can blueshift if photon passes through a well thats shallowing or redshifted if passing through a well thats deepening.
2. [[Scattering#Thomson scattering|Thomson scattering]] (isotropic and scale-independent)
3. [[CMB#SZ effect|SZ effect]] 
4. [[Lensing]]
   Large scale structure can lens the CMB
5. Late-time integrated Sachs–Wolfe effect -  dark energy?

Theres also the [[CMB#CMB Polarization|CMB polarization]] signal.


## 129
**What are acoustic peaks in the CMB power spectrum? What do their locations and amplitudes tell us?**

Lets look at the [[CMB#CMB power spectrum|CMB power spectrum]] (explanation of origins of peaks found there). Megans notes are great, here is mostly just those:
![[CMB_PS_cosmological_params.png]]

Using the relative densities $\Omega_i$ defined in the context of the [[FLRW]] metric and [[FLRW#Friedmann equation|Friedmann equation]], changing the $\Omega_i$ has the following effects on the power spectrum:

1. $\Omega_k$
   Changes the scale we measure these peaks on, since we measure angular sizes of these length scales and angles change with curvature. If the length scale is $L$, the angular size in and open/flat/closed universe is $\theta_{o/f/c}$ and the multipole moment corresponding to its angular size is $l_{o/f/c}$ then we would see: 
   - Open ($\Omega_k >0$, like hyperbolic space) $\implies$ angle we measure is smaller, $l_o$ big
   - Flat ($\Omega_k =0$, flat space) $\implies$ angle we measure is simple, $l_f$ intermediate
   - Closed ($\Omega_k <0$, like a sphere) $\implies$ angle we measure is bigger, $l_c$ small

   That is, $l_c < l_f < l_o$. Think of it like "in an open universe, a cone opens up between you and the object, so the cone angle at the tip where you are is thinner" and converse for a closed universe. 
   ![[omega_k.png]]

2. $\Omega_M$
   Essentially "the more matter there is, the faster we reach [[Recombination]]" and if we reach recombination faster, there is less time for structure to grow in the early universe, and we see weaker power across the whole spectrum. Similarly less matter means stronger structure.

3. $\Omega_b$
   Baryons (or ordinary matter) load down the photon-baryon plasma and add inertial (and gravitational) mass to the oscillating system. 
 
   Their effect on the acoustic peaks is as follows.  Remember what happens when you add mass to a spring and let it fall in the gravitational field of the Earth.  With more mass loading the spring, it falls further before pulled back by the spring.  On the other hand, it rebounds to the same position it started from. 
   
   Since the odd numbered (first, third, fifth...) acoustic peaks are associated with how far the plasma "falls" into gravitational potential wells (how much the plasma compresses), they are enhanced by an increase in the amount of baryons in the universe.   The even numbered peaks (second, fourth, sixth) are associated with how far the plasma "rebounds" (how much the plasma rarefies).  Thus with the addition of baryons the odd peaks are enhanced over the even peaks.  For example, baryons make the first acoustic peak much larger than the second.  The more baryons the more the second peak is relatively suppressed. If we had almost no baryons at all, the first two peaks would be about the same size 
   ![[omega_b.png]]

4. $\Omega_\Lambda$
   Seems we define it as $\Omega_\Lambda = 1-\Omega_k - \Omega_M - \Omega_r$ but I thought the fact that they all sum to 1 was confusing? Not sure. If we assume $\Omega_k = 0$ can use location of first peak to get $H_0$ . This one is unclear.

5. $\Omega_r$
   Actually doesnt show up here, but if we know $H_0$ then we can calculate this directly from the CMB temperature since we know how radiation energy density scales with $T$.


## 130
**Write down the Jeans equation for a disturbance propagating in a self-gravitating medium. From this show how to find the critical wavenumber for propagating modes. What is the Jeans mass?**
We essentially want to find the Jeans length. 

1. Intuitive answer:
   See [[Jeans#Jeans length|Jeans length]]
   
2. From Jeans equation: 
   Skipping the derivation, if you want details see Megan's notes, start with the collisionless Boltzmann equation and take the first moment (multiply it by $\mathbf{v}$ and integrate over velocity space) to end up with $$\frac{D\mathbf{v}}{Dt} = -\nabla \Phi - \frac{1}{\rho}\nabla P$$where $D/Dt = \partial/\partial t + (\mathbf{v}\cdot\nabla)$ is the convective dervative. Here $\Phi$ is the gravitational potential and $P$ is the pressure. We then use the following:
   - steady state ($\partial / \partial t = 0$)
   - spherically symmetric
   - radial equilibrium ($\langle v_r\rangle = 0$)
   - perturbations, so every quantity is background + small perturbation (eg $\rho = \rho_0 + \rho'$)
   -  mass continuity 
   - "Jeans swindle" (assume $\nabla^2\Phi_0 = 0 \neq 4\pi G \rho_0$ but $\nabla^2\Phi' = 4\pi G \rho'$ where the 0 refers to the background and prime to the perturbation), 
   
   one finds a wave equation for a density perturbation $\rho'$ on a background $\rho_0$ of $$\frac{\partial^2 \rho'}{\partial t^2} - 4\pi G\rho_0 \rho' = c_s^2\nabla^2\rho'$$where $c_s = \sqrt{\partial P / \partial \rho}$. Making a plane wave ansatz $$\rho'(\mathbf{k},t) \propto e^{i(\mathbf{k}\cdot\mathbf{x} - \omega t)}$$ one finds a dispersion relation $$\omega^2 = c_s^2k^2 - 4\pi G \rho_0$$Which can be recast in terms of the wavelength $\lambda = 2\pi / k$ as $$\omega = 2\pi\sqrt{\frac{c_s^2}{\lambda^2} - \frac{G\rho_0}{\pi}}$$One can see that for $$\lambda > \lambda_J := \sqrt{\frac{\pi c_s^2}{G\rho}} \implies \omega \text{ complex} \implies \text{perturbation grows in time}$$and conversely if $\lambda < \lambda_J$ the perturbation will oscillate and not collapse. Then [[Jeans#Jeans mass|Jeans mass]] is simple to calculate.


## 131
**Qualitatively, how does a density fluctuation grow over cosmic history and how does the answer differ for dark matter and baryons?**

There are two considerations to be made here, the Jeans length in each epoch, and the size scale of the "sound horizon" at different times. The sound horizon is the length scale that sound can travel at a particular time, and thus the length scale over which overdensities can be washed out at any given time. 

<mark class="hltr-pink">When the spatial size of a perturbation is larger than the sound horizon, it will grow as the universe grows (since it cant be stabilized/washed out yet), and if it is smaller than the Jeans length, it will also not collapse</mark>. However, once the sound horizon grows big enough, it will be able to stabilize the perturbation. The below is closely related to [[CMB#Sound horizon size|this note]] on sound horizon size at recombination.

- First consider the [[Jeans#Jeans length|Jeans length]] $$\lambda_J = \sqrt{\frac{\pi c_s^2}{G\rho}}$$which is set by the sound speed. Before [[Recombination]], the fluid is dominated by [[Stars/Equations of state#Radiation pressure|Radiation pressure]] and so the sound speed is $$P_{rad} = \frac{1}{3}\rho c^2 \implies c_s = \sqrt{\frac{\partial P}{\partial \rho}} = \frac{c}{\sqrt{3}}$$After recombination, the baryons are efectively an ideal gas and so the sound speed is $$P = \frac{\rho}{\mu m_p}kT \implies c_s = \sqrt{\frac{\partial P}{\partial \rho}} = \sqrt{\frac{kT}{\mu m_p}} \ll c$$where we use $T  = T_0(1+z) \simeq 2.7\,\pu{K} (1100)\simeq 3000\,\pu{K}$ and $\mu$ is the [[Mean molecular weight#Mean molecular weight|mean molecular weight]]. This means $c_s$ drops dramatically at recombination, and the Jeans mass actually drops from $$M_J \sim10^{16}\,M_\odot \longrightarrow M_J \sim 10^{5}\, M_\odot$$which implies most of the structure we see today formed after recombination. As a result, lets only consider overdensity growth due to expansion and ignore the Jeans criteria for now.

- Next consider how the sound horizon evolves in different epochs (which term dominates the evolution of the scale factor $a$ of the [[FLRW#Friedmann equation|Friedmann equations]]). See [[#137|this question]] for the form of $a(t)$ in each era, or just [[Mnemonics]].
  1. Radiation-dominated era, $a(t) \propto t^{1/2}$
     The proper length of the sound horizon is $$\chi_s \simeq \int_0 ^{t}\frac{dt'}{a(t')} \, c_s \propto 2 c_s\, t^{1/2}$$ and so the proper length is $L_s = a\, \chi_s \propto 2c_s\, t$ which if we used the full expression for $a$, i suppose we would find is smaller than the Jeans length (thus no collapsing).
   2. Matter-dominated era, $a(t) \propto t^{2/3}$
      Here as above we get  $L_s = a\, \chi_s \propto 3c_s\, t$ 

The scaling of densities (and thus overdensities) in time in each of these epochs is given in [[#132|this question]], where one finds that for radiation dominated epochs $\delta \propto a^2$ and for matter-dominated $\delta \propto a$.

Choose a particular length scale for a perturbation $L$. Until the sound horizon is equal to $L$ (ie perturbations on this scale "enter the horizon") all perturbations on the scale $L$ grow as in [[#132|this question]] in time, but a sound wave has not had enough time to stabilize and wash out this perturbation yet. Once this length scale has "entered the horizon" then the sound waves can !UNFINISHED. Then upon collapsing the photon pressure pushes the baryons back out, reducing their overdensity but not that of dark matter, as DM and photons are not meaningfully coupled (but the DM is with the baryons, so in fact there will be some small impact on the dark matter). The picture is as below (Megans notes), where the oscillating portion is illustrated with animations in [[CMB#CMB power spectrum|CMB power spectrum]]. The exact position of "entering the sound horizon" can only be calculated by assuming a particular overdensity spatial scale $L$, with smaller sizes "entering the horizon" earlier and thus spending more time oscillating.
   ![[overdensity_growth.png]]


## 132
**What is the "spherical top hat" model for the formation of galaxies and clusters? What is the significance of the number $18\pi^2$?**

Assume an overdensity is a step function in radius (constant density sphere of a given radius) which looks like 

![[tophat.png]]

The overdensity it defined as $$\delta(\mathbf{x}) = \frac{\rho(\mathbf{x}) - \bar\rho}{\bar\rho}$$where the average density is calculated from the [[FLRW#Friedmann equation|Friedmann equation]] for the (assumed flat) background $$\bar\rho = \frac{3H^2}{8\pi G}$$<mark class="hltr-pink">How does this overdensity grow with time?</mark> We use Birkhoff's theorem to treat the spherically symmetric perturbation as a little closed ($k=+1$) universe, such that its density is given by $$\rho = \frac{3}{8\pi G}\left( H^2 + \frac{c^2}{a^2}\right)$$In this case the overdensity is $$\delta = \frac{1}{a^2}\frac{3}{8\pi G \bar\rho}$$Since in a radiation dominated universe the energy density (and thus $\bar\rho$) goes as $a^{-4}$ (3 factors for volume, one for redshift) and in a matter dominated universe the mass density goes as $a^{-3}$ we have (using the results of [[#137|this question]])
- Radiation-dominated $\implies \delta \propto a^2 \propto t$
- Matter-dominated $\implies \delta \propto a \propto t^{2/3}$

The growth of this overdensity continues until it decouples from the Hubble flow, after which it collapses. 
![[turn_overdensity.png|350]]

To find the time when it turns around from "getting bigger" with the Hubble flow to "getting smaller" as it collapses, use energy conservation while its expanding/contracting, and when it has its maximum radius at turnaround which we label $r_{max}$ (where $\dot{r} = 0$) $$E = \frac{1}{2}\dot{r}^2 - \frac{GM}{r} = -\frac{GM}{r_{max}}$$This is a differential equation for $r(t)$, and after making some not obvious substitutions and inverting to get $t(r)$ one finds $$t_{max} = \frac{\pi}{2}\left(\frac{3}{8\pi G\rho(t_{max})}\right)^{1/2}$$Lets compare this to the background at that time. The [[FLRW#Friedmann equation|Friedmann equation]] for a matter-dominated universe tells us $$H^2 = \left(\frac{\dot{a}}{a}\right)^2 = \left(\frac{2}{3t}\right)^2 = \frac{8\pi G \bar\rho}{3} \implies \bar\rho = \frac{1}{6\pi Gt^2}$$Therefore evaluating the background density at that time we find $$\bar\rho(t_{max}) = \frac{2}{3\pi^3 G}\left(\frac{8\pi G\rho(t_{max})}{3}\right) \implies \frac{\rho(t_{max})}{\bar\rho(t_{max})} = \frac{9\pi^2}{16}$$Since we mostly care about the end state of such an overdensity (that is, after it collapses and becomes a galaxy or similar) we may look at this object once it has virialized. We will use this to examine how dense the virialized object is relative to a part of the universe that is unperturbed, without needing to think about the details of nonlinear growth.

Via the virial theorem we know $E = (1/2) U_{vir}$ so using the above expression for energy at maximum radius we get $r_{max} = 2 r_{vir}$ which implies $\rho_{vir} = 8\rho(t_{max})$. Thus via the above we have  $$\frac{\rho_{vir}}{\bar\rho(t_{max})} = \frac{9\pi^2}{2}$$but really we dont want to compare to $\bar\rho(t_{max})$, rather we want to compare to $\bar\rho(t_{vir})$ and we can assume that the time to maximum is about the same as the time to virialization $t_{vir} = 2 t_{max}$ such that by the above work where we showed $\bar\rho \propto t^{{-2}}$ we know $\bar\rho(t_{max}) = 4\bar\rho(t_{vir})$ leading to $$\frac{\rho_{vir}}{\bar\rho(t_{vir})} = 18\pi^2$$So this number described the density of a virialized galaxy relative to that of the background $\simeq 180$ which lead to people discussing the $R_{200}$ for example, the radius within which the mean density was 200 times the average density of the universe at that time. It is now known however that this is a biased metric and something like the splashback radius is more appropriate.


## 133
**Summarize the observational evidence in favor of the standard "Big Bang" model of the universe.**
1. The universe is expanding
   We see everything moving away from us in a way that implies space is expanding. This is [[#134|Hubble's law]] and it could be caused by us being the center of some explosion of galaxies the likes of which we have no other observational evidence for, or that the universe is expanding uniformly (the same everywhere in space). This means the universe used to be much smaller, denser and hotter.
2. [[CMB]]
   - Originates in early universe and [[Spectra#Redshift|redshifted]] by expansion of universe
   - The universe used to be a [[Blackbody radiation#Blackbody radiation|blackbody]] until it cooled and expanded so photons could free stream. Implies hot and dense early universe
3. Big bang nucleosynthesis + abundance
   - In early universe ($\sim 2\,\pu{min}$ after big bang) nuclear fusion could occur, fusing hydrogen into helium and some others like lithium (see [[#146|this question]]).
   - The expected abundances from modelling the big bang match the observed abundances (although maybe they dont? Is cosmic lithium problem resolved?)
4. [[Galaxies#Galaxy|Galaxy]] evolution
   - High redshift galaxies look different as a population than local galaxies $\implies$ evolution over cosmic time(?)
   - The distribution of [[Galaxy clusters]] match expectations for structure formation after big bang


## 134
**What is the Hubble constant?** 
See [[Hubble constant]]

**Explain in detail at least three independent methods to measure it.**
1. Distance ladder     |     $H_0 \simeq 73\pm 1\,\pu{km s^{-1} Mpc^{-1}}$ 
   The most challenging part is distances. Here are the different methods which have been used to measure distances on different scales, together forming a "ladder". An example would be: 
   - we measure close objects of type A with parallax
   - calibrate a relationship to estimate distances to A based on observational characteristics
   - Observe A near rarer object B, and infer distances to B based on calibration of A
   - Calibrate B and repeat, getting distances to very distant objects

   The current state of our cosmological distance ladder depends on pulsating objects like [[Pulsating stars#Cepheids|cepheids]], [[Pulsating stars#RR-lyrae stars|RR-lyrae stars]] and "standard candles" of presumably known luminosity like Type 1a [[Supernovae#Supernova|supernovae]]  and the helium flash at the tip of the [[HR-diagram#RGB|red giant branch]] (independent measurement using this metric finds $H_0 \simeq 70\pm ?\,\pu{km s^{-1} Mpc^{-1}}$). We also have distant rungs like the [[Velocity dispersion#Tully-Fisher relation|Tully-Fisher relation]]. The below diagram is explained in more detail [here](https://en.wikipedia.org/wiki/Cosmic_distance_ladder)
   ![[distance_ladder.png|500]]

2. [[Lensing#Strong lensing|Strongly-lensed]] [[AGN#Quasar|quasars]]     |     $H_0 \simeq 73\pm 2\,\pu{km s^{-1} Mpc^{-1}}$ 
   The H0LiCOW team measures time delays between multiple images of a strongly lensed background quasar by a large foreground object, and the time delay (can be $\sim$ seconds) can be used to infer a distance independent of [[CMB]] and distance ladder constraints

3. Standard sirens     |     $H_0 \simeq 70\pm 2\,\pu{km s^{-1} Mpc^{-1}}$ 
   Method co-invented by Scott Hughes here at MKI. [[Gravitational waves|Gravitational wave]] observation can tell us the [[Gravitational waves#Chirp mass|chirp mass]] of a binary source, and from this we can calculate the power emitted in the merger. Via the inverse square law and the magnitude of our observation we then obtain a distance measurement (known loudness of siren + measurement $\implies$ distance). With EM followup to get a recessional velocity, we get an estimate of $H_0$.

4. [[CMB]] measurements     |     $H_0 \simeq 67\pm 1\,\pu{km s^{-1} Mpc^{-1}}$ 
   For example fitting the [[CMB#CMB power spectrum|power spectrum]] with the $\Lambda\rm{CDM}$ model, and predicting $H_0$ within the context of this model. Can combine with [[BAO]] to improve constraints.

**How does it relate to the age of the universe?**
The Hubble time is the age of the universe if it has always expanded at the same rate, and that rate is the one we measure today. If the universe was always expanding (starting from size 0) with rate described by $H_0$ then its size $L$ is as measured at the time $t_H$ (today) would be $$L = v \, t_H = H_0 \, d\, t_H \implies t_H = \frac{1}{H_0} \simeq 14\,\pu{Gyr}$$where $v$ is the constant rate of expansion.


## 135
**How can the age of the universe be estimated empirically? Do the current estimates agree with that obtained from the Hubble constant?**

1. Can estimate from the turn-off point of the [[HR-diagram#Main sequence|MS]] in [[Clustering#Globular Cluster|GCs]] as in [[Stars - Questions#17|this question]]. Theyre very old so provide a good lower bound on age of universe. Current estimates are roughly consistent with [[#134|Hubble time]] as we find GCs with ages of $\sim 12-13\,\pu{Gyr}$. The figure below is just for open clusters but the same principle applies to globular. 
   ![[zams.gif|400]]
2. [[Stellar classes#White dwarf|WD]] cooling from $T\sim 10^4\,\pu{K}$ with the [[Units#Luminosity|luminosity]] scaling with the core temperature as $L \propto T_c^{7/2}$. As a result, we can use the coolest white dwarfs to get a lower limit on age of the universe if we understand the processes by which they cool. Also $\sim 12-13\,\pu{Gyr}$
3. The [[Milky Way#Milky Way|MW]] stellar halo. This is thought to contain old stellar populations, but because these stars come from multiple populations (mergers) this can be difficult to do


## 136
**How would you compute the age of our universe using the Friedmann equation? What approximations can be made to simplify this calculation?**

Can estimate the age of the universe roughly via the [[FLRW#Friedmann equation|Friedmann equation]] if we assume the universe is matter dominated. In a matter-dominated universe (see [[#137|this question]]) the scale factor is  $$a(t) \propto t^{2/3} \implies H(t) = \frac{\dot a}{a} = \frac{\frac{2}{3}t^{-1/3}}{t^{2/3}} = \frac{2}{3t}$$Evaluating the expression $t = \frac{2}{3H}$ today (ie using the presnt-day Hubble constant $H = H_0$) one gets an estimate for the age of the universe as $$t_0 = \frac{2}{3H_0} = \frac{2}{3} t_H \simeq 9\,\pu{Gyr}$$ where $t_H$ is the Hubble time as in [[#134|this question]]. Note that this is smaller than other estimates, the reason being that we assumed matter-dominated, which is the second-fastest driving force in expansion, with radiation as the fastest, and dark energy the slowest. As a result, we end up underestimating the age a bit.


## 137
**What is the Robertson-Walker metric? What are the Friedmann equations?**

See [[FLRW]] for the answer to both.

**How does the universe expand if it is 
(i) radiation dominated?** 
   Radiation-dominated $\implies$ Friedmann equation reduces to $$\left(\frac{H}{H_0}\right)^2 = \Omega_r (1+z)^4 = \frac{\Omega_r}{a^4}$$Evaluating this at $z=0$ reveals that in the assumed radiation-dominated universe, $\Omega_r = 1$ (as expected). Then $$\frac{\dot a}{a} = H = \frac{H_0}{a^2}\implies \dot a  = \frac{H_0}{a} \implies a(t) = \sqrt{2H_0 t}\propto t^{1/2}$$
**(ii) matter dominated with $\mathbf{\Omega \ll 1,\, \Omega = 1,\, \Omega \gg 1}$?**
   Matter-dominated if we assume $\Omega_M = 1$ $\implies$ as above $$\dot a  = \frac{H_0}{\sqrt{a}} \implies a(t) = \left(\frac{3}{2}H_0 t\right)^{2/3}\propto t^{2/3}$$However, if we assume $\Omega \neq 1$ and allow $|\Omega_k| \neq 0 < |\Omega_M|$ (since still matter dominated)  then this is altered. Intuitively (and roughly), if the universe is 
   - open (negative curvature, $k = -1$) it should expand, 
   - but if its closed (positive curvature, $k = +1$) it should contract 

   See Megans notes for calculation.

**(iii) dominated by a cosmological constant?**
   Dark energy dominated $\implies$ as above $H^2 = H_0^2 \Omega_\Lambda = H_0^2$ and thus $$\frac{\dot a}{a} = H_0 \implies a = e^{H_0 t}$$which expands exponentially. The universe reached matter-dark energy equality at $z = 0.3$ (recent!).


## 138
**What was the approximate temperature of the universe at recombination, and why did recombination happen then?**

Short answer: 
- $T = T_0(1+z)$ (see [[Blackbody radiation#Blackbody radiation|BB]]) 
- $z_{rec} = 1100$ at [[Recombination]]
- so it was about $2.7\,\pu{K}(1100) \simeq 3000\,\pu{K}$ 

Why is that the redshift? Need to establish the redshift at which half of the hydrogen is ionized. This calculation is dnoe in [[Recombination]]. 

Note that the ionization energy of hydrogen is about $13.6\,\pu{eV}$ which would correspond to a thermal temperature on the order of $T \simeq E/k_B \simeq 10^5\,\pu{K}$  (using $k_B \simeq 10^{-4}\,\pu{eV K^{-1}}$) which implies we should have recombined much earlier than the redshift at which $T$ was $3000\,\pu{K}$. The reason it takes longer to reach half ionization is that the photon energy distribution has a long tail which keeps things ionized for longer (think of it as a [[Blackbody radiation#Blackbody radiation|BB]] with peak temperature much smaller than that required to ionize, but the tail is long so it can still do so).
![[photon_tail.png]]


## 139
**When (or at what redshift) did the universe become 
(i) matter dominated?** 
Matter-radiation equality of the [[FLRW#Friedmann equation|Friedmann equation]] happens when (using rough [[Observatories#Planck|Planck]] numbers)$$\Omega_{r}(1+z)^4 = \Omega_M(1+z)^3\implies z = \frac{\Omega_M}{\Omega_r} -1 \simeq \frac{0.3}{10^{-4}} - 1 = 3000$$**(ii) optically thin to electron scattering?** 
[[Recombination]], after which [[Scattering#Electron scattering|electron scattering]] occurs far less frequently.

**What temperature was the CMB at these times?** 
$T = T_0 (1+z)$ where $T_0 = 2.7\,\pu{K}$

**What significance did these events have for the CMB?**

For matter-radiation equality:
- Before this, no structure forms because the expansion is too fast. After, [[Dark matter]] starts to collapse and set potential wells in which the baryons oscillate with gravity against photon pressure (once enough time as passed for sound waves to travel in them, ie they "entered the sound horizon" as in [[#131|this question]]).
- Once potential wells are set, the [[CMB#CMB power spectrum|CMB power spectrum]] is impacted because as photons climb out of those wells, they get redshifted (the non-integrated Sachs-Wolfe effect). Since one large scales the DM potential wells are not varying, this means no power in the power spectrum on large scalles (small $l$ plateau).
- $\Omega_M$ sets the heights of the peaks on the power spectrum (see [[#129|this question]]) and also the redshift of M-R equality, so $z_{mr}$ related to heights of peaks.

For [[Recombination]]:
- Sets the scales that show up as peaks on the [[CMB#CMB power spectrum|power spectrum]].
- [[BAO]] which is just the same thing as the first peak.


## 140
**What evidence is there for dark energy and what might it be?**

What is it? 
- Cosmological constant/dark energy which acts like a negative pressure (think of a positive pressure as pushing in isotropically on a small body, such that a negative pressure pulls on it isotropically). 
- Maybe not a constant, rather a scalar field which changes in time ("quintessence")
- Maybe some exotic modified gravity

Particle physics predicts $\Omega_\Lambda\sim10^{120}$ via the planck time which is 120 orders of magnitude different than modelling of [[CMB]].

Evidence:
1. [[CMB#CMB power spectrum|CMB power spectrum]] fitting
   (and other things related to CMB) gives $\Omega_\Lambda \simeq 0.7 \neq 0$.

2. Integrated Sachs-Wolfe effect
   We see large scale redshifting consistent with an accelerated expansion that only occurs if universe is $\Lambda$ or radiation dominated

3. [[Supernovae#Supernova|Supernova]] cosmology
   Can measure [[Distances#Luminosity distance|luminosity distance]] of SNe and plot against redshift, (from Megans notes) ![[sne_cosmology.png]]
   Since the luminosity distance depends on cosmological params, can constrain $\Omega_\Lambda$ with these measurements. Difference becomes pronounced at higher redshifts, because expansion rate varies over cosmic time. Real data looks like the below (from Riess et al 1998) and w
   
   ![[perlmutter_snecosmology.jpg|500]]
   
   If the universe is flat (otherwise degeneracy between $\Omega_M$ and $\Omega_\Lambda$) we can use these measurements to make plots like ![[sne_constraints.png]]


## 141
**Is most of the hydrogen in the universe neutral or ionized? Describe the approximate ionization history of the Universe, and at what redshift the major phase transitions occurred.**

[[Reionization]] happened so its almost all ionized. 


## 142
**What is the Ly alpha forest? Why are cosmologists interested in it?**

See [[Spectra#Lyman-alpha forest|Lyman alpha forest]]. 

Cosmologists are interested in it because it provides a map of the matter along the line of sight.


## 143
**What are the "flatness problem" and the "isotropy problem" in standard Big-Bang cosmology? How does the inflationary model resolve these problems?**

**Flatness problem**
The fact that the total $\Omega = \rho/\rho_c$ of the [[FLRW#Friedmann equation|Friedmann equations]] is remarkably close to 1 today ($\Omega \simeq 1.00\pm 0.01$) that is, it is very *flat*. 

Why is this a problem? If you look at the Friedmann equations, a deviation from flatness will be blown up as the universe expands. A flatness of $\Omega \simeq 1.00\pm 0.01$ today would require
- $\Omega \simeq 1.00\pm 0.00004$ at [[Recombination]]
- $\Omega \simeq 1.00\pm 10^{-12}$ at nucleosynthesis

This implies an incredibly fine tuning of the universe at early times to be incredibly flat.

Derivation: 
Start with the Friedmann equation and ignore $\Lambda$ (since in early universe it was negligible) (or define $\rho_c$ with $\Lambda$ in it as in [[FLRW#Friedmann equation|this note]]). It can be rearranged to $$\left(\frac{3H^2}{8\pi G} - \rho(z)\right)a^2 = -\frac{3kc^2}{8\pi G} = \text{const}$$Then using that $\Omega(z) = \rho(z) / \rho_{c}(z)$ and the definition of the critical density this can be written (using also $\rho(z)\propto a^{-3}$) we have $$\begin{align}
\rho(z)\left(\frac{\rho_c(z)}{\rho(z)} - 1\right)a^2 &= \text{const}\\
\frac{1}{\Omega(z)} - 1 &\propto a(z)
\end{align}$$meaning that if today ($a=1$) we observe an $\Omega\simeq 1$ then since $a$ has changed by a factor of $10^{60}$ since the Planck era, so too must have $\Omega^{-1} - 1$ (implying it was extremely close to 1).

Inflation solves this by rapidly expanding the universe by a large factor such that locally, the universe looks very flat. 
![[flatness_problem.jpeg|400]]

**Isotropy problem**
The light horizon size at [[Recombination]] is only $\sim 2^\circ$ on the sky today (see [[CMB#Sound horizon size|sound horizon size]] and note that we assumed sound speed was $c/\sqrt{3}$ so we can just multiply that answer of about $1^\circ$ by $\sqrt{3}$) but its almost a perfect [[Blackbody radiation#Blackbody radiation|blackbody]] meaning it was in thermal equilibrium, suggesting this scale should be the size of the entire sky. When was it in causal contact in order to reach equilibrium?

Inflation solves this by whole universe being in causal contact close to big bang
![[isotropy_problem.png]]


## 144
**What is the baryonic contribution to the cosmological mass density and how is it determined?**

We have measured $\Omega_b \simeq 0.05$ and $\Omega_M \simeq 0.3$, so about 18% of the mass budget. We measure this via 
1. The baryon loading effect of the [[CMB#CMB power spectrum|CMB power spectrum]] (see [[Cosmology - Questions#129|Q129]]) via the difference between the first and second peaks. 
2. [[BBN#BBN|Big bang nucleosynthesis]] and the abundance of primordial elements, finds consistent baryon fraction with CMB. Point of confusion: Why do we measure things close to the big bang if we want to constrain the baryon fraction $\Omega_b$ now (redshift 0)?
   ![[BBN.png|300]]

**Where are the bulk of the baryons in our Universe?**
- If we add up all the baryons we see in [[Stars - Questions|stars]], [[Galaxies]], the [[Interstellar medium|ISM]], [[Cluster media#ICM|ICM]] etc, we only get $\sim 50\%$ of the baryons we'd expect from measurements of the [[CMB]] and [[BBN]]. This is the "missing baryon problem"
- Solution is that half the baryons are in a warm-hot ($10^5-10^7\,\pu{K}$) intrgalactic medium ("WHIM") along cosmic filaments. Have recently observed this medium along the line of sight to distant quasars via the SZ-effect.

![[missing_baryon_problem.png|400]]


## 145
**How did the particle content of the universe evolve? What is the most abundant particle in the universe today?**
Stealing very nice table of early universe particle history + timeline afterwards from Megan's notes 

![[particle_content_history.png]]

The most abundant particles in the universe now are not baryons, but photons and neutrinos (can understand in terms of their "mass/energy per particle" and their relative abundances $\Omega_i$ currently). It may also be the case that dark matter is highly abundant in number density, via $$n_{DM,0} = \frac{\Omega_{DM}\rho_{crit,0}}{m_{DM}}$$provided that it is very light.


## 146
**Describe, qualitatively, the synthesis of light elements in the Big Bang. What is the deuterium bottleneck, and how does it help produce the right helium abundance?**

See [[BBN]]. 

**What role does radiation play in Big Bang nucleosynthesis?**
The role of radiation is that universe is radiation-dominated, setting the timescale over which temperature changes, and this sets when deuterium can form.


## 147
**What are the thermal and kinetic Sunyaev-Zel'dovich effects? What are they useful for?**

See [[CMB#SZ effect|SZ effect]].


## 148
**What range of physical scales are being probed by current and future CMB experiments?** 
- [[Observatories#COBE|COBE]]: $\sim 7^\circ$ 
- [[Observatories#WMAP|WMAP]]: $\sim 0.5^\circ$ 
- [[Observatories#Planck|Planck]]: $\sim 7'$  ([[Units#Arcminute|arcmin]])
- [[Observatories#SPT|SPT]]: $\lesssim 5'$ 
- [[Observatories#ACT|ACT]]: $\sim 1'$ 
- [[Observatories#CMB-S4|CMB-S4]] will go from 10s of degrees to an arcmin, since CMB polarization B mode measurements require both low and high $l$ data (in order to delens, see [this](https://indico.fnal.gov/event/12206/contributions/12877/attachments/8517/10858/CMB-S4_PAC_160621v2.pdf))

**Are the anisotropies related to galaxy formation?** 
[[CMB#CMB|CMB]] anisotropies $\implies$ matter over- and under-densities which are believed to ultimately grow into the large scale structure of the universe like [[Galaxy clusters]] and [[Galaxy groups]]. However, silk damping (photon diffusion damping on small scales) wipes out structures smaller than the silk mass $\sim 10^{13}\,M_\odot$

**What is the current observational status?**
- Planck gives amazing anisotropy data and [[CMB#CMB power spectrum|power spectrum]] data down to very small ($l\simeq 2000$) scales, and we are reaching the statistical limit of what can be done with CMB
- There is need for higher resolution measurements of [[CMB#CMB Polarization|CMB polarization]]
- Future observations from [[Observatories#BICEP|BICEP3]], Simons observatory and [[Observatories#CMB-S4|CMB-S4]].


## 149
**What is the "Lyman limit", and how does it relate to observations of high-redshift galaxies?**

See [[Spectra#Lyman-alpha forest|Lyman alpha forest]]. When there are a significant number of neutral hydrogen atoms along the line of sight, any light more energetic than $\lambda = 912\,\pu{Å}$ will be absorbed (wavelength corresponding to ionization energy of ground state hydrogen $\chi_H = 13.6\,\pu{eV}$). 

The wavelength of the Lyman break informs the redshift of <mark class="hltr-pink">the source</mark> (since at that stage the spectrum was the "most energetic") after which follow-up spectroscopy can be performed.  Assuming a source hits the lyman limit along the line of sight, ie we see no flux at wavelengths smaller than $\lambda = 912\,\pu{Å} (1+z)$ which is a valid assumption for far away things. Should see source disappear in bluer filters if its at high redshift (Rohan Naidu here at MKI uses this).
![[lyman_limit.jpg]]


## 150
**What mass should a neutrino have to close the universe?**

"Close the universe" just means to make the universe flat $\Omega = 1$ in the context of the [[FLRW#Friedmann equation|Friedmann equations]]. If all mass is in neutrinos then this is the condition that $$\rho_\nu = \rho_{crit} = \frac{3H_0^2}{8\pi G}$$If we only needed neutrinos to account for all the [[Dark matter]], then we would instead have $$\rho_\nu = \Omega_{DM}\rho_{crit} = \frac{3\Omega_{DM}H_0^2}{8\pi G}$$with $\Omega_{DM}\simeq 0.3$ (see [[Observatories#Planck|Planck]]). Though if this was true there would be no large scale structure, as things would be moving too quickly to collapse.

To work out the mass, we need the number density of neutrinos in the universe. One can calculate the neutrino to photon temperature ratio via conservation of neutrino entropy (I guess its conserved because they dont interact with other things so their thermal properties dont change) and end up with $$\frac{T_\nu}{T_\gamma} = \left(\frac{4}{11}\right)^{1/3} \implies T_{\nu,0} \simeq 2\,\pu{K}$$for the cosmic neutrino background today, since that factor is about $0.7$ and the photon temperature (CMB blackbody) is $2.73\,\pu{K}$. Since $\rho \propto T^4$ this leads to $$\frac{\rho_\nu}{\rho_\gamma} \simeq N_{eff}\left(\frac{4}{11}\right)^{4/3}$$where $N_{eff} =  3$ comes from the greater number of degrees of freedom of neutrinos relative to photons since 3 neutrino flavors, and I've left out a factor of $7/8$. Then !UNFINISHED (how have we converted $\rho$ to $n$ ??)

There are about 300 neutrinos per $\pu{cm^{3}}$ and about 400 photons. Leads to neutrino masses of $m_\nu \simeq 18\,\pu{eV}$ and $5\,\pu{eV}$ respectively for the above two cases.

**Compare it with current upper bounds (or detections)**
Current upper bound is $m_\nu < 0.8\,\pu{eV}$ from [[Observatories#KATRIN|KATRIN]]. 

Experimental neutrino mass timeline below, but the x axis is $m^2$ so actually this may be confusing. Just use it for experimental history and relative sizes of error bars. Also cosmological contraints using [[BAO]] and other probes finding constraints $m_\nu \lesssim 0.1\,\pu{eV}$ but bounds depend on cosmological assumptions.

![[NeutrinoMassTimeline2022.png|500]]


## 151
**What is the meaning and purpose of a log N – log S curve? Explain the current interpretation of this curve for gamma-ray bursts.**

Used to measure deviation of a population of sources from being homogeneous and isotropic in the universe (eg uniform on sky and at all redshifts).

- $N$ is number of [[GRBs]]
- $S$ is total energy released = "fluence" = time-integrated [[Units#Flux|flux]]. Often measured in total number of counts observed. The flux $F$ for a source of [[Units#Luminosity|luminosity]] $L$ at distance $D$ is $$F = \frac{L}{4\pi D^2} \longrightarrow \text{time integrate} \longrightarrow S = \frac{E}{4\pi D^2}$$for total energy output $E$. 

For some minimum detectable fluence $S_{min}$ for our instrument, the maximum distance at which we can observe an object of energy $E$ is $$D_{max} = \sqrt{\frac{E}{4\pi S_{min}}}$$meaning we expect to be able to see sources in a volume of space (centered on us) is $V = \frac{4}{3} \pi D_{max}^3$ such that if the spatial density of sources is uniform, we should see $N\propto D_{max}^{3} \propto S_{min}^{-3/2}$ events, ie a line on a log-log plot of slope $-3/2$.

The [[GRBs#GRB|GRB]] curve looks like: 
![[logn_logs.gif]]
The fact we are seeing deviations at low energy (ie far away form us) implies we are seeing out to redshifts at which GRBs had not yet formed. Could be due to 
- Finite age of universe, not enough time for [[Supernovae]] and binary [[Neutron stars#Neutron stars|NS]] mergers etc
- Evolving GRB rate or intrinsic luminosity over cosmic time, perhaps scaling with star formation rate or metallicity


## 152
**In our Universe, at roughly what scale does perturbation theory break down and become non-perturbative?**

Linear perturbation growth breaks down when overdensities decouple form the Hubble flow (see [[#132|this question]]). Structure in the universe forms hierarchically because smaller scales go non-linear first. 

At what length scale does this transition occur for a given redshift? From [[#132|this question]] we have for the density of a perturbation $$\frac{\rho(t_{max})}{\bar\rho(t_{max})} = \left(\frac{r(t_{max})}{r}\right)^{3} = \frac{9\pi^2}{16}\simeq 5$$where $t_{max}$ is the time at which the overdensity decouples from the Hubble flow. Thus the transition occurs at approximately $$\rho \simeq 5\bar\rho = 5\bar\rho_0 (1+z)^3 = \frac{15\Omega_M H_0^2}{8\pi G}(1+z)^3$$We can convert this to a (mass-dependent) radius via $\rho = 3M/4\pi r^3$ and end up with a nonlinear scale of $$r_{\rm{nonlinear}} \lesssim \left(\frac{M}{10^{12}\,M_\odot}\right)^{1/3} \left(\frac{1}{1+z}\right) \,\pu{Mpc}$$which gives something like 10s of $\pu{Mpc}$.  