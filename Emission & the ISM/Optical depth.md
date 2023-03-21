## Optical depth
Relates a physical distance to the absorptivity over that distance. Can be thought of as a measure of distance that "accounts for transparency". Effectively "the number of mean free paths traversed".$$\tau = \int_0^z \alpha\,dz = \sigma N$$where $\alpha$ is the [[#Extinction coefficient]], $\sigma$ is the effective cross section for interaction and $N$ is the column number density ($\rm{particles\,m^{-2}}$)


## Extinction coefficient


## Mean free path
Scale length for a scattering process. For volume number density $n$ and effective cross section $\sigma$ (units of area) the mean free path is $$l = \frac{1}{n\sigma}$$For a material with proerties $n$ and $\sigma$ and side length $L$ the probability of a particle scattering in length $dx$ is $n\sigma dx$, since it equals area of scatterers / area of object = $\sigma n L^2 dx / L^2$. (total number of particles in the slab is $n$ times volume $=L^2 dx$). For initial flux $F$ incident on that differential length of material, have $dF = -F n \sigma dx$ solve to get:

**Lamber-Beer law**:
Brings us to the solution for incident flux $F_0$
$$F = F_0 e^{-\frac{x}{l}}$$