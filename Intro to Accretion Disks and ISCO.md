Return to [[Overview]]

## Questions

- Concept behind accretion disks
* Characteristic size of the innermost stable orbit is relativistic radius

## Intro to Accretion Disks

As we saw in the notes for the [[Bondi Accretion Rate]], infalling matter that initially doesn't have any angular momentum into a gravitational source is radiatively inefficient because the velocity of infall is too fast and the optical depth is low, both of which don't allow for a proper dissipation of energy in the form of radiation. For a high radiative efficiency, we need:

1) Gravitational energy to be converted into internal energy $U$
2) Increase the cooling rate
3) Increase the infall flow time, so that there is enough time to radiate

All of this can be achieved if the infalling matter has a *non-zero angular momentum* initially.

Consider inflowing material with an angular momentum $L$. If the material conserves angular momentum, then eventually the structure it forms must become rotationally supported since the centrifugal force has steeper radial dependence than the gravitational force. This modifies the gravitation potential energy $\phi$, leaving us with an effective version of it:

$$
\phi_{eff} = \frac{L^2}{2r^3} - \phi
$$

Making a plot of this effective potential energy as a function of the radial distance $r$ gives us insight about the shape of the possible orbits (both bounded and unbounded). Of special interest is the critical point corresponding to a minimum of $\phi_{eff}$, since it corresponds to circular orbits.

Since the material ends up forming a disk, we can find an angular velocity $\Omega$ as a function of $r$ by using basic circular motion and dynamics:

$$
\Omega \propto \sqrt{\frac{GM}{r^3}} \propto r^{-3/2}
$$

This dependency on $r$ causes shear (differential rotation). That is, elements that are closer to the center move faster than those in the outer parts of the disk. 

If we now introduce viscosity and dissipation, such that something actually hapens, then the inner parts of the disk would be slowed down and the outer parts would speed up. It is thus the case that *matter flows inwards as angular momentum flows outwards*. 

## Energy

Now let us consider the mechanical energy of the infalling matter. Per unit mass, we have the following:

$$
\frac{\text{KE}}{m} = \frac{1}{2}v^2 = \frac{GM}{2r}
$$

$$
\frac{U_g}{m} = - \frac{GM}{r}
$$

And consequently, the total mechanical energy is:

$$
\frac{\text{E}}{m} = \text{KE} + U_g = - \frac{GM}{2r}
$$

Which is an easy result from the virial theorem for circular orbits:

$$
E = U + K = \frac{1}{2} U = -K
$$

Now, if the fluid element moves inward, it undergoes a change of energy given by:

$$
\Delta E = \frac{1}{2} \Delta U
$$

That is *the inward motion of the fluid element cuases it to lose an energy equivalent to half ot the potential energy it loses, which is released as heat*. This process continues until the fluid element reaches the *Innermost Stable Circular Orbit*.

## ISCO

In classical mechanics, an object orbiting around another could possibly become as close as possible to the central object. In GR, however, the scenario is more complicated. As a first consideration, the orbital speed of the object cannot exceed the speed of light. That is, the radius $r_{ISCO}$ of the smallest possible circular orbit is given by:

$$
mc^2 = \frac{GMm}{r} \Rightarrow r_{ISCO} \sim \frac{GM}{c^2}
$$

A more careful consideration gives the radius of the ISCO that depends on the spin of the BH and its direction with respect to the direction in which the fluid element is orbiting. 

The total energy of the fluid element that is processed through the disk is simply the bidning energy of ISCO as measured at infinity, and it is about $\sim 0.05mc^2$ for a Schwarzchild BH and $\sim 0.42mc^2$ for a Kerr BH with direct orbits.