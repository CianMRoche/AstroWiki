Summary of distances [here](https://arxiv.org/abs/astro-ph/9905116)

## Comoving distance
Distance (derived along a lightlike path) between points in spacetime factoring out expansion of universe, such that two otherwise unmoving objects will have constant comoving distance over cosmological time. 

The comoving coordinate system evolves "with" the Hubble flow and is related to the [[#Proper distance|proper distance]] $d_p = a(t)\,d_C$ measured by an observer at a particular time $t$ where $a$ is the scale factor of the [[FLRW#Friedmann equation|Friedmann equations]]. 

It is essentially the $r$ coordinate in the [[FLRW#FLRW metric|FLRW metric]] (in a flat universe) measured along a null geodesic between points in spacetime where $t_e$ and $t_0$ are the time coordinate values when the light is emitted and observed, respectively. It is given by the following $$d_C(z) = c\int_{t_e}^{t_0}\frac{dt}{a(t)} =  d_H \int_0^{z} \frac{dz}{E(z)}$$where we have defined the Hubble distance $d_H = c/H_0$ and $$E(z) = \frac{H(z)}{H_0} = \sqrt{\Omega_{r}(1+z)^4 + \Omega_M(1+z)^3 + \Omega_k(1+z)^2 + \Omega_\Lambda}$$
**Derivation**
We'll do the derivation for a flat universe, but it holds (with more complicated expressions, see [this page](https://www.wikiwand.com/en/Comoving_and_proper_distances)) even for a non-flat universe. For a radial light ray ($d\mathbf{\Omega} = 0$, $d\tau = 0$) in the [[FLRW#FLRW metric|FLRW metric]] in a flat universe, we have $$c\,dt = a(t)\,dr$$ and the comoving distance $r$ between light emitted at $t_e$ and observed today at $t_0$ is $$r = c\int_{t_e}^{t_0}\frac{dt}{a(t)}$$Using the relations  $$H = \frac{\dot{a}}{a} \implies dt= \frac{1}{H}\frac{da}{a}\quad ,\quad a(z) = \frac{1}{1+z} \implies \frac{da}{a} = -a\, dz$$we can rewrite this as $$d_C = r = c\int_{0}^{z}\frac{dz}{H(z)}= \frac{c}{H_0}\int_{0}^{z}\frac{dz\,H_0}{H(z)}$$

## Proper distance
The *instantaneous* distance between points in an expanding universe, which changes with the Hubble flow. Given in terms of the [[#Comoving distance]] and scale factor $a$ of the [[FLRW#Friedmann equation|Friedmann equations]] via $$d_{p}(z) = a(z)\,d_C(z) = \frac{1}{1+z}d_C(z)$$This makes sense because we define $a$ such that today, comoving and proper distances are the same. If we go into the past then $a$ is smaller but the comoving distance is the same (as it is invariant under the Hubble flow), so proper distances get smaller as we go into the past. I think this is the same thing as the [[#Angular diameter distance]] in a flat universe.


## Angular diameter distance
An object of proper length $x$ at redshift $z$ that appears to have angular size $\delta\theta$ has the angular diameter distance of $d_A ( z ) = x / \delta\theta$. This is commonly used to observe so called "standard rulers", for example in the context of [[BAO#BAO|baryon acoustic oscillations]].

In a flat universe, simply given in terms of the [[#Comoving distance]] by $$d_A(z) = \frac{d_C(z)}{1+z}$$The apparent angular size of an object at a fixed comoving distance then exhibits a turnover at about redshift 1. This can be understood as at low redshifts, as things get further away they look smaller and smaller, but eventually we get to a redshift where the universe was small enough that the object encompassed a significant portion of the sky, and so it starts to look larger again.

![[angular_diameter_redshift.jpg|300]]


## Luminosity distance
If the intrinsic [[Units#Luminosity|luminosity]] $L$ of a distant object is known, we can calculate its "luminosity distance" by measuring the [[Units#Flux|flux]] $F$ (both bolometric, ie integrated over all frequencies) and determine a distance $d_L(z)=\sqrt{L/4\pi F}$. 

In a flat universe, given in terms of the [[#Comoving distance]] by $$d_L(z) = (1+z)\,d_C(z)$$**Why?**
The luminosity ($L_{obs} \sim h\nu_{obs}/\delta t_{obs}$) is affected in the following way by an expanding universe:
1. The energy of the photons is reduced with [[Spectra#Redshift|redshift]] as $$\frac{\nu_{emit}}{\nu_{obs}} = \frac{\lambda_{obs}}{\lambda_{emit}} = \frac{a_{obs}}{a_{emit}} = 1+z$$
2. The arrival time between photons emitted at $t_{emit}$ and $t_{emit}+\delta t_{emit}$ is adjusted as $$\frac{\delta t_{obs}}{\delta t_{emit}} = \frac{a_{obs}}{a_{emit}} = 1+z$$since the light has a slightly different distance to travel.

The net effect is then $$L_{obs} = \frac{h\nu_{obs}}{\delta t_{obs}} = L_{emit}\left(\frac{a_{emit}}{a_{obs}}\right)^2 = L_{emit}(1+z)^2$$such that the observed flux and the square root lead to the factor above.