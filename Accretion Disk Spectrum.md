Returnt to [[Overview]]

## Questions

- Proper version of the Planck function
- Three different parts of an accrection disk's spectrum

## Planck Function

The version that we use for the Planck Function is the following:

$$
I_\nu = \frac{2h\nu^3}{c^2}\frac{1}{e^{h\nu/kT} - 1}
$$

Which is different from the most common one, since that version gives the frequency distribution of energy density. For our purposes, it suffices to know that Planck's function gives:

$$
I_\nu \propto \frac{\nu^3}{e^{h\nu/kT} - 1}
$$

Now, BB radiation is isotropic, but several scenarios in astronomy actually present anisotropic radiation fields. This means that we need to use a specific intensity that is also a function of direction. In this case, calculating the flux is thus given by:

$$
F_\nu \propto \nu^3 \int \frac{r}{e^{h\nu/kT(r)} - 1} dr
$$

Now we must consider how different values of $h\nu/kT(r)$ shape the disk's spectrum.

## Accretion Disk Spectrum

In this model, there are three parts to the spectrum:

### $h\nu \gg kT_{max}$

In this case, the flux simply follows the same shape as the usual Wien Spectrum, such that:

$$
F_\nu \propto \nu e^{-h\nu/kT}
$$

### $h\nu \ll kT_{min}$

We would expect the disk to have a finite outer radius, which means that there is a minimum disk temperature $T_{min} = T(r_{out})$. This lands us on the other end of the spectrum, which now follows the shape of the Rayleigh-Jeans distribution:

$$
F_\nu \propto \nu^2
$$

## The middle part

In between the previous two parts of the spectrum, the shape at every frequency $\nu$ will be dominated by an annulus with temperature $kT(r) \approx h\nu$. Using the fact that $T(r) \propto r^{-3/4}$ (as we saw in [[Local Spectral Temperature]]), then the integration yields the following:

$$
F_\nu \propto \nu^{1/3}
$$

Combining these three parts allows us to get a rough sketch of the shape of these spectra, which you can find in the notes for Lecture 11. 