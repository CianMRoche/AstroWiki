## 1 (a) 
**Describe, qualitatively, the standard model for the formation of the solar system, and discuss observational evidence for this model.**

Formed ~$4.5\,\pu{Gyr}$ ago, obtained by radioactive dating of heavy elements in meteorites

1. Gravitational collapse of gaseous [[Nebulae|nebula]] 
	- Conservation of angular momentum $\implies$ as radius of cloud decreases, spins up, forms [[Accretion#Accretion disk|accretion disk]] 
2. Hot dense, [[Stellar classes#Protostar|protostar]] forms. See [[Star formation]] for details.
3. Planetesimals (~$10\,\pu{km}$) form via collisions of small dust ($1\,\pu{\mu m}$ - $1\,\pu{cm}$), rocks and ices. Type of planetesimal formed depends on composition of material and therefore the temperature in the disk at that location. 
	- Every element has an **ice line**, the radius at which volatiles of that element can condense into ice grains (for water, about 3 AU). Volatiles are easily vaporized things like $\rm{H_2O}$, $\rm{CO_2}$ and $\rm{NH_3}$ (ammonia)
	- **Ice giants** form after this line, **rocky planets** form before this line (closer to star), and there are **gas giants** and their relationship to this line I dont know. Likely inside(?)
	- People also talk about a **soot line** relating to the sublimation of carbon but resources arent great.
4. Once large enough, rocky cores accumulate a gas envelope, becoming a **gas giant**. **Solar wind** prevents inner planets from maintaining gas envelopes early in their development.
5. Moons form via each planetesimal forming its own accretion disk 
6. [[Definitions - The Solar System#Asteroid|Asteroid]] belt (between Mars and Jupiter) forms via perturbtions from Jupiter preventing the gravitational collapse into planets. Even now we see the "**Kirkwood gap**" in asteroid belt orbits, which are gaps in the distribution of semi-major axes of asteroids in the belt due to [[Orbital resonance]] with Jupiter, occurring at integer ratios of the Jupiter:asteroid semimajor axis.
7. Remnant material craters planets and moons
8. Disk is not exactly Keplerian due to pressure gradient, so things drift toward star 
	- Problem: timescale is short relative to formation and growth times. How do they survive? Pressure fluctuates and local pressure maxima allow for more growth

Sarah: People think that planets cant get large enough fast enough to maintain gas envelope without ice

**Observational evidence**
- Locations of rocky planets, gas giants and ice giants within solar system
- Heavy cratering
- All planets roughly in ecliptic plane (formed from same disk)
- [[Definitions - The Solar System#Asteroid|Asteroid]] belt


## 1 (b)
**Describe observations of exoplanets that have challenged this simple picture as a universal explanation for planet formation.**

Existence of hot Jupiters: We've seen Jupiter-like planets near their host stars ($<0.1\,\pu{AU}$). How did they migrate all the way in? A potential resolution is a perturbation of their orbit to a high-eccentricity one, then they tidally migrate the orbit down to a much closer one. 


## 2
**Explain the steps that you would take to show that both the orbital period and the total energy of a Keplerian orbit depend only on the semimajor axis, and not on the orbital eccentricity**

**Energy indep of e**: 
 ----- Method 1 -----
Total energy conserved at any point in the orbit
$$E = T + U_{\rm{eff}} = \frac{1}{2}\mu\dot{r}^2 + \frac{l^2}{2\mu r^2} - \frac{G M_1 M_2}{r}$$
Use the perihelion $\varphi=0$ where $\dot{r} = 0$ and write the energy as
$$E = \frac{l^2}{2\mu}\frac{(1+e)^2}{a^2(1-e^2)^2} - G M_1 M_2\frac{(1+e)}{a(1-e^2)}$$
Where we used the $r(\varphi)$ relationship for a Keplerian orbit
$$r = \frac{a(1-e^2)}{1+e\cos(\varphi)}$$
Then also use $a = \frac{1}{2}(r(0) + r(\pi))$ which implies$$\frac{l^2}{a(1-e^2)\mu} = GM_1M_2$$and replace in the energy equation to get (after a little algebra)$$E =- \frac{G M_1 M_2}{2a}$$
----- Method 2 (ignore this its wrong) ----- 
We make the observation that this answer is the same as the result youd get by applying the virial theorem to a circular gravitational orbit of radius $a$. With that inspiration, we look at the connection between circular orbits and elliptical, namely the "eccentric anomaly": 

Virial theorem is $E = \frac{1}{2}\langle U\rangle$ where$$\langle U\rangle = \frac{1}{P} \int_{\rm{period}} dt\, U(t) = -\frac{1}{P} \int_{\rm{period}} dt\,\frac{G M_1 M_2}{r(t)} = -\frac{GM_1M_2}{\langle r \rangle}$$Nope that last step is totally wrong. There's a nice argument here but I dont have it. Using the angular variable called the "[eccentric anomaly](https://en.wikipedia.org/wiki/Eccentric_anomaly)" which we label $\epsilon$ we can express the radial coordinate as$$r = a(1 - e\cos\epsilon)$$ Then use that over a period, the cosine of $\epsilon$ will average to zero? Then you get result. But argument is wrong so I dont know.

**Orbital period indep of e**: 
Start with the area of an arc $$dA = \int dr\, rd\varphi = \frac{1}{2}r^2 d\varphi$$Then via $l = \mu r^2 \dot{\varphi}$ $$\frac{dA}{dt} = \frac{1}{2}r^2 \frac{d\varphi}{dt} = \frac{l}{2\mu}$$Integrating over a period one gets $A = \frac{l}{2\mu} P$. Looking at the area of an ellipse one sees $A = \pi a b = \pi a^2\sqrt{1-e^2}$. Equating the two expressions for $A$ and making explicit the dependence of $l$ on $a$ and $e$ via the equation $\frac{l^2}{a(1-e^2)\mu} = GM_1M_2$ as in the previous part we have (with a little algebra)$$ \frac{a^3}{P^2} =\frac{G(M_1 + M_2)}{4\pi^2} $$which is independent of $e$.


## 3
**Calculate the approximate distance to the heliopause**:
The scale of the Solar system and heliopause is as follows:
![[solarsystemscale.jpg]]
Note that the [[The Sun#Heliosphere|heliosphere]] is **not spherical** and so the question requires some heavy approximating

We need to balance the pressure from the solar wind with the thermal pressure of the ISM. 
1. The solar wind in the heliosphere can be viewed as exerting a [[Definitions - The Solar System#Ram pressure|ram pressure]] on the [[Interstellar medium|ISM]] as $$P_{\rm{ram}} = \rho_{sw}(R) v^2$$ where $R$ labels the distance from [[The Sun#The Sun|the Sun]] to heliopause, $v$ is the relative velocity of the two bodies and we use the subscript $sw$ for the solar wind. 
	- We can approximate $v$ by assuming the speed of the solar wind is about the escape velocity from the surface of the Sun, and that it maintains a constant speed until reaching the Heliopause. We also treat the ISM as at rest. The escape velocity from the surface of the Sun is$$v\sim v_{\rm{esc},\odot} = \sqrt{\frac{2GM_\odot}{R_\odot}} \simeq 600\,\pu{km s^{-1}}$$
	- We can estimate $\rho_{sw}(r)$ using $\rho_{sw}(R_{\bigoplus}) \simeq n(R_{\bigoplus})\, \mu \, m_H \simeq (6\times10^6 \pu{m^{-3}})\, \frac{1}{2} \, (1.6\times 10^{-27}\,\pu{kg}) \simeq 10^{-21}$ (in SI units) where the number density at 1AU is determined by ground-based measurements, $\mu$ is the [[Mean molecular weight#Mean molecular weight|mean molecular weight ]] (here for an ionized hydrogen gas, so $\mu = \frac{1}{2}$) and the hydrogen mass is about 1 [[Units#amu|amu]]. We extend this value to any $r$ by mass continuity for a spherically symmetric density $\rho$, namely: $\frac{dM}{dr} = 4\pi r^2 \rho(r) = \text{const}$ because the mass integrated over a sphere at any radius should be equal for this simple flow. As a result, we have$$\rho_{sw}(R) = \left(\frac{R_\bigoplus}{R}\right)^2 \rho_{sw}(R_{\bigoplus})$$
2. The thermal pressure of the ISM can be modelled as an ideal gas with pressure $$P_{ism} = n_{ism} k T_{ism}$$ 
	- $n_{ism} \simeq 0.1\,\pu{cm^{-3}}$ as an average of the most abundant [[Interstellar medium|ISM]] components
	- $T_{ism} \simeq 7000\,\pu{K}$ in the same way
	- $k = 1.38\times 10^{-23}\,\pu{m^2 kg s^{-2} K^{-1}}$ is the Boltzmann constant

3. Equating the pressure equations we have$$R = R_{\bigoplus}\sqrt{\frac{\rho_{sw}(R_{\bigoplus})\,v^2}{n_{ism} k T_{ism}}} \sim (7\times 10^8\,\pu{m})\, 10^{\frac{1}{2}(-21+11-5+23-4)} \sim 10^{11}\,\pu{m} \sim 1\,\pu{AU}$$but thats **wrong** and we shouldve gotten ~100 AU. Blame the 3 random numbers I guess. 

**Does the local interstellar medium begin at this boundary? Explain.**
The heliopause is the location where pressure balances betweem the solar wind and the ISM thermal pressure. Thus, this location is by definition at some distance within the ISM, meaning that the ISM begins closer to the Sun than the heliopause, where it is understood that no clear boundary between the species exists.


## 4
**Describe the physics involved in the Earth-Moon interaction whereby the Earth's rotation rate is  
slowing and the orbital separation is increasing.**
Essentially the inverse of [[Binaries#Tidal migration|tidal migration]]; since the Earth is rotating in the same direction as the Moon's orbit, the tidal bulge actually leads the Earth-Moon line, slowing the Earths rotation and giving orbital energy to the Moon.

Moon is receding at $~\sim 3-4\,\pu{cm yr^{-1}}$ 
Earth's rotation period is slowing at $\sim 1\,\pu{ms century^{-1}}$ 

Eventually Earth-Moon orbit will be synchronous and the orbital period will be the same as Earth's rotation period. See also [[Exoplanets - Questions#11]] 

From Megan's notes:
![[Earth_Moon_tidal_interaction.png]]


## 5
**Describe the Oort cloud and the Kuiper belt, and theories of their origins.**
1. Kuiper Belt
   Like the [[Definitions - The Solar System#Asteroid|asteroid]] belt but further out (starts at Neptune $\sim30\,\pu{AU}$ out to {debated} but either 50 or up to 1000 $\pu{AU}$) and thus, more icy (contains volatiles like water, methane and ammonia). Has a similar relationship to Neptune that the asteroid belt has to Jupiter, in terms of the planet preventing the formation of further bodies in that orbital region.
   
   - Contains Pluto and other dwarf planets
   - Disk-shaped
   - First Kuiper belt object (AKA "trans-Neptunian object") discovered by MIT professor+grad student (Jewitt+Luu?)
   - Source of short period comets in the solar system ($P<200\,\pu{yr}$)
   ![[Kuiper_Belt.jpeg]]

2. Oort cloud
   See [[#3]] for diagram. Spherical cloud of [[Definitions - The Solar System#Comet|comets]] from 1000 to 100,000 $\pu{AU}$. 
   Thought to be source of long-period ($P>200\,\pu{yr}$) comets

**Formation/Origins**: the so-called "Nice" model
- Giant planets (like Neptune and Uranus) and Kuiper belt form closer to the Sun 
- Gravitational encounters between planets scatter Neptune to more eccentric orbit that scatters planetesimals outward to form Kuiper belt
- Dynamical friction decreases eccentricity of Neptune's orbit
- [[Definitions - The Solar System#Kozai mechanism|Kozai mechanism]] pushes some objects to higher-inclination orbits
- Does not seem to produce enough low-eccentricity opbects in Kuiper belt, other problems
- Oort cloud objects scattered ut to larger radii
- Even in other models, key feature is outward migration of giant planets


## 6
**Explain why solar system bodies are often found with integer ratios of orbital periods.**
Integers in physics where we dont expect them come from
- Quantum effects
- Symmetries
- Resonances

There are several types of **resonance** at play in the solar system, the two primary being:
1. **Mean-motion resonance**: (see [[Orbital resonance]])
   Essentially creates a stable equilibrium of integer orbit ratios that appears naturally in many types of "multiple objects orbiting a common larger object" systems.
   
   Examples: Kuiper belt resonances with Neptune, asteroid belt resonance gaps with Jupiter, gaps in rings of Saturn due to resonances with moons, Pluto-Neptune at 2:3 ratio.
   
2. **Laplace resonance**:
   1:2:4 period ratio in 3-body orbiting systems. Other 3-body resonances are called "Laplace-like"
   
   Example: Io, Europa and Ganymede moons of Jupiter