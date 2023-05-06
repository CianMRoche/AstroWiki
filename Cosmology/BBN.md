## BBN
"Big bang nucleosynthesis". The synthesis of light elements in the early universe  ~minutes after the big bang. Has following characteristics:
- The initial conditions (neutron–proton ratio) were set in the first second after the Big Bang, at the neutron "freeze-out" (see below). In general a "freeze out" is when the conditions (like temperature or density) change such that a certain interaction becomes very unlikely to happen. This ratio is the key parameter determining the abundances of light elements after nucleosynthesis ends
- The universe was very close to homogeneous at this time, and strongly radiation-dominated.
- The fusion of nuclei occurred between roughly 10 seconds to 20 minutes after the Big Bang; this corresponds to the temperature range when the universe was <mark class="hltr-pink">cool enough for deuterium to survive, but hot and dense enough for fusion reactions to occur at a significant rate</mark>.

**Deuterium bottleneck**
The fusion reactions are as follows, noting that they almost all involve fusing deuterium$$\begin{align}
\mathrm{p}+\mathrm{n} &\longrightarrow{ }^2 \mathrm{H}+\gamma \\
\mathrm{p}+{ }^2 \mathrm{H} &\longrightarrow{ }^3 \mathrm{He}+\gamma \\
{ }^2 \mathrm{H}+{ }^2 \mathrm{H} &\longrightarrow{ }^3 \mathrm{He}+\mathrm{n} \\
{ }^2 \mathrm{H}+{ }^2 \mathrm{H} &\longrightarrow{ }^3 \mathrm{H}+\mathrm{p} \\
{ }^3 \mathrm{He}+{ }^2 \mathrm{H} &\longrightarrow{ }^4 \mathrm{He}+\mathrm{p} \\
{ }^3 \mathrm{H}+{ }^2 \mathrm{H} &\longrightarrow{ }^4 \mathrm{He}+\mathrm{n}
\end{align}$$The binding energy of deuterium is $2.22\,\pu{MeV}$ so deuterium fusion cant begin until the universe is $\ll 2.22\,\pu{MeV}$. In this time, some neutrons can decay into protons via $\beta$-decay with a lifetime of $890\,\pu{s}$ (this helps reconcile the observed $\ce{He}$ mass fraction from BBN, see below). 

**The neutron-proton ratio**
Set by Standard Model physics before the nucleosynthesis era, essentially within the first 1-second after the Big Bang. Neutrons can react with positrons or electron neutrinos to create protons and other products in one of the following reactions: $$\begin{align}
\mathrm{n}+\mathrm{e}^{+} &\rightleftharpoons \bar{\nu}_{\mathrm{e}}+\mathrm{p} \\
\mathrm{n}+\nu_{\mathrm{e}} &\rightleftharpoons \mathrm{p}+\mathrm{e}^{-}
\end{align}$$At times much earlier than 1 sec, these reactions were fast and maintained the n/p ratio close to 1:1. As the temperature dropped, the equilibrium shifted in favour of protons due to their slightly lower mass, and the n/p ratio smoothly decreased. These reactions continued until the decreasing temperature and density caused the reactions to become too slow, which occurred at about $T = 0.8 \,\pu{MeV}$ (time around 1 second) and is called the <mark class="hltr-pink">freeze out</mark> temperature. 

At freeze out, the neutron–proton ratio was about $1/5$. Why? We can estimate this ratio via a simplified [[Saha equation]] as a function of $T$ $$\frac{n_n}{n_p} \simeq \left(\frac{m_n}{m_p}\right)^{3/2}  \exp \left[-\frac{\left(m_n-m_p\right)c^2}{k_B T}\right]\simeq \exp\left[-\frac{1.3\,\pu{MeV}}{0.8\,\pu{MeV}}\right]\simeq \frac{1}{5}$$where in the second to last step we used that the difference between the neutron and proton masses is $1.3\,\pu{MeV}$ (about 2.6 electron masses), and that the freeze-out temperature for this decay has been measured in the lab to be about $kT\sim 0.8\,\pu{MeV}$. This ratio sets the amount of helium which can possibly be made during BBN.

However, free neutrons are unstable with a mean life of $\sim880\,\pu{s}$; some neutrons decayed in the next few minutes before fusing into any nucleus, so the ratio of total neutrons to protons after nucleosynthesis ends is about $0.15$ (for details see atro 2 notes or Megans notes). This has an observable consequence: the helium abundance. 

**The helium problem**
Lets estimate how much helium we expect to make in BBN relative to other elements, and compare that to observed mass fractions in primordial gases. If the freeze-out neutron to proton ratio is constant up to the point where the universe is cool enough for deuterium to survive, we can make an estimate of the helium mass fraction as follows:

To make a helium 4, we need 2 neutrons. If $n_n/n_p = 0.2$ then we will also have 10 protons. Once the helium is formed, we'll be left with 8 protons. Then the mass fraction of the newly formed helium relative to all involved nucleons is $$f_{He}\simeq \frac{m_{He}}{8m_p + m_{He}} \simeq \frac{4}{12} = \frac{1}{3}$$and we can extrapolate this to the global helium mass fraction by assuming everything is protons and neutrons that want to turn into helium. However, when we observe helium in primordial gas we see a mass fraction of $f_{He}\simeq 0.24$ so what causes this discrepancy? Its the fact that some neutrons decay with the lifetime $\tau \simeq 890\,\pu{s}$ into protons after freezeout (both before BBN starts and during), reducing the number of neutrons around, which restricts the amount of helium we can make. 

The simple version of this argument is to take for granted that BBN takes place over $\sim 200\,\pu{s}$ (the amount of time that must pass before the deuterium is as abundant as the neutrons, details in astro 2 notes and Megans notes) and then make the simplified calculation for the neutron number after freeze-out $$\frac{n_n}{n_p} \simeq \frac{n_n}{n_p}(\text{freezeout})\,e^{-t/\tau} \simeq 0.2 \,e^{-200/890}\simeq 0.15$$where we rounded down from 0.159 to make the next calculation a bit simpler. Now as before we look at the mass fraction, but this time if we want to make $3\,\ce{^4He}$ (chosen for round numbers) we will need $6\,\rm{n}$ and $6/0.15\,\rm{p} = 40\,\rm{p}$ resulting in a mass fraction of $$f_{He}\simeq \frac{3m_{He}}{40m_p + 6m_n} \simeq \frac{12}{46} \simeq 0.26$$which is far closer to the measured value. Account for the fact that not *everything* turns into helium that can, and we have a good match.
