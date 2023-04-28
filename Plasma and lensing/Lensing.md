Nice notes [here](https://arxiv.org/pdf/astro-ph/9606001.pdf) but all the figures are at the end. Also [here](https://lweb.cfa.harvard.edu/~dfabricant/huchra/ay202/lectures/lecture12.pdf) which might be better.

## Lensing
When we see light, we assume its source is in the direction the light came from. Light can be bent by optics like lenses, so if we can see the light is coming out of a lens, we can infer that the source may not be where it appears to be. When we look at a light source in space we dont see any (obvious) lenses, so we assume the source is along the line of sight of the "bright spot" on the sky. 

However, [[General relativity]] tells us that light doesnt travel in "straight lines" in the way we are used to, and that this effect grows with the amount mass (energy) present near the path of light. Large collections of mass like a [[Galaxy clusters#Galaxy cluster|galaxy cluster]] can thus act as massive astronomical lenses, making objects appear in positions they are not (if we had erroneously made the assumption that light is not bending). The geometric picture (from Megan's notes) is 

![[grav_lens_geometry.png]]

If the "true source angle" $\beta$ is zero, then we see a perfect ring of images of the source (by rotating the above picture about the observer-lens axis) called an <mark class="hltr-pink">Einstein ring</mark>. The angular size of the Einstein ring is the *Einstein angle* $$\theta_E = \sqrt{\frac{4GM}{c^2}\frac{D_{LS}}{D_{L}D_{S}}}$$the derivation of which we skip (it seems like almost everyone does, its a GR prediction plus trigonometry). Best thing to remember is the approximation $$\theta_E\,[\pu{mas}] \simeq \sqrt{\frac{M\,[M_\odot]}{10 D\,[\pu{kpc}]}}$$

## Strong lensing

Visible distorsion and formation of rings/arcs/multiple images by a large foreground gravitational lens of a background object. See [[#Lensing]] and [[Plasma and lensing - Questions#96|Q96]]. In the example below, a [[Galaxy clusters#Galaxy cluster|galaxy cluster]] in the foreground is lensing many background objects, but produces clear multiple images of a background [[AGN#Quasar|quasar]] and [[Galaxies#Galaxy|galaxy]].

![[strong_lensing.jpg]]

- Fun fact: the number of images produced is governed by the "odd number theorem"  of differential topology. It states "<mark class="hltr-pink">the number of multiple images produced by a bounded transparent lens must be odd</mark>".

- Fun fact 2: Was not believed to be observable back in the 1930s when [[Galaxies]] were believed to have masses of $10^9\,M_\odot$ until Zwicky demonstrated their mass was much larger via the virial theorem in the [[Galaxy cluster examples#Coma cluster|Coma cluster]], arguing this would produce images at a sufficient distance from the lens to be resolvable.

- Fun fact 3: Zwicky predicted: about 1 in 100 bright high-redshift sources would be lensed in a manner detectable in principle by a foreground [[Galaxies#Galaxy|galaxy]]. Turns out to be pretty much correct. More distant means more intervening galaxies, increasing chances of lensing (but has to be bright so a [[AGN#Quasar|quasar]] is an ideal candidate, also because it is compact and so multiple images can more easily be resolved).

We can also see rings and arcs like this:
![[A_Horseshoe_Einstein_Ring_from_Hubble.JPG]]

The lensing "power" of a system can be thought of in terms of a mass density projected along the line of sight (like a column density). In the limit that the lens is thin compared to the distances between the observer and lens, and lens and background object, define this projected mass density $\Sigma$ (units of $\pu{kg m^{-2}}$) as $$\Sigma(\vec{\xi}') = \int \rho(\vec{\xi}', z)\, dz$$where $\vec{\xi}'$ is a vector on the plane of the sky as in the image below and $\rho$ is the volumetric mass density. The deflection angle (again see the image below, but also [[#Lensing]]) is then $$\overrightarrow{\hat{\alpha}}(\vec{\xi})=\frac{4 G}{c^2} \int \frac{\left(\vec{\xi}-\vec{\xi}^{\prime}\right) \Sigma\left(\vec{\xi}^{\prime}\right)}{\left|\vec{\xi}-\vec{\xi}^{\prime}\right|^2} d^2 \xi^{\prime}$$If you're wondering why $\overrightarrow{\hat{\alpha}}$ is a vector, its because it depends on $\vec{\xi}$ not only through it's magnitude, but also through its direction. It is common to discuss discuss the surface density $\Sigma$ relative to some critical density $\Sigma_{crit}$ above which we "expect lensing" and below which we "dont expect lensing". <mark class="hltr-grey">It is the mean surface density enclosed within the Einstein radius</mark>. The relative mass density is called the <mark class="hltr-pink">convergence</mark> and is written $$\kappa(\vec{\theta}) = \frac{\Sigma(\vec{\theta})}{\Sigma _{crit}}\quad, \quad \Sigma_{crit} = \frac{c^2}{4\pi G} \frac{D_S}{D_{LS} D_L}$$
![[thin_strong_lens.png|400]]

And an object **passing behind a lens** looks like this, where (from Scott Gaudi) the lens is shown in yellow and its Einstein ring in green. The source is shown in red, its two images in blue, and its image paths in gray. 
![[lensing.gif]]
**What do we use strong lensing for?**
- To constrain the masses of objects acting as gravitational lenses (parametric fitting, one method is to assume there are $N$ halos and let their masses and positions be fit parameters).
- Act as cosmological magnifying glasses, allowing us to see much fainter objects if they happen to lie behind lenses, since more of their light is focused toward us. Most effective when the background objects lie on curves of very high magnification. 
- To map out the spatial distribution of underlying dark matter that we could otherwise not see (can be less powerful than [[#Weak lensing]] for large scale mapping).


## Weak lensing

A statistical effect on a distribution of background sources. The degree of lensing on any individual background object is not detectable, but the statistical impact of many minor lensing events (eg way too many galaxies looking elliptical and stretched) can be quantified over an image to constrain the distribution of smaller mass halos (lumps) in the foreground. They may also apear to be "lined up" along circles or arcs in a way that would be otherwise highly unlikely.

Below, "shape noise" refers to adding on a combination of real expected galaxy shapes and projection effects in a random way. Many galaxies will look highly elongated or elliptical even without lensing, but the distribution of shapes is very well-understood (both by understanding galaxies and doing some simple projection math with random orientations).
![[weak_lensing.png]]

**What do we use weak lensing for?**
- Huge result is that of mass mapping in the [[Galaxy cluster examples#Bullet Cluster|bullet cluster]]. [[Observatories#CHANDRA|CHANDRA]] provided strong evidence for an alternative massive and abundant species not coupled (in a detectable way currently) to electromagnetism, ie [[Dark matter]]. Also in particular allows one to constrain the self-interaction cross section.
- The surface mass density recovered from weak lensing measurements does exhibit a degeneracy called the "mass sheet degeneracy" which can be broken with any independent measurements of the magnification, since magnification does not exhibit the same degeneracy.
- Need a precise understanding of the point spread funciton of your instrument to do well.

Below is a lensing map of the bullet cluster.
![[Bullet_cluster_lensing.jpg]]


## Microlensing
Lensing due to a compact halo-like object, largely independent of its mass and not depending on the lens' luminosity. With microlensing, the lens mass is too low (mass of a planet or a star) for the displacement of light to be observed easily, but the apparent *brightening* of the source may still be detected. Note that the light curve ends up looking highly Lorentzian.

Note in the image below the bending would be of small enough mangitude that the apparent sources would be in approximately the same position as the "true" source and not resolvable as in the animation.
![[Gravitational_microlens.gif]]

[[Observatories#GAIA|GAIA]] sees microlensing events in the [[Milky Way]], but not nearly enough to explain all the "missing mass" we attribute to [[Dark matter]]
![[MicrolensingGAIA.gif]]

Can be used to observe an exoplanet around a star via two superimposed microlensing events, provided the planet sits near the Einstein angle of the primary lens.

![[Microlensingexoplanet.gif]]