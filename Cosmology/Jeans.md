## Jeans equation
Start with the collisionless Boltzmann equation and take the first moment (multiply it by $\mathbf{v}$ and integrate over velocity space) to end up with $$\frac{D\mathbf{v}}{Dt} = -\nabla \Phi - \frac{1}{\rho}\nabla P$$where $D/Dt = \partial/\partial t + (\mathbf{v}\cdot\nabla)$ is the convective dervative. Here $\Phi$ is the gravitational potential and $P$ is the pressure.


## Jeans length
The Jeans length is the length scale above which a body will gravitationally collapse. Consider sound crossing time of a perturbation in a gas. If the sound crossing time (the timescale over which the material can respond) is longer than the [[Timescales#Dynamical timescale|free fall timescale]] then the material will collapse. Therefore for a length scale $\lambda$ we have collapse when $$\frac{\lambda}{c_s} > \frac{1}{\sqrt{G\rho}} \implies \lambda_J \simeq \sqrt{\frac{c_s^2}{G\rho}} \simeq \sqrt{\frac{\pi c_s^2}{G\rho}}$$where in the last step we were really off by a factor of $\sqrt{\pi}$ (see [[Cosmology - Questions#130|Q130]] for reason). Can also derive from virial theorem. 


## Jeans mass
The Jeans mass is just the mass contained within a sphere of radius equal to the [[#Jeans length]]
$$M_J = \frac{4}{3}\pi \lambda_J^3 \rho$$


## Jeans analysis