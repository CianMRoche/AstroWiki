A pretty good page on this topic [here](http://spiff.rit.edu/classes/phys440/lectures/optd/optd.html). You'll notice a lot of the things below are just describing the same thing in different ways. Summary is as follows, with all symbols defined below $$\rho\kappa = \frac{1}{l} = n\sigma = \alpha$$

## Optical depth
The measure you use when what you care about is "how much light is absorbed". Relates a physical distance to the absorptivity of a material over that distance. Can be thought of as a measure of distance that "accounts for transparency". Effectively <mark class="hltr-pink">the number of mean free paths traversed</mark>, see [[#Opacity]] and note that for a uniform material its just legth of material / mean free path.$$\tau(z) = \int_0^z \alpha\,dz = \int_0^z \kappa\rho\,dz \underbrace{=\,\sigma N}_{\text{uniform material}}$$where $\alpha$ is the [[#Extinction coefficient]], $\sigma$ is the effective cross section for interaction, $\kappa$ is the [[#Opacity|opacity]] and $N$ is the column number density ($\rm{particles\,m^{-2}}$). People often define this using the Rosseland mean [[#Opacity|opacity]] whereby $\alpha = \kappa \rho$ (which is not frequency-dependent) as above. The **frequency-dependent** optical depth is$$\tau_\nu(z) = \int_0^z \alpha_\nu\,dz = \int_0^z \kappa_\nu\rho\,dz$$

## Extinction coefficient
Dimensions of inverse length. Its basically one over the mean free path, so high extinction corresponds to short mean free paths and light has a "harder time" moving through the material $$\alpha = \frac{1}{l}$$


## Mean free path
Scale length for a scattering process. For volume number density $n$ and effective cross section $\sigma$ (units of area) the mean free path is $$l = \frac{1}{n\sigma}$$For a material with proerties $n$ and $\sigma$ and side length $L$ the probability of a particle scattering in length $dx$ is $n\sigma dx$, since it equals area of scatterers / area of object = $\sigma n L^2 dx / L^2$. (total number of particles in the slab is $n$ times volume $=L^2 dx$). For initial flux $F$ incident on that differential length of material, have $$dF = -F n \sigma dx$$solve to get Lambert-Beer law below. Note we say [[Units#Flux|flux]] instead of [[Units#Intensity|intensity]] as one may see on wikipedia to avoid confusion with the prevelant astronomy usage of these terms.

**Lambert-Beer law**:
Brings us to the solution for incident flux $F_0$ and [[Optical depth#Optical depth|optical depth]] $\tau$
$$F = F_0 e^{-x/l} = F_0 e^{-\tau}$$


## Opacity
AKA "absorption coefficient", labelled $\kappa$, dimensions of "cross section per mass". Expresses the efficiency with which this particular sort of material (hydrogen, or helium, or electrons, etc) absorbs and scatters light. Defined via $$\rho\kappa = \frac{1}{l} = n\sigma = \alpha$$where $\rho$ is the mass density, $l$ is the [[#Mean free path]] and $\alpha$ is the [[#Extinction coefficient]]. In principle $\kappa$, $\sigma$ and $\alpha$ are frequency-dependent.

Since the opacity is frequency-dependent, really the **Rosseland mean opacity** that we are speaking about here. We define the Rosseland mean opacity in terms of the frequency dependent opacity $\kappa_\nu$ as$$\frac{1}{\kappa} = \frac{\int_0^\infty \frac{1}{\kappa_\nu} \frac{\partial B_\nu}{\partial T} d\nu }{\int_0^\infty \frac{\partial B_\nu}{\partial T} d\nu }$$where $B_\nu$ is the [[Blackbody radiation|blackbody]] spectral density. 


## Optical thickness
Loosely defined notion of "how difficult it is for light to get through a unit length of this material". Thickness is an appropriate word because when thinking about distance in terms of [[#Optical depth|optical depth]], a "thick" material is one which has a very short mean free path, and thus a large optical depth. the converse is true for a "thin" material.

**Optically thick**: Many [[#Mean free path|mean free paths]] per unit length
**Optically thin**: Few [[#Mean free path|mean free paths]] per unit length
