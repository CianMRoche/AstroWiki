## Comoving distance
Distance between objects factoring out expansion of universe, such that two otherwise unmoving objects will have constant comoving distance over cosmological time. 

The comoving coordinate system evolves "with" the Hubble flow and is related to the [[Units#Proper distance|proper distance]] $d_p = a(t)\,d_C$ measured by an observer at a particular time $t$ where $a$ is the scale factor of the [[FLRW#Friedmann equation|Friedmann equations]]. 

It is essentially the $r$ coordinate in the [[FLRW#FLRW metric|FLRW metric]] (in a flat universe) measured along a null geodesic between points in spacetime where $t_e$ and $t_0$ are the time coordinate values when the light is emitted and observed, respectively. It is given by the following $$d_C(z) = c\int_{t_e}^{t_0}\frac{dt}{a(t)} =  d_H \int_0^{z} \frac{dz}{E(z)}$$where we have defined the Hubble distance $d_H = c/H_0$ and $$E(z) = \frac{H(z)}{H_0} = \sqrt{\Omega_{r}(1+z)^4 + \Omega_M(1+z)^3 + \Omega_k(1+z)^2 + \Omega_\Lambda}$$
**Derivation**
We'll do the derivation for a flat universe, but it holds even for a non-flat universe. We are in this derivation accounting for the fact that For a radial light ray ($d\mathbf{\Omega} = 0$, $d\tau = 0$) in the [[FLRW#FLRW metric|FLRW metric]] in a flat universe, we have $$c\,dt = a(t)\,dr$$ and the comoving distance $r$ between light emitted at $t_e$ and observed today at $t_0$ is $$r = c\int_{t_e}^{t_0}\frac{dt}{a(t)}$$Using the relations  $$H = \frac{\dot{a}}{a} \implies dt= \frac{1}{H}\frac{da}{a}\quad ,\quad a(z) = \frac{1}{1+z} \implies \frac{da}{a} = -a\, dz$$we can rewrite this as $$d_C = r = c\int_{0}^{z}\frac{dz}{H(z)}= \frac{c}{H_0}\int_{0}^{z}\frac{dz\,H_0}{H(z)}$$

## Angular diameter distance
An object of proper length $x$ at redshift $z$ that appears to have angular size $\delta\theta$ has the angular diameter distance of $d_A ( z ) = x / \delta\theta$. This is commonly used to observe so called "standard rulers", for example in the context of [[BAO#BAO|baryon acoustic oscillations]].

In a flat universe, simply given in terms of the [[#Comoving distance]] by $$d_A(z) = \frac{d_C(z)}{1+z}$$

## Luminosity distance
If the intrinsic [[Units#Luminosity|luminosity]] $L$ of a distant object is known, we can calculate its "luminosity distance" by measuring the [[Units#Flux|flux]] $F$ and determine a distance $d_L(z)=\sqrt{L/4\pi F}$. 

In a flat universe, simply given in terms of the [[#Comoving distance]] by $$d_L(z) = (1+z)\,d_C(z)$$