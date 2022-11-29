Return to [[Overview]]

## Questions

- Radiative Processes
- Why do electrons radite the most?
- Cyclotron frequency
- Synchroton frequency
- Inverse Compton
- Power of syn
- Power of IC

## Radiative Processes

We know that accelerating charges emit radiation in the form of electromagnetic waves. There are a few different mechanisms for this, but in the case of continiuum processes, we have:

$$
P = \frac{2 q^2 a^2}{c^3}
$$
Where $q$ is the charge, and $a$ is the acceleration of the charged particle. Since the power is proportional to the acceleration, which in turn is inversely proportional to the mass of the charged particle, it is easy to see that electrons are the most important particles emitting radiation, because their mass is significantly smaller than that of the rest of charged particles.

## Cyclotron  and Synchroton Frequencies

Imagine a charged particle moving in a uniform circular motion inside of an external magnetic field. From basic dynamics and kinematics, we know that the following is valid:

$$
m \omega^2 r = \frac{qvB}{c} = \frac{q \omega r B}{c}
$$

Solving for the frequency gives us they cyclotron frequency:

$$
\omega_{c} = \frac{qB}{m c}
$$

While this is pretty straightforward, it is a non-relativistic scenario, which makes it very rare in reality (only seen in high B environments). 

In the relativistic scenario, the result is pretty much the same with the corresponding lorentz factor:

$$
\omega_{syn} = \omega_c / \gamma
$$
BUT synchroton emission is affected by relativistic beaming, which makes the emission be:

$$
\nu_{syn} = \gamma^2 \omega_c = \frac{\gamma^2 q B}{m c}
$$

## Power of Synchrotron Emission

To begin with, we have to note that power $P$ is Lorentz invariant, meaning that it doesn't matter with reference frame we use to calculate it. 

In the rest frame of the charge, there is an electric field:

$$
E' = \frac{v}{c}\gamma B \approx \gamma B
$$

This electric field induces an acceleration

$$
a' = \frac{q E'}{m}
$$

The energy radiated is then given by:

$$
\frac{dE}{dt} = P = \frac{q^2}{c^3} a'^2 = \frac{q^2}{c^3} \frac{q^2 \gamma^2 B^2}{m^2} 
$$

Now, we can define the energy density of the magnetic field as $U_B = B^2/8\pi$, and use the cross-section $\sigma_T$ to get

$$
P_{syn} \sim U_B \gamma^2 c \sigma_T
$$

## Inverse Compton 

Compton scattering occurs when the energy of a photon is decreased by an ellastic collision with an electron, with the latter gaining momentum. Interestingly enough, the opposite can also happen. That is, the Inverse Compton Scattering happens when an electron collides with a photon, providing energy to such photon. 

Clearly, this is also a way in which emission of radiation can happen. The way to derive an expression for the power of IC is very similar to that of the synchrotron, but considering that the radiation field has an energy $U \sim E^2 \sim B^2$, which leaves us with the following expression:

$$
P_{IC} \sim U_\gamma \gamma^2 c \sigma_T
$$

Another way at arriving at this expresison is considering the folllowing:

$$
P_{IC} \sim (\text{rate of collisions}) \times (\text{energy per collision})
$$

Using the appropiate expressions:

$$
P_{IC} \sim \frac{U_\gamma \sigma_T c}{h\nu} \times \gamma^2 h \nu
$$

Which yields the same result as before.