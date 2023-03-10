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
6. Asteroid belt (between Mars and Jupiter) forms via perturbtions from Jupiter preventing the gravitational collapse into planets. Even now we see the "**Kirkwood gap**" in asteroid belt orbits, which are gaps in the distribution of semi-major axes of asteroids in the belt due to orbital resonance with Jupiter, occurring at integer ratios of the Jupiter:asteroid semimajor axis.
7. Remnant material craters planets and moons
8. Disk is not exactly Keplerian due to pressure gradient, so things drift toward star 
	- Problem: timescale is short relative to formation and growth times. How do they survive? Pressure fluctuates and local pressure maxima allow for more growth

Sarah: People think that planets cant get large enough fast enough to maintain gas envelope without ice

**Observational evidence**
- Locations of rocky planets, gas giants and ice giants within solar system
- Heavy cratering
- All planets roughly in ecliptic plane (formed from same disk)
- Asteroid belt


## 1 (b)
**Describe observations of exoplanets that have challenged this simple picture as a universal explanation for planet formation**

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

**Orbital period**: $$dA = \int dr\, rd\varphi = \frac{1}{2}r^2 d\varphi$$Then via $l = \mu r^2 \dot{\varphi}$ $$\frac{dA}{dt} = \frac{1}{2}r^2 \frac{d\varphi}{dt} = \frac{l}{2\mu}$$Integrating over a period one gets $A = \frac{l}{2\mu} P$. Looing at the area of an ellipse one sees $A = \pi a b = \pi a^2\sqrt{1-e^2}$. and fill in etc to get P= not a function of e