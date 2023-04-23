The start of cosmology is super super dense. I recommend reviewing [[FLRW]] first, and keep in mind that the order of the questions is a bit backwards in places. You will find that the answer to question $n$ often depends on something like $n+2$ and $n+5$, and in such a case its personal preference whether you go in order or jump around as needed.


## 126
**Summarize the state of the experimental field of 21cm cosmology and what it hopes to accomplish.**

See [[Spectra#21cm line|21cm line]] for explanation of line physics. 

What is the use of this line in studying cosmology? 
- Can use this transition to map the fraction of Hydrogen which is neutral over cosmic time, which tells us about the [[Reionization#Epoch of reionization|epoch of reionization]]. ![[neutral_hydrogen.png|500]]
- As [[CMB#CMB|CMB]] photons pass through a neutral hydrogen region, what we observe (ask Haochen)

What experiments can do this?
- [[Observatories#CHIME|CHIME]]. Also can measure [[BAO#BAO|BAO]] signal with these measurements
- [[Observatories#HERA|HERA]]. Can allow us to study first stars and epoch of reionization. Will place limits on 21cm power spectrum and thus ou understanding of how ionized bubbled form and evolve. More robust against astrophysical foreground, but still need accurate foreground models in all cases to see any signal at all
- [[Observatories#MWA|MWA]] and [[Observatories#SKA|SKA]] similar.


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
- Essentially measured the low-$l$ (Megan's notes says high $l$? unclear) flat part of the [[CMB#CMB power spectrum|CMB power spectrum]]
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
   - The effect is not constant across the sky due to differences in the matter/energy density at the time of last scattering, such that deeper potential wells lead to more reddened photons, and thus apparently lower [[Blackbody radiation#Blackbody radiation|blackbody]] peak temperaure via [[Blackbody radiation#Wien's displacement law|Wien's law]] (can also think of the peak wavelegth being redshifted to longer values). 
   - From Tegmark (1995): potential well also leads to time dilation, and so photons from deeper wells are actually from earlier times and therefore hotter (bluer). On larger scales this effect is proportional to the time of last scattering gravitational potential.

2. Acoustic oscillations ($100\lesssim l\lesssim 1000$)
   See [[BAO#BAO|BAO]].

3. Silk damping ($l\gtrsim 1000$)
   "photon diffusion damping" which washes out scales smaller than $1^\circ$ ($\lesssim 0.1^\circ$, around the third acoustic peak)
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
   - "Jeans swindle" (assume $\nabla^2\Phi = 0 \neq 4\pi G \rho$), 
   
   one finds a wave equation for a density perturbation $\rho'$ on a background $\rho_0$ of $$\frac{\partial^2 \rho'}{\partial t^2} - 4\pi G\rho_0 \rho' = c_s^2\nabla^2\rho'$$where $c_s = \sqrt{\partial P / \partial \rho}$. Making a plane wave ansatz $$\rho'(\mathbf{k},t) \propto e^{i(\mathbf{k}\cdot\mathbf{x} - \omega t)}$$ one finds a dispersion relation $$\omega^2 = c_s^2k^2 - 4\pi G \rho_0$$Which can be recast in terms of the wavelength $\lambda = 2\pi / k$ as $$\omega = 2\pi\sqrt{\frac{c_s^2}{\lambda^2} - \frac{G\rho_0}{\pi}}$$One can see that for $$\lambda > \lambda_J := \sqrt{\frac{\pi c_s^2}{G\rho}} \implies \omega \text{ complex} \implies \text{perturbation grows in time}$$and conversely if $\lambda < \lambda_J$ the perturbation will oscillate and not collapse. Then [[Jeans#Jeans mass|Jeans mass]] is simple to calculate.


## 131
**Qualitatively, how does a density fluctuation grow over cosmic history and how does the answer differ for dark matter and baryons?**

There are two considerations to be made here, the Jeans length in each epoch, and the size scale of the "sound horizon" at different times. The sound horizon is the length scale that sound can travel at a particular time, and thus the length scale over which overdensities can be washed out at any given time. 

<mark class="hltr-pink">When the spatial size of a perturbation is larger than the sound horizon, it will grow as the universe grows (since it cant be stabilized/washed out yet), and if it is smaller than the Jeans length, it will also not collapse</mark>. However, once the sound horizon grows big enough, it will be able to stabilize the perturbation.

- First consider the [[Jeans#Jeans length|Jeans length]] $$\lambda_J = \sqrt{\frac{\pi c_s^2}{G\rho}}$$which is set by the sound speed. Before [[Recombination]], the fluid is dominated by [[Stars/Equations of state#Radiation pressure|Radiation pressure]] and so the sound speed is $$P_{rad} = \frac{1}{3}\rho c^2 \implies c_s = \sqrt{\frac{\partial P}{\partial \rho}} = \frac{c}{\sqrt{3}}$$After recombination, the baryons are efectively an ideal gas and so the sound speed is $$P = \frac{\rho}{\mu m_p}kT \implies c_s = \sqrt{\frac{\partial P}{\partial \rho}} = \sqrt{\frac{kT}{\mu m_p}} \ll c$$where we use $T  = T_0(1+z) \simeq 2.7\,\pu{K} (1100)\simeq 3000\,\pu{K}$ and $\mu$ is the [[Mean molecular weight#Mean molecular weight|mean molecular weight]]. This means $c_s$ drops dramatically at recombination, and the Jeans mass actually drops from $$M_J \sim10^{16}\,M_\odot \longrightarrow M_J \sim 10^{5}\, M_\odot$$which implies most of the structure we see today formed after recombination. As a result, lets only consider overdensity growth due to expansion and ignore the Jeans criteria for now.

- Next consider how the sound horizon evolves in different epochs (which term dominates the evolution of the scale factor $a$ of the [[FLRW#Friedmann equation|Friedmann equations]]). See [[#137|Q137]] for the form of $a(t)$ in each era.
  1. Radiation-dominated era, $a(t) \propto t^{1/2}$
     The proper length of the sound horizon is $$\chi_s \simeq \int_0 ^{t}\frac{dt'}{a(t')} \, c_s \propto 2 c_s\, t^{1/2}$$ and so the proper length is $L_s = a\, \chi_s \propto 2c_s\, t$ which is we used the full expression for $a$ i suppose we would find is smaller than the Jeans length. The connection between this and how $\delta$ scales is in [[#132|Q132]]
   2. Matter-dominated era, $a(t) \propto t^{2/3}$
      Here as above we get  $L_s = a\, \chi_s \propto 3c_s\, t$ 

   So until  (ie perturbations "enter the horizon") all perturbations grow as the scale factor grows, but do not collapse as their sizes are smaller than the Jeans length. Finally, (ignoring Jeans instability) the picture is as below (Megans notes), where the oscillating portion is illustrated in [[CMB#CMB power spectrum|CMB power spectrum]] and the dark matter doesnt oscillate because there isnt the equivalent photon coupling and thus the overdensities can keep growing. The exact position of "entering the sound horizon" can only be calculated by assuming a particular overdensity spatial size, with smaller sized "entering the horizon" earlier and thus spending more time oscillating.
   ![[overdensity_growth.png]]


## 132
**What is the "spherical top hat" model for the formation of galaxies and clusters? What is the significance of the number $18\pi^2$?**

Assume an overdensity is a step function in radius (constant density sphere of a given radius) which looks like 

![[tophat.png]]

The overdensity it defined as $$\delta(\mathbf{x}) = \frac{\rho(\mathbf{x}) - \bar\rho}{\bar\rho}$$where the average density is calculated from the [[FLRW#Friedmann equation|Friedmann equation]] for the (assumed flat) background $$\bar\rho = \frac{3H^2}{8\pi G}$$<mark class="hltr-pink">How does this overdensity grow with time?</mark> We use Birkhoff's theorem to treat the spherically symmetric perturbation as a little closed ($k=+1$) universe, such that its density is given by $$\rho = \frac{3}{8\pi G}\left( H^2 + \frac{c^2}{a^2}\right)$$In this case the overdensity is $$\delta = \frac{1}{a^2}\frac{3}{8\pi G \bar\rho}$$Since in a radiation dominated universe the energy density (and thus $\bar\rho$) goes as $a^{-4}$ (3 factors for volume, one for redshift) and in a matter dominated universe the mass density goes as $a^{-3}$ we have (using the results of [[#137|Q137]])
- Radiation-dominated $\implies \delta \propto a^2 \propto t$
- Matter-dominated $\implies \delta \propto a \propto t^{2/3}$

The growth of this overdensity continues until it decouples from the Hubble flow, after which it collapses. 
![[turn_overdensity.png|350]]

To find the time when it turns around from "getting bigger" with the Hubble flow to "getting smaller" as it collapses, use energy conservation while its expaning/contracting, and when it has its maximum radius at turnaround which we label $r_{max}$ (where $\dot{r} = 0$) $$E = \frac{1}{2}\dot{r}^2 - \frac{GM}{r} = -\frac{GM}{r_{max}}$$This is a differential equation for $r(t)$, and after making some substitutions and inverting to get $t(r)$ one finds $$t_{max} = \frac{\pi}{2}\left(\frac{3}{8\pi G\rho_{max}}\right)^{1/2}$$Lets compare this to the background at that time. The [[FLRW#Friedmann equation|Friedmann equation]] for a matter-dominated universe tells us $$H^2 = \left(\frac{\dot{a}}{a}\right)^2 = \left(\frac{2}{3t}\right)^2 = \frac{8\pi G \bar\rho}{3} \implies \bar\rho = \frac{1}{6\pi Gt^2}$$Therefore evaluating the background density at that time we find $$\bar\rho(t_{max}) = \frac{2}{3\pi^3 G}\left(\frac{8\pi G\rho_{max}}{3}\right) \implies \frac{\rho_{max}}{\bar\rho(t_{max})} = \frac{9\pi^2}{16}$$Since we mostly care about the end state of such an overdensity (that is, after it collapses and becomes a galaxy or similar) we may look at this object once it has virialized. We will use this to examine how dense the virialized object is relative to a part of the universe that is unperturbed. 

Via the virial theorem we know $E = (1/2) U_{vir}$ so using the above expression for energy at maximum radius we get $r_{max} = 2 r_{vir}$ which implies $\rho_{max} = 8\rho_{vir}$. Thus via the above we have  $$\frac{\rho_{vir}}{\bar\rho(t_{max})} = \frac{9\pi^2}{2}$$but really we dont want to compare to $\bar\rho(t_{max})$, rather we want to compare to $\bar\rho(t_{vir})$ and we can assume that the time to maximum is about the same as the time to virialization $t_{vir} = 2 t_{max}$ such that by the above work where we showed $\bar\rho \propto t^{{-2}}$ we know $\bar\rho(t_{vir}) = 4\bar\rho(t_{max})$ leading to $$\frac{\rho_{vir}}{\bar\rho(t_{vir})} = 18\pi^2$$