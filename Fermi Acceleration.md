Return to [[Overview]]

## Questions

- Power laws
- 2nd order Fermi Acceleration
- 1st order Fermi Acceleration
- Schematic of the scenario

## Shocks 

In High Energy Astrophysics, scenarios frequently arise where the particles involved are not thermailized, and instead of following a Maxwell-Boltzmann distribution, they tend to follow power law distributions. 

One of such scenarios involves strong shocks.

A shock is simply a discontinuity between 2 fluids (such that $\rho$, $v$, and $P$ are discontinous). Note, however, that energy, momentum and flux accross the surface are continous regardless of the shock. They occur when there is a supersonic flow, which arise due to the non-linearity of fluids in this case. 

Now, at the discontinuity, particles diffuse across the shock, converting part of their kinetic energy into acceleration. Fermi came up with a possible explanation, that we now refer to as the *Fermi 2nd Order Acceleration*.

## Fermi 2nd Order Acceleration

Consider a big cloud of mass $M$ moving at a speed $V$ in 1D space, colliding with a test particle of mass $m$ and speed $v$. Using Lorentz transformations combined with conservation of linear momentum (and assuming that $M\gg m$ and $V\ll v$ ), we can show that the change of energy of the test particle is given by:

$$
\frac{\Delta E}{E} \approx \frac{2Vv cos\theta}{c^2} + \frac{2V^2}{c^2}
$$

Now, *Fermi's argument* is that head-on collisions are more frequent than tail-on collisions (just like when we are moving through rain, we get more wet in the front than in the back). This means that we can approximate $\theta \sim 0$ which means that $cos\theta \sim 1$. In this case, we find that:

$$
\frac{\Delta E}{E} \propto \frac{V}{c}
$$

However, if collisions are isotropic, then we'd expect $\langle cos\theta \rangle \approx 0$, and therefore: 

$$
\frac{\Delta E}{E} \propto \frac{V^2}{c^2}
$$

A more careful consideration yields the following:

$$
\bigg \langle \frac{\Delta E}{E} \bigg \rangle = \frac{8}{3} \frac{V^2}{c^2}
$$

Which shows the second-order dependency that gives this acceleration its name. 

Making a careful consideration, this is actually an issue. First, a second order dependency renders the process too slow (since $V^2/c^2 \ll 1$). Second, there is no particular power slope predicted by the 2nd order Fermi acceleration, which contradicts observations where $N(E) \propto E^{-p}$ with $p \in [2,3]$. 

## 1st Order Fermi Acceleration

The trick to get a first order acceleration lays on the fact that, despite there only being a magnetic field in the cloud's reference frame (which wouldn't allow for accelerations since energy is conserved), there *IS* an *electric field* in the lab's and test particle's reference frames.

With a similar setup, the physical situation is as follows:

Rapid scattering renders velocity distributions isotropic in the fast (upstream) and slow (downstream) portions of the shock. Given invariance of Galilean relativity, and using conservation of momentum/energy, one can conclude that the collisions look symmetric from both regions, and separately, they see the particles colliding head-on with a velocity:

$$
V = \frac{3}{4} U
$$

Intuitively, repeated head-on collisions are like a ping-pong ball being hit by paddles. This keeps increasing the energy of the accelerated particle in a way that:

$$
\frac{\Delta E}{E} \propto \frac{V}{c}
$$

A more careful consideration gives an exact result:

$$
\frac{\Delta E}{E} \approx 2\frac{V}{c} cos\theta + 2\frac{V^2}{c^2}
$$

Carefully calculating $\langle cos\theta \rangle$, gives us:

$$
\bigg \langle \frac{\Delta E}{E} \bigg \rangle = \frac{4}{3} \frac{V}{c}
$$

As we'll see, this first order dependence *does* produce the observed power laws for the non-thermalized distributions.

##  Non-Thermalized Distributions (Power Laws)

Suppose that at the shock's boundary, each collision changes a particle's energy by a factor of $\beta$. Additionally, let $P$ be the probability that a particle remains in the acceleration zone after an "acceleration cycle". After $k$ collisions, we would have that the number of particles $N$ and energy $E$ is given by:

$$
N(k) = N_0 P^k
$$
$$
E(k) = E_0 \beta^k
$$

Taking the logarithms gives:

$$
k = \frac{ln(N/N_0)}{lnP} = \frac{ln(E/E_0)}{ln\beta}
$$

Solving for $N$, we get:

$$
N = N_0 \bigg( \frac{E}{E_0} \bigg)^{lnP/ln\beta}
$$

Taking the derivative with respect to $E$ gives:

$$
\frac{dN}{dE} \propto E^{\frac{lnP}{ln\beta} -1 }
$$

For Fermi I acceration, this becomes:

$$
\frac{dN}{dE} \propto E^{-2}
$$

Which is aligned with observations. Fermi II acceleration doesn't yield similar results.