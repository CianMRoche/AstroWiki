## Recombination
The time at which the universe had expanded and cooled enough after the big bang for half of the ionized hydrogen to recombine. Happened at $z\simeq 1100$

**Redshift of recombination**:
If we assume 
- a simplified model of the universe as "one level hydrogen atoms" (that is only protons and electrons and a 1-level H atom with ionization energy $\chi = 13.6\,\pu{eV}$)
- treat via the [[Saha equation]] 
- $T = T_0(1+z)$ because $\rho_{rad} \propto (1+z)^4$ (see [[FLRW#Friedmann equation|Friedmann eq]]) and also $\rho_{rad} \propto P_{rad} \propto T^4$ (see [[Stars/Equations of state|EoS]])
- Number density of protons given by $$n_p = \frac{\rho_b}{m_p} = \frac{\Omega_b\rho_{crit,0}(1+z)^3}{m_p}$$
Then we can get the redshift where half ionized (ie $n_p = n_e = n_H$) via Saha $$n_p = \frac{n_p^2}{n_p}=\left(\frac{2\pi m_e k_B T_0(1+z)}{h^2}\right)^{3/2} \exp \left[-\frac{\chi}{k_B T_0(1+z)}\right]$$by equating the two expressions for $n_p$ and solving numerically for $z$ finding $z_{rec}\simeq 1500$ but this is an overestimate. Why?
- There are other elements which will recombine earlier due to higher ionization energies
- The H atom does not recombine straight to the ground state. Instead it will spend some time with the electron in an excited state and the de-excite eventually. The 2-level treatment of the hydrogen atom in this context gives a different redshift (see image below)

![[recombination.png|300]]