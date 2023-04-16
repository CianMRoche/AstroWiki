## Apparent magnitude
A measure of "how much flux do we observe from a thing", scales oddly so <mark class="hltr-pink">low magnitudes mean bright things</mark>. Apparent magnitude differences due to differences in observed [[Units#Flux|flux]] $F$ are given by $$\Delta m = m_1 - m_2 = -2.5\log _{10}\left(\frac{F_1}{F_2}\right)$$If observing with a filter $X$ (such as the passbands in the [[#UBVRI]] system) which has reference point "zero-point" flux $F_{X,0}$ then the apparent magnitude in that filter is $$m_X = -2.5\log _{10}\left(\frac{F_X}{F_{X,0}}\right)$$This also implies that the magnitude will change depending on your chosen zero-points. This is the issue of choosing a magnitude system, an example of which is the Vega magnitude system which places the star Vega at magnitude 0 in all bands (but the spedctral energy density of Vega isnt flat so this makes for a weird magnitude system). AB magnitude system makes a bit more sense.

## Absolute magnitude
[[#Apparent magnitude]] that would be measured at a distance of $10\,\pu{pc}$, labelled by $M$. Since $F \propto 1/r^2$ we can write for an apparent magnitude $m$ measured at a distance $d$ <mark class="hltr-pink">measured in pc</mark> (and ignoring the filter subscript $X$ as in apparent magnitudes)  $$M - m = -2.5\log _{10}\left(\frac{F_{10\rm{pc}}}{F_{d}}\right) = -2.5\log _{10}\left(\frac{L}{L}\frac{d^2}{(10\,\pu{pc})^2}\right) = -5\left(\log_{10}d - 1 \right)$$or equivalently we can get $d$ in $\pu{pc}$ via $$d = 10^{\frac{m - M + 5}{5}}$$

## Bolometric magnitude
The [[#Absolute magnitude]] across all wavelengths, were we able to observe the emission with perfect efficiency (ie no filter, absorption, extinction etc). For a star labelled $\star$ we then have relative to [[The Sun#The Sun|the Sun]] $$ M_{bol,\star} - M_{bol,\odot} = -2.5\log _{10}\left(\frac{L_\star}{L_\odot}\right)$$

## Photographic magnitude
A measure of the relative brightness of a star or other astronomical object as imaged on a <mark class="hltr-grey">photographic film emulsion</mark> with a camera attached to a telescope. Has since been superseded by [[Electronics#CCD|CCD]] photometry and alternative magnitude systems such as [[#UBVRI]]


## UBVRI
Also called the Johnson/Bessel (or maybe even Johnson-Cousins?) system. A set of defined photometric filters used for source classification.

- Ultraviolet
- Blue
- Vert (green) / "visual"
- Red
- Infrared
![[UBVRI.jpg]]