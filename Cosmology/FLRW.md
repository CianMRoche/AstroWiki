## FLRW metric
"Friedmann–Lemaître–Robertson–Walker". The general form of the metric follows from the assumptions of an expanding/contracting universe which is
- homogeneous
- isotropic

These assumptions lead to a form of the metric $$- c^2 d\tau^2 = -  c^2 dt^2 + a(t)^2d\mathbf{\Sigma}^2 $$where $d\mathbf{\Sigma}$ is the line element on a 3D space of uniform curvature $$d\mathbf{\Sigma}^2 = \frac{dr^2}{1 - kr^2} + r^2 d\mathbf{\Omega}^2,\quad\text{where }d\mathbf{\Omega}^2 = d\theta^2 + \sin^2{\theta} d\varphi^2$$where $k$ represents the type of curvature of the space $$k = \cases{
+1 \implies \text{positive curvature,~~~~~ (closed) 3-sphere} \\
~~~0 \implies \text{zero curvature~~~~~~~,~~~~~ flat Euclidean space} \\
-1 \implies \text{negative curvature,~~~~ (open) hyperbolic space} \\
}$$and in this parameterization $a$ has dimensions of length (and represents the radius of curvature) and $r$ is dimensionless. In these coordinates, $r,\theta,\varphi$ are all comoving coordinates which are invariant under the expansion of the universe, which is described by $a(t)$. 


## Friedmann equation
Time evolution of a homogeneous, isotropic universe.

1. **Friedmann equation version 1**
   If we write down the Einstein equations for the [[#FLRW metric]] one can find two differential equations for the scale factor $a(t)$. One of these expresses energy conservation and the other is $$H(t)^2 := \left( \frac{\dot{a}}{a} \right)^2 = \frac{8\pi G \rho}{3} - \frac{kc^2}{a^2} +\frac{\Lambda c^2}{3}$$where $H(t)$ is the *Hubble parameter*, $\rho$ is the volumetric mass density and $\Lambda$ is the cosmological constant with units $\pu{length^{-2}}$, each of which can vary in time (as can $k$). 

2. **Critical density**
   The critical density of the universe $\rho_c$ is just the mass density $\rho$ at a given cosmological time required to eventually "stop" the expansion of the universe, and for (reasons unclear at the moment) we calculate it by setting $k$ and $\Lambda$ to zero, finding $$\rho_c(t) = \frac{3 H(t)^2}{8\pi G}$$Assuming a zero vacuum energy density ($\Lambda=0$)
   - If $\rho > \rho_c$ the space sections of the universe are closed; the universe will eventually stop expanding, then collapse
   - If $\rho < \rho_c$ they are open, and the universe expands forever
   
3. **Friedmann equation version 2**
   We can then rewrite the Friedmann equation in terms of things we would measure at redshift zero in the following way. Skipping the calculation, if we define $$\begin{align}
   \Omega_M &= \frac{\rho_0}{\rho_{c,0}} = \frac{8\pi G \rho_0}{3 H_0^2}\\
   \Omega_\Lambda &= \frac{\Lambda}{3 H_0^2}\\
   \Omega_k &= -\frac{k}{H_0^2}\quad \text{(note opposite sign of $k$)}\\
   \Omega_r &= \frac{\rho_{rad, 0}}{\rho_{c,0}} = \frac{8\pi G \rho_{rad,0}}{3 H_0^2}
   \end{align}$$where $\rho_0$ represents the matter density only and $\rho_{rad}$ represents the radiation mass density, then we can write the Friedmann equation as $$\frac{H^2}{H_0^2} = \Omega_{rad}(1+z)^4 + \Omega_M(1+z)^3 + \Omega_k(1+z)^2 + \Omega_\Lambda$$which uses in its derivation the relation between scale factors at a certain [[Spectra#Redshift|redshift]] and the scale factor today $a_0$ (can understand as "universe and thus $a$ was smaller at $z$ bigger")$$a_0 = a(1+z)$$Why are the powers as they are? 
   - Radiation gets 3 factors of $a$ from volume density, and an additional factor since the photon energy is redshifted. 
   - Matter is just volume density
   - Curvature and $\Lambda$ I dont have a good explanation for

   Note if we measure any of these $\Omega_i$ along with some other quantities then we could measure $H_0$.