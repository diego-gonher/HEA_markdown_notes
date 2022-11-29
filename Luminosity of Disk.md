Return to [[Overview]]

## Questions

- Naive calculation of the Flux $F$ and Luminosity $L$
- Explanation of the factor of 3 in the correct calculation
- Correct derivation of $L$

## A Naive calculation of $F$ and $L$

As we saw in [[Intro to Accretion Disks and ISCO]], the total increase in thermal energy is equal to half of the change in gravitational potential energy:

$$
\Delta E = \frac{1}{2}\Delta U_g \Rightarrow L = \frac{GM\dot{M}}{2r_{in}}
$$

Now, we also know that

$$
F = \frac{L}{4\pi r^2} \sim \frac{GM\dot{M}}{8r^3_{in}}
$$

This is a factor of 3 smaller than our result in [[Equations of Disk Structure]]. The reason why an accretion disk produces 3 times more power locally than from the local release of gravitational potential energy is because viscous stresses transport both energy and angular momentum.

## A correct derivation of $L$

Correctly deriving the luminosity amounts to using the correct expression for the flux and integrating it with respect to a differential of area:

$$
L = 2 \int^\infty_{r_{in}} 2 \pi r F(r) dr
$$

Performing such integration gives us a luminosity of:

$$
L = \frac{GM\dot{M}}{2r_{in}}
$$

Which is the same as our naive attempt at calculating $F$. The explanation is subtle: this does makes sense as the increase of thermal energy indeed is half of the loss in potential energy, but the geometry and the physical considerations of the naive derivation were fundamentally wrong. 

## Radiative efficiency

Using a relativistic approach and the corresponding values for, say, a Schwarzchild BH gtives an efficiency $\eta \sim 1/12$, which corresponds to an efficiency of about 8%.