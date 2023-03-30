## Polytrope
A pseudo-stellar object modelled by the pressure-density relation $$P = \kappa \rho^{\gamma} = \kappa \rho^{1 + \frac{1}{n}}$$for $\kappa$ a constant, $\gamma$ the "polytropic exponent" and $n$ the "polytropic index". We have the following cases for $n$: $$n = \cases{0&\text{rocky planets}\\
0-1&\text{neutron star}\\
1.5&\text{non-rel degenerate (low mass WD) convective core}\\
3&\text{relativistic degenerate (high mass WD) / radiative zone (Sun)}\\
\infty&\text{isothermal sphere}
}$$We can make the ansatz that $$\rho = \rho_c\,\theta\,{}^n$$such that under this assumption, we can write $$P = \kappa\rho^{1 + \frac{1}{n}} = \kappa \rho_c^{1 + \frac{1}{n}}\,\theta\,{}^{n+1} = P_c\,\theta\,{}^{n+1}$$ with boundary conditions $$\theta(r=0) = 1\quad,\quad\theta(r=R) = 0$$It turns out $\theta$ represents a dimensionless temperature and $\theta\,{}^n$ a dimensionless density (astro 1 pset). Substituting this ansatz into the $r$-derivative of the [[Stellar structure equations#Hydrostatic equilibrium|hydrostatic equilibrium]] equation and defining some variables $$a^2 := \frac{(n+1)P_c}{4\pi G\rho_c^2} \quad,\quad \xi = \frac{r}{a}$$we find the **Lane-Emden equation** $$\frac{1}{\xi}\frac{d}{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right) = -\theta\,{}^n$$which completely specifies the mass, radius, density and pressure profiles of a polytrope. 

**Motivation**:
The [[Stellar structure equations]] are complicated, but much of the difficulty comes from the third and fourth ($L$ and $T$). If we just take the first two equations (hydrostatic equilibrium and mass continuity) we arrive at a system that may or may not describe a physically realistic thing, which yields the polytrope equation above when solved.