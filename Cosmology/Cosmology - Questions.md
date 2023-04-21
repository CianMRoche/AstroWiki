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

There has been a number of ground-based and balloon experiments since, but the main results are summarized below. 

![[cmb_comparison.png]]

The best measured quantities today are:
1. The almost perfect CMB [[Blackbody radiation#Blackbody radiation|blackbody]] spectrum which has peak at $T=2.73\,\pu{K}$. The anisotropies are on the order of $\Delta T/T \sim 10^{-5}$ which corresponds to temperature differences of about $30\,\pu{\mu K}$ that result from matter under and over-densities in the early universe.
2. The [[CMB#CMB power spectrum|CMB power spectrum]] 

Whats left to measure: Primarily the B-mode polarization (the thing [[Observatories#BICEP|BICEP]] didnt see because of [[Dust#Dust|dust]]), which informs primordial [[Gravitational waves]] from the big bang.


## 128
**What are the anisotropies in the CMB? How do their amplitudes depend on angular scale?**

The anisotropy, or directional dependency, of the [[CMB#CMB|cosmic microwave background]] signal is divided into two types: **primary anisotropy**, due to effects that occur at the surface of last scattering (the spherical shell on the sky so photons are now received that were originally emitted at [[Recombination#Recombination|recombination]]) and before; and **secondary anisotropy**, due to effects such as interactions of the background radiation with intervening hot gas or gravitational potentials, which occur between the last scattering surface and the observer. These effects have an impact on the shape of the [[CMB#CMB power spectrum|CMB power spectrum]].

Explaining the <mark class="hltr-pink">primary anisotropies</mark>: 
1. Non-integrated Sachs-Wolfe effect ($l\lesssim 100$)
   - Photons in a grav. well get redshifted climbing out of it (like the opposite of  [[Galaxies - Questions#113|violent relaxation]])
   - Caused by gravitational [[Spectra#Redshift|redshift]] occurring at the surface of last scattering. 
   - The effect is not constant across the sky due to differences in the matter/energy density at the time of last scattering, such that deeper potential wells lead to more reddened photons, and thus apparently lower [[Blackbody radiation#Blackbody radiation|blackbody]] peak temperaure via [[Blackbody radiation#Wien's displacement law|Wien's law]] (can also think of the peak wavelegth being redshifted to longer values). 
   - From Tegmark (1995): potential well also leads to time dilation, and so photons from deeper wells are actually from earlier times and therefore hotter (bluer). On larger scales this effect is proportional to the time of last scattering gravitational potential.

2. Acoustic oscillations ($100\lesssim l\lesssim 1000$)
   See [[BAO#BAO|BAO]].

3. Silk damping ($l\gtrsim 1000$)
   "photon diffusion damping" which washes out scales smaller than $1^\circ$ ($\lesssim 0.1^\circ$, around the third acoustic peak)
   - [[Recombination#Recombination|Recombination]] $\implies$ photons can "suddenly" travel much farther
   - These photons carry energy from the hot regions and diffuse to the cold regions, also dragging baryons around, such that any anisotropy on a very small scale is quickly washed out. Effect is strongest for smallest scales (largest $l$)
   - The *silk scale* is distance scale over which photon diffusion is important at $z=1100$, so about $3\,\pu{Mpc}$ when using an angular scale measured now of $0.1^\circ$. The mass contained within the scale is the *Silk mass* which we estimate to be $\sim 10^{13}\,M_\odot$, i.e. about the mass of a [[Galaxies#Galaxy|galaxy]] today 😱. SMaller sclaes (and smaller masses) are washed out.
   - There also exists electron diffusion damping for the same reasons but it is far weaker since the electrons couldnt diffuse nearly as far.

Explaining the <mark class="hltr-pink">secondary anisotropies</mark>: 
1. Integrated Sachs-Wolfe effect
   Same thing as non-integrated but can blueshift if photon passes through a well thats shallowing or redshifted if passing through a well thats deepening.
2. [[Scattering#Thomson scattering|Thomson scattering]] (isotropic and scale-independent)
3. [[CMB#SZ effect|SZ effect]] 
4. [[Lensing]]
   Large scale structure can lens the CMB
5. Late-time integrated Sachs–Wolfe effect -  dark energy?
