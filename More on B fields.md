Return to [[Overview]]

## Questions

- What are the typical B-field values?
- How are they measured?
- Give basic idea behind Faraday rotation
- How to measure RM?

## Typical B-Field values

These are some of the typical values for the magnetic fields found in astrophysics:

- *Clusters and galaxies:* $\sim 10^{-6}$ G
- *Sun's photosphere*: $\sim 10^{3}$ G
- *Accretion Disk's*: $\sim 10^{9}$ G

There are a few different methods to measure astrophysical magnetic fields, which include using *Zeeman splitting*, *synchroton emission*, but most importantly, *Faraday Rotation*.

## Faraday Rotation
Suppose that there is a source of polarized radio source. If we assume that the polarized emission is linear, then we know that it can be decomposed into two circular polarizations which propagate with two different velocities, given by:

$$
v_{ph,\pm} = \frac{\omega}{k_{\pm}}
$$
Where $k_{ph,\pm}$ is a function of the plasma frequency $\omega_p$ and the cyclotron frequency $\omega_c$. Now, this means that different circular polarizations will reach the observer at a different phase. The difference of these phases is detected as a difference in rotation angle, which is expressed by:

$$
\Delta \phi = \int (k_+ - k_-) \hspace{0.2 cm} dS = \lambda^2 \int_0^L n B_{||} \hspace{0.2cm} dS = \lambda^2 \hspace{0.2cm}\text{RM}
$$

Clearly, we need guesses for $n$ and $L$. Once that is done, we can see that a plot of $\Delta \phi$ as a function of $\omega^{-2}$ is linear, and the slope is proportional to RM. It is important to note that this is only a lower limit on $B_{||}$, since field reversals are possible and cancel each other. 
