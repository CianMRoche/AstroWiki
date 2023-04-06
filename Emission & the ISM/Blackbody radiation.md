## Blackbody radiation
Black body spectral power density [interactive](https://phet.colorado.edu/sims/html/blackbody-spectrum/latest/blackbody-spectrum_en.html) with units power/(surface area of "emitter" $\cdot$ solid angle of "detector" $\cdot$ frequency) $\pu{J s^{-1}Hz^{-1}m^{-2} sr^{-2}}$ (ie in the notation of these notes, a [[Units#Intensity|specific intensity]])
$$B_\nu(\nu\,;T) = \frac{2h\nu^3}{c^2}\frac{1}{e^{\frac{h\nu}{kT}} - 1}$$
But can also reforumulate in terms of wavelength. To do the conversion, need to remember that this is a density and perform a change of variables under the integral sign. 
$$\int d\nu B_\nu(\nu;T) = \int d\lambda \underbrace{\frac{d\nu}{d\lambda}}_{= \frac{d}{d\lambda}\frac{c}{\lambda} = -\frac{c}{\lambda^2}}B_\nu(\nu;T) \implies B_\lambda(\lambda;T) = \frac{c}{\lambda^2}B_\nu\left(\frac{c}{\lambda};T\right)$$
where we drop the minus sign because we integrate in the opposite direction for $\lambda$ so the definition of $B_\lambda$ is nice. 

**When redshifted**:
Effective temperature gets redshifted as $$T_{obs} = \frac{T_{emit}}{1+z}$$Why? When you redshift the blackbody spectrum in a constantly proportional way $\nu_{emit} \rightarrow \nu_{obs} = c\nu_{emit}$ for all $\nu$ (here $c = (1+z)^{-1}$, see [[Spectra#Redshift|redshift]]) it has the effect of introducing an effective temperature $T_{eff} = T_{emit}/(1+z)$ so redshifts maintain the BB spectrum form with a different temperature (note this will be a contravariant transformation of $\nu$ so even though $\nu \rightarrow c\nu$ we must actually apply the inverse transformation to the variable in the distribution) $$\mathrm{BB}\sim\exp\left(\frac{h\nu}{kT_{emit}}\right) \longrightarrow \exp\left(\frac{h(1+z)\nu}{kT_{emit}}\right)$$ where the RHS is what we observe, such that effectively we have $$\implies T_{obs} = \frac{T_{emit}}{1+z}$$
Isnt it actually that (1+z)Temit = Tobs? It cant be that since Tobs must be less than Temit for z>0. I think its a covariant vs contravariant thing. We're transforming the x axis rather than the curve maybe?


## Wien's displacement law
The wavelength at which the spectrum has its peak is inversely proportional to temperature
$$\lambda_{peak} \propto \frac{1}{T}$$
but the constant of proportionality depends on the solution of an implicit equation. A good reference point is $$\lambda_{peak} \simeq \frac{3}{T\,[K]}\,\pu{mm} = \frac{3\times 10^{-3}}{T\,[K]}\,\pu{m}$$
such that at room temp, peak is at ~10 microns. We can also express this in $\pu{eV}$ via the energy-wavelength relation in [[Fun conversions]] $$E_{peak} = \frac{hc}{\lambda_{peak}} \simeq \frac{10^{-6}\,\pu{eV\,m}}{3\times 10^{-3}\,\pu{m}} T\,[\pu{K}] \simeq \left(3\times 10^{-4}\,T\,[\pu{K}]\right)\,\pu{eV}$$


## Stefan-Boltzmann Law
Obtained by integrating over solid angle, area and frequency, $L$ in units of $\pu{W} = \pu{J s^{-1}}$
$$L = \underbrace{\frac{2\pi^5 k^4}{15 h^3 c^2}}_{\colon = \sigma} A T^4$$
where we have defined the Stefan-Boltzmann constant $\sigma = 5.67\times 10^8 \,\pu{W\,m^{-2}\,K^{-1}}$ 

