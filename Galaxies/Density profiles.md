## Isothermal sphere
The density profile of an isothermal sphere is $$\rho(r) = \frac{\sigma^2}{2\pi G r^2}$$where $\sigma$ is the [[Velocity dispersion#Velocity dispersion|velocity dispersion]]. See [[Galaxies - Questions#104|Q104]] for the derived rotation curve.

**Derivation (incomplete)**
The potential $\Phi$ and mass density $\rho$ are related via Poisson's equation $\nabla^2\Phi = 4\pi G\rho$ which in spherical symmetry reduces to $$\frac{1}{r^2} \frac{d}{dr} \left[r^2\frac{d\Phi}{dr}\right] = \frac{1}{r} \frac{d^2}{dr^2} \left[r\Phi\right] = 4\pi G \rho$$I dont think we end up using this for anything? For an isothermal ($T = \text{const}$) sphere, we use two of the [[Stellar structure equations]] and we end up assuming kinetic energy = thermal and an ansatz for the density profile.

1. [[Stellar structure equations#Hydrostatic equilibrium|Hydrostatic equilibrium]] 
   Start with hydrostatic equilibrium $$\frac{dP}{dr} = -\frac{GM_r\rho}{r^2}$$Then assume ideal gas law holds $P = n k T = k T (\rho/m)$ where $m$ is the mean particle mass. This yields $$\frac{d\rho}{dr} = -\frac{GM_r m}{kT}\frac{\rho}{r^2}$$Now assume the velocity in the system is given by the [[Velocity dispersion#Velocity dispersion|velocity dispersion]] $\sigma$ such that equating the thermal energy and kinetic energies gives $m\sigma^2 = kT$. I dont understand because as soon as we make this assumption, we fix the Use this in the above and get$$\frac{d\rho}{dr} = -\frac{GM_r}{\sigma^2}\frac{\rho}{r^2}$$Which is the differential equation the density profile of a self-gravitating ideal gas with constant temperature in hydrostatic equilibrium must satisfy. This can be rewritten as $$r^2 \frac{d\ln\rho}{dr} = -\frac{GM_r}{\sigma^2}$$
2. [[Stellar structure equations#Mass continuity|Mass continuity]]
   Start with mass continuity $$\frac{dM_r}{dr} = 4\pi r^2 \rho$$Differentiating the equilibrium equation above wrt $r$ and using this mass continuity we have $$\frac{d}{dr} \left[r^2\frac{d\ln\rho}{dr}\right] = -\frac{G}{\sigma^2}\frac{dM_r}{dr} = -\frac{G}{\sigma^2}4\pi r^2\rho$$Making the ansatz $\rho = \rho_0 r^{-\alpha}$ (why? does this somehow follow from the [[Polytropes#Polytrope|polytrope]] equation? Maybe relying on uniqueness of solutions) I'm confused, but what one finds is $\alpha = 2$ by matching powers of $r$ and also $\rho_0 = \sigma^2 / 2\pi G$ such that we find the result above.


## NFW
See [[Galaxies - Questions#118|this question]] 