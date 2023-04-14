We will be exhibiting an *SI units bias* because standardizing is good. 

## Degree
Unit of <mark class="hltr-pink">angle</mark>: $1/360$ of a full rotation

**Notation**:
$6^\circ$ = 6 degrees


## Arcminute
Unit of <mark class="hltr-pink">angle</mark>: $1/60$ of a [[#Degree]]
- 60 [[#Arcsecond|arcseconds]]
- 1arcmin ~ 1 Mpc at z=0.7

**Notation**:
$4'$ = 4 arcmin

## Arcsecond
Unit of <mark class="hltr-pink">angle</mark>: 1/60 of an [[#Arcminute]], $1/3600$ of a degree
$12''$ = 12 arcsec
$1'' = \frac{\pi}{180\times3600}\,\pu{rad} \simeq 5\times 10^{-6}\,\pu{rad}$
8kpc per arcsec at z=0.8

## Proper distance
<mark class="hltr-pink">Distance</mark> between objects including expansion of universe; changes in time, in contrast to [[#Comoving distance]].

**Examples**:
- pkpc = proper kiloparsec
- ply = proper light year


## Comoving distance
<mark class="hltr-pink">Distance</mark> between objects factoring out expansion of universe, such that two otherwise unmoving objects will have constant comoving distance over cosmological time. The comoving coordinate system evolves "with" the Hubble flow.


## parsec
Unit of <mark class="hltr-pink">distance</mark>: $1\,\pu{pc}$ is defined as the distance at which a baseline of 1 [[#AU]] results in a parallax angle of one [[#Arcsecond]]. Can be thought of in terms of trying to measure the distance to an object which is at $1\,\pu{pc}$ or simply as being defined by this triangle.
![[parsec.png|500]]

$1\,\pu{pc} \simeq 3\,\pu{ly}\sim 3\times 10^{16}\,\pu{m}$


## AU
Unit of <mark class="hltr-pink">distance</mark>. Distance from Earth to Sun
$1\,\pu{AU} \simeq 1.5\times 10^{11}\,\pu{m}$


## amu
Unit of <mark class="hltr-pink">mass</mark>. "atomic mass units". Defined as 1⁄12 of the mass of a free carbon-12 atom at rest in its ground state.

$1\,\pu{amu}\,\simeq\,1.66\times 10^{-27}\,\pu{kg}$  


## erg
Unit of <mark class="hltr-pink">energy</mark>. Just Joules but smaller. The unit of energy in the CGS unit system.

$1\,\pu{erg}\,=\,10^{-7}\,\pu{J} = 100\,\pu{nJ}$  


## Luminosity
Units of power ($\pu{W}$). The energy per time leaving a (usually astrophysical) body. Intrinsic property of a source.


## Flux
Loosely used, generally refers to some power per area ($\pu{W\,m^{-2}}$). Not intrinsic property of source, depends on "observation"/"location" parameters such as distance from source.

<mark class="hltr-pink">Specific flux</mark> refers to the flux density in frequency space, such that $F_\nu(\nu)\,d\nu$ is the flux in the frequency band from $[\nu,\nu + d\nu]$ 

Can be defined in terms of the [[#Intensity|specific intensity]] via 
$$F_\nu = \int \cos\theta \,d\Omega\,I_\nu$$

## Intensity
Also called <mark class="hltr-pink">"surface brightness"</mark> because it is an intrinsic feature of the source which doesnt depend on how it is observed (ideally). Refers to a flux per solid angle ($\pu{W\,m^{-2}}\,\rm{steradian}^{-1}$). Think "per unit area on my detector, what is the flux I get from a given solid angle on the sky". Since intensity is per unit area and solid angle, changing the size of your detector of viewing area (as long as the source is entirely within that area in each case) will not increase the intensity.![[intensity.png|450]]

<mark class="hltr-pink">Specific intensity</mark> refers to the intensity density in frequency space, such that $I_\nu(\nu)\,d\nu$ is the intensity in the frequency band from $[\nu,\nu + d\nu]$ 

A differential energy element can be expressed in terms of this quantity via (noting in the image above they use $d\sigma$ for area but here we use $dA$ to be consistent with astro 1 notes)$$dE = I_\nu \cos\theta\, d\theta\,dA\, d\Omega\, d\nu\, dt$$
Note that one can also define the (specific) <mark class="hltr-pink">mean intensity</mark> as $$J_\nu = \frac{1}{4\pi}\int d\Omega\,I_\nu$$where $d\Omega$ is a solid angle element (divide by $4\pi$ since there are $4\pi$ steradians on a sphere, want average) which means for an isotropic source $J_\nu = I_\nu$.