Return to [[Overview]]

## Questions

- Accretion rate
- Torque
- Flux as a function of radial distance
- Rate of change of angular momentum

## Introduction

To obtain a better description of the structure and properties of accretion disks, we can start by considering the conservation of mass, angular momentum and energy, each of which allow us to gain a great deal of insight.

## Accretion Rate (mass conservation)

Making a simple schematic, it is easy to see that the accretion rate for an accretion disk that has a density $\Sigma$ is given by:

$$
\dot{M} = 2\pi \Sigma r v_{r}
$$

Where $r$ is the radial distance and $v_r$ is the radial velocity, defined to be positive for an inward (accreting) motion. 

## Torque (angular momentum conservation)

Let us define a viscous stress $\tau_{r\phi}$ as the azimuthal force per unit area exerted across an area element which has a normal in the radial direction. 

With $\tau_{r\phi}$, the inner material, which is more rapidly rotating, torques *UP* the outer material. We can find the actual expression for the torque as follows:

$$
\text{Torque} = r \times F = r\times \tau_{r\phi} \cdot \text{Area} =  2\pi r \cdot 2h \cdot \tau_{r\phi} = 4 \pi r^2 h \tau_{r\phi}
$$

This means that the material inside $r$ is losing angular momentum and migrating inwards. 

Calculating the rate at which angular moemntum is lost as a fluid element moves from an outer radius $r_a$ to an inner radius $r_b$, we end up with the following:

$$
\dot{M}(L - L_{in}) = \dot{M} ( \sqrt{GMr} - \sqrt{GMr_{in}})
$$

In order to be able to simplify this expression, we must make a decision on what $\tau_{r\phi}$ is at the inner radius. For simplicity, we can assume that this quantity is equal to zero (no torque boundary condition), but this could be wrong and a better consideration of the physics of the boundary layer is required for a better description of the problem. With this approximation, we find that the torque can be apprixmated as: 

$$
\text{Torque} = 4 \pi r^2 h \tau_{r\phi} = \dot{M} \sqrt{GMr} \bigg(1 - \sqrt{\frac{r_{in}}{r}}  \bigg)
$$

## Flux (energy conservation)

We start by considering the dissipation of heat as photons with the following:

$$
\text{viscous dissipation per unit volume} =  \text{viscous stress} \hspace{0.2cm} \times \hspace{0.2cm} \text{rate of strain}
$$

Which becomes

$$
\text{viscous dissipation per unit volume} = \tau_{r\phi} \times -r\frac{d\Omega}{dr}
$$

From energy conservation, we know that the power dissipated per unit area has to equal the power radiated per unti area. That is:

$$
2h \tau_{r\phi} \cdot -r\frac{d\Omega}{dr} = 2F(r)
$$

Where $F(r)$ is the flux. Remember that:

$$
\Omega = \sqrt{\frac{GM}{r^3}}
$$

Using this, and manipulating the previous expression gives us an equation for the flux:

$$
F(r) = \frac{3}{2}h \tau_{r\phi} \sqrt{\frac{GM}{r^3}}
$$

Lastly, we can replace the viscous stress by using the angular momentum equation from the previous section. That leaves us with:

$$
F(r) = \frac{3GM\dot{M}}{8\pi r^3} \bigg(1 - \sqrt{\frac{r_{in}}{r}}  \bigg)
$$

This is the equation of the flux leaving each face of the disk, and it is considered the *most important equation for the disk structure*. 

A full GR treatment yields a similar result:

$$
F(r) = \frac{3GM\dot{M}}{8\pi r^3}Q \bigg(1 - \frac{r_{in}}{r} \bigg)
$$

Where $Q$ is a spin dependent function. 

