## Hydrostatic equilibrium
Where $M_r$ is mass enclosed within a spherical shell of radius $r$ $$\frac{dP}{dr} = -\frac{GM_{<r}\rho}{r^2} = -g(r)\rho$$ where $g(r)$ is the acceleration due to gravity at the radius $r$.

**Derivation**:
Consider the following shell of mass, where in calculations we relabel $m(r)$ to $M_{<r}$
![[hydrostatic_equilibrium.png|300]]
The gravitational force on this mass shell is $$\mathrm{d} F_g=-\frac{G[\rho(r) \mathrm{d} r \mathrm{~d} A] M_{<r}}{r^2}$$In equilibrium, this gravitational force will be balanced by a pressure, the force of which is given by the difference in pressure pushing "down" from the outside and "out" from the inside, and we define the minus signs so $\mathrm{d} F_P$ points inward  $$\mathrm{d} F_P=[P(r)-P(r+\mathrm{d} r)] \mathrm{d} A=-\frac{\mathrm{d} P}{\mathrm{~d} r} \mathrm{~d} r \mathrm{~d} A$$Balancing the forces as $\mathrm{d} F_g+\mathrm{d} F_P = 0$ one finds $$\frac{dP}{dr} = -\frac{GM_{<r}\rho}{r^2}$$

## Mass continuity
Where $M_r$ is mass enclosed within a spherical shell of radius $r$ $$\frac{dM_{<r}}{dr} = 4\pi r^2 \rho$$**Derivation**:
Fairly straight forward, $\frac{dM_{<r}}{dr}$ is the increase in mass by increasing $r$ by $dr$. Since $dM_{<r}$ is the same as the mass of a shall of radius $r$ and thickness $dr$ which is simply $dM_{<r} = V_{shell}\rho = 4\pi r^2 dr \rho$ we recover the above. 


## Energy conservation
Obtained by simply equating the [[Units#Luminosity|luminosity]] of the star with the net power generated, which has the following contributions, each with dimensions power per mass:
- $\epsilon_n$ : nuclear processes which "produce" energy
- $\epsilon_\nu$ : energy "lost" to neutrinos that will escape (which we'll ignore here) 
- $\epsilon_g$ : the energy produced (or lost) by gravitational expansion (or contraction)
$$\frac{dL}{dr} = 4\pi r^2 \rho\, (\epsilon_n - \epsilon_\nu +\epsilon_g)$$
The last term $\epsilon_g$ can be positive or negative and represents the heat gained or lost in the shell. This will have a pressure and entropy term (from the second law of thermodynamics) but we neglect the pressure term and end up with $$\frac{dL}{dr} = 4\pi r^2 \rho\, \left[\epsilon_n - T\frac{dS}{dt}\right]$$where $S$ is the specific (i.e. per unit mass) entropy. 


## Energy transport
Energy can be transported radiatively or convectively, depending on the density and temperature, see [[Equations of state]]. 

**Radiative**:$$\frac{dT}{dr} = -\frac{3\kappa}{64\pi \sigma} \frac{\rho L}{ r^2 T^3} = -\frac{3\kappa}{16\pi a c}\frac{\rho L}{ r^2 T^3}$$
**Convective/"adiabatic"**:$$\frac{dT}{dr} = \left(1 - \frac{1}{\gamma_{rad}}\right)\frac{T}{P}\frac{dP}{dr}$$where $\gamma_{rad}$ is the [[Polytropes#Polytrope|polytropic]] exponent. Convection occurs when the temperature gradient is large. See [[Stars - Questions#37|Q37]]. 