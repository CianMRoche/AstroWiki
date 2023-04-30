## Saha equation
The Saha equation uses the Boltzmann factor to calculate the ratio of the population of a particle's state, and the population of the next ionized state (ie after losing one electron) based on their relative energies in a gas at equilibrium. Only valid:
- In thermal equilibrium
- If pressure not too high, so pressure ionization and degeneracy pressure can be neglected
- Simple composition, since more species complicate the picture.

Skipping the derivation (which involves taking the ratio of Boltzmann factors, see [this](https://www.astro.princeton.edu/~gk/A403/ioniz.pdf) and assuming that the thermal De Broglie wavelenth of the unionized and ionized species are approximatesly equal, so they cancel) we have the Saha equation $$\frac{n_{i+1} n_e}{n_i}=\frac{2}{\lambda^3} \frac{g_{i+1}}{g_i} \exp \left[-\frac{\left(\epsilon_{i+1}-\epsilon_i\right)}{k_B T}\right]$$where 
- $n_{i}$ is the density of atoms in the _i_-th state of ionization, that is with _i_ electrons removed.
- $n_e$ is the electron density
- $g_i$ is the degeneracy of states for the i-ions (see below)
- $\epsilon_i$ is the energy required to remove i electrons from a neutral atom, creating an i-level ion. The difference present in the formula is an ionization energy for ionization level $i$ to level $i+1$.
- $m_e$ is the mass of an electron
- $T$ is the temperature of the gas
- $h$ is Planck's constant
- $\lambda$ is the thermal de Broglie wavelength for the electron (for $k_B$ Boltzmann's constant)
$$\lambda  = \sqrt{\frac{h^2}{2\pi m_e k_B T}}$$

If only the first excited state matters and $i$ represents the ground state, then $n_1 = n_e$ and defining the total non-electron density $n = n_0 + n_1$ we have $$\frac{n_e^2}{n - n_e}=\frac{2}{\lambda^3} \frac{g_1}{g_0} \exp \left[-\frac{\chi}{k_B T}\right]$$for first ionization energy $\chi$.

On the degeneracy of states $g$, here is a quick reference table:
$$\begin{align}
\text{ionization of hydrogen:} \quad \chi=13.54 \mathrm{eV}, \quad 2 g_{i+1} / g_i=1\\
\text{first ionization of helium:} \quad \chi=24.48 \mathrm{eV}, \quad 2 g_{i+1} / g_i=4\\
\text{second ionization of helium:} \quad \chi=54.17 \mathrm{eV}, \quad 2 g_{i+1} / g_i=1
\end{align}$$