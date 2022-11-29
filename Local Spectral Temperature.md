Return to [[Overview]]

## Questions

- How does temperature $T$ scale with $r$
- How does temperature scale with $M$
- Implications of our calculations

## Effective Temperature $T_{eff}$

Using the flux we obtained in [[Equations of Disk Structure]], we can find the effective temperature doing the following:

$$
F = \sigma_B T_{eff}^4 \Rightarrow T_{eff} = \bigg( \frac{F}{\sigma_B} \bigg)^{1/4}
$$

Using the corresponding expression for the flux, we are left with:

$$
T_{eff} = \bigg( \frac{3GM\dot{M}}{8 \pi r^3 \sigma_B} 
\bigg(1 - \frac{r_{in}}{r} \bigg)  \bigg)^{1/4}
$$

That is, the effective temperature scales as:

$$
T_{eff}(r) \propto r^{-3/4}
$$

Which intuitively shows that inner parts of the disk are hotter than the outer parts. 

## Scaling with mass $M$

To get a sense on how $T_{eff}$ scales with the mass $M$ fo the central object, we can use the following expressions:

$$
L_{edd} = \eta \dot{M}_{edd} c^2 = \frac{4\pi G M m_p}{\sigma_T}
$$
Which tell us that:

$$
L_{edd} \propto \dot{M}_{edd} \propto M
$$

In conjuction with the gravitational radius $r_g$:

$$
r_g = \frac{GM}{c^2}
$$

To find that

$$
T_{eff} \propto \bigg( \frac{M\dot{M}}{r^3} \bigg)^{1/4} \propto M^{-1/4}
$$

That means that smaller objects tend to be hotter.

## Implications

Using a more careful derivation and actual values, we find that:

- BHs and neutron stars should be x-ray sources
- Accreting WDs should be optical/UV sources
- SMBHs shoud be UV sources
- YSOs with accreting disks shoudl be IR/optical sources

All of which agree with observations
