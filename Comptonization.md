Return to [[Overview]]

## Questions

- Rise of Bose-Einstein distribution
- Energy exchange per scatter
- Number of scatters depending on different opacities
- Energy spectrum


## Definition

Comptonization is the redistribution of the energies of photons that are scattered by electrons in space

## Rise of Bose-Einstein Distribution

A scenario where a source of EM radiation is within a region where electrons are free to move is prone to comptonization. As a refresher, the power output for a single electron is given by the Compton Power:

$$
P_{compton} = \frac{4}{3} \sigma_T c \gamma^2 \beta^2 U_{photon}
$$

If the electrons are not relativistic, then the energy jumps are going to be small, causing a diffusion in energy space. Assuming a homogenous plasma and an isotropic radiation field, we arrive at *Kompaneets Equation*. This equation is a bit complicate, but an equilibrium solution to it is given by $dn/dt =0$, where $n$ is the photon occupation number of a given energy state. Finding this equilibrium solution gives us:

$$
n = \frac{1}{e^{x+\alpha} - 1}
$$

Which is the Bose-Einstein distribution with $x=h\nu/kT$ and a non-zero chemical potential $\alpha$. Look at the notes for *Lecture 7* for a sketch of this plot.

## Comptonization of Soft Photon Source by Hot Corona

In this scenario, the spectrum is determined by a competition between the Compton diffusion in energy space and the photon escape for the system. Plotting $logI_{\nu}$ as a function of $log\nu$ looks like a compostion of the sources BB radiation and a continium made of the 1st, 2nd, 3rd... order scatterings. Such continium ends around where the energy of the photon is comparable to the thermalized energy of the electrons $kT \sim h\nu$. To find a proper description, a detailed treatment to solve the radiative transfer equation is required. 

However, we can make a crude approximation. Assume a photon escape with a term (Escape probability approximation):

$$
\frac{\partial n}{\partial t} \bigg|_{esc} = \frac{n}{\text{no. of scatterings} \times \frac{\lambda}{c}}
$$

Where $\lambda$ is the mean free path:

$$
\lambda = \frac{1}{n_e\sigma_T}
$$

Now, to calculate the no. of scatterings, we can consider two cases depending on the optical depth $\tau = R/\lambda$ (where $R$ is the size of the system):

$$
\text{if} \hspace{0.2cm} \tau < 1 \hspace{0.2cm} \text{then} \hspace{0.2cm} \text{no. of scatterings} \hspace{0.2cm} = \tau
$$
$$
\text{if} \hspace{0.2cm} \tau \gg 1 \hspace{0.2cm} \text{then} \hspace{0.2cm} \text{no. of scatterings} \hspace{0.2cm} = \tau^2
$$

Using this and going back to Kompaneets Equation, we find that energy exchange is important if 

$$
y\sim\frac{kT}{m_e c^2} \text{max} [\tau, \tau^2] > 1
$$

This $y$ parameter is known as the *Compton y-parameter*, and conceptually:

$$
y \approx \text{fractional energy change per scattering} \hspace{0.2cm} \times \hspace{0.2cm} \text{no. of scatterings} 
$$

## The emerging spectrum

Lastly, we can get approximations to $I_\nu$ by considering the limiting cases for $y$ and $x$.

From the diffusion equation, approximations can be made to land us at:

$$
I_\nu \propto \nu^3 n \propto \nu^{m+3}
$$

If $y \gg 1$, then $m \approx 0$, and therefore we find that:

$$
I_\nu \propto \frac{\nu^3}{e^{x+\alpha} -1}
$$

Considering the limits of $x$, we finally get:

$$
\text{if} \hspace{0.2cm} x \ll 1 \hspace{0.2cm} \text{then} \hspace{0.2cm} I_\nu \propto \nu^3
$$

$$
\text{if} \hspace{0.2cm} x \gg 1 \hspace{0.2cm} \text{then} \hspace{0.2cm} I_\nu \propto \nu^3 e^{-x}
$$

Despite of this model's approximations, it is qualitatively correct.