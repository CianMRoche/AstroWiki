## FLRW metric
"Friedmann–Lemaître–Robertson–Walker". The general form of the metric follows from the assumptions of an expanding/contracting universe which is
- homogeneous
- isotropic

These assumptions lead to a form of the metric $$- c^2 d\tau^2 = -  c^2 dt^2 + a(t)^2d\mathbf{\Sigma}^2 $$where $d\mathbf{\Sigma}$ is the line element on a 3D space of uniform curvature $$d\mathbf{\Sigma}^2 = \frac{dr^2}{1 - kr^2} + r^2 d\mathbf{\Omega}^2,\quad\text{where }d\mathbf{\Omega}^2 = d\theta^2 + \sin^2{\theta} d\varphi^2$$where $k$ represents the type of curvature of the space 

| $k$  | Curvature | Topology | Example          |
| :------: | :-----------: | :----------: | :------------------: |
| $+1$ | positive  | closed   | 3-sphere         |
| $0$  | zero      |          | Euclidean space  |
| $-1$ | negative  | open     | Hyperbolic space |

and in this parameterization $a$ has dimensions of length (and represents the radius of curvature) and $r$ is dimensionless. In these coordinates, $r,\theta,\varphi$ are all comoving coordinates which are invariant under the expansion of the universe, which is described by $a(t)$. 

In such a universe, the relation between scale factors at a certain [[Spectra#Redshift|redshift]] $z$ and the scale factor today, which we write as $a_0$ is given by $$a(z) = \frac{a_0}{1+z}$$(can understand as "universe and thus $a$ was smaller at $z$ bigger"). We usually define $a$ such that $a_0=1$.


## Friedmann equation
Time evolution of a homogeneous, isotropic universe.

1. **Friedmann equation version 1**
   If we write down the Einstein equations for the [[#FLRW metric]] one can find two differential equations for the scale factor $a(t)$. One of these expresses energy conservation and the other is $$H(t)^2 := \left( \frac{\dot{a}}{a} \right)^2 = \frac{8\pi G \rho}{3} - \frac{kc^2}{a^2} +\frac{\Lambda c^2}{3}$$where $H(t)$ is the *Hubble parameter*, $\rho = \rho_M + \rho_r$ is the volumetric mass density (often easier to think of $\rho = \epsilon/c^2)$ where $\epsilon$ is the energy density of matter including rest energy, thermal energy and things like radiation energy density) and $\Lambda$ is the cosmological constant with units $\pu{length^{-2}}$, each of which can vary in time (as can $k$). We can rewrite this in a convenient form as $$\begin{align}
   H(t)^2 &= \frac{8\pi G}{3}\left(\rho_M + \rho_r - \frac{3kc^2}{8\pi G}\frac{1}{a^2} + \frac{\Lambda c^2}{8\pi G}\right)\\
   &=: \frac{8\pi G}{3}\left(\rho_M + \rho_r + \rho_k + \rho_\Lambda\right)
   \end{align}$$   
2. **Critical density**
   The critical density of the universe $\rho_c$ is just the mass density $\rho$ at a given cosmological time required to "close" the universe. We can derive it by finding the $\rho$ that makes $k=0$. 
   - If we have $\Lambda \neq 0$ the the "$\rho$" we refer to in $\rho_c$ is $\rho = \rho_M +\rho_r + \rho_\Lambda$  
   - If we assume $\Lambda = 0$ then the "$\rho$" we refer to in $\rho_c$ is $\rho = \rho_M +\rho_r$. People often do this, but it is not necessary to do so.  
  
   In either case we express this as $$\rho_c(t) = \frac{3 H(t)^2}{8\pi G}\quad,\quad \rho_c := \frac{3 H_0^2}{8\pi G}$$   
   - If $\rho > \rho_c$ the space sections of the universe are closed; the universe will eventually stop expanding, then collapse
   - If $\rho < \rho_c$ they are open, and the universe expands forever

   This can be discussed in terms of the parameter $\Omega(t):= \rho(t)/\rho_c(t)$ and whether it is larger or smaller than 1 (time-dependence made explicit as when we dont write it, it is often implied we mean evaluated at redshift 0). 
   
   Important note: when we talk about mean densities of the universe (for example in [[Cosmology - Questions#132|this question]]) we mean the **matter** density, and so $\bar{\rho}(z) = \Omega_{M ,0}(1+z)^3\rho_{c,0}$ where for clarity we wite the zeroes explicitly that are usually left out.
   
3. **Friedmann equation version 2**
   With this definition we can rewrite the Friedmann equation above in terms oftghings we wouldmeasure today like $H_0$ (by evaluating the above at redshift 0) and the critical density (at redshift 0) as $$\begin{align}
   \left(\frac{H(z)}{H_0}\right)^2 = \frac{\rho(z)}{\rho_c} &= \frac{\rho_M}{\rho_c} + \frac{\rho_r}{\rho_c} + \frac{\rho_k}{\rho_c} + \frac{\rho_\Lambda}{\rho_c}\\
   &= \frac{\rho_{M,0}}{\rho_{c}}(1+z)^3 + \frac{\rho_{r,0}}{\rho_{c}}(1+z)^4 + \frac{\rho_{k,0}}{\rho_{c}}(1+z)^2 + \frac{\rho_{\Lambda,0}}{\rho_{c}}
   \end{align}$$where the redshifts come from the fact that mass densities go as $\text{volume}^{-1} \sim a^{-3} \sim (1+z)^3$ and for radiation one finds an extra factor of $(1+z)$ due to the redshifting of the photons. The curvature and cosmological constant ones come straight from the original form of Friedmann equation.
   
   such that making the following substitutions$$\begin{align}
   \Omega_M &= \frac{\rho_{M,0}}{\rho_{c}} = \frac{8\pi G \rho_{M,0}}{3 H_0^2}\\
   \Omega_r &= \frac{\rho_{r, 0}}{\rho_{c}} = \frac{8\pi G \rho_{r,0}}{3 H_0^2}\\
   \Omega_k &= \frac{\rho_{k,0}}{\rho_{c}} =  -\frac{kc^2}{H_0^2}\quad \text{(note opposite sign of $k$)}\\
   \Omega_\Lambda &= \frac{\rho_{\Lambda,0}}{\rho_{c}} = \frac{\Lambda c^2}{3 H_0^2}\\
   \end{align}$$then we can write the Friedmann equation as $$\frac{H(z)^2}{H_0^2} = E^2 (z) = \Omega_{r}(1+z)^4 + \Omega_M(1+z)^3 + \Omega_k(1+z)^2 + \Omega_\Lambda$$Note if we measure any of these $\Omega_i$ along with some other quantities then we could measure $H_0$.

The scale factor $a$ evolves differently over time depending on the "type" of universe (choices of the different $\Omega$) and some common examples are shown in the figure below
![[scale_factor_universe_types.png]]