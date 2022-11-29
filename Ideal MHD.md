Return to [[Overview]]

Lecture 3

## MHD
To begin, we define MHD as the dynamics of electrically conducting fluids in the prescence of magnetic fields. This is of great application in astrophysics, since a lot of scenarios include ionized gases or plasmas submerged in magnetic fields.

As a refresher, here are Maxwell's equations:

$$
\nabla \cdot E = 4 \pi \rho_e
$$
$$
\nabla \times E = - \frac{1}{c} \frac{dB}{dt}
$$
$$
\nabla \cdot B = 0
$$
$$
\nabla \times B = \frac{4 \pi}{c} j_e + \frac{1}{c}\frac{dE}{dt}
$$

## Assumptions of Ideal MHD 
There are some further assumptions that we can make to model some astrophysical phenomena. We start with:

$$
\nabla \times B \approx \frac{4 \pi}{c} j_e 
$$

Dropping the second term since there are no large scale electric fields (any E would cause movement of charges that would quickly cancel it out). Thus, we can say that magentic fields are only caused by electric currents. Now our issue involves finding out how large drift velocities (velocities of the charged particles) need to be in order to create magnetic fields that are significant. For that, simply consider:

$$
j_e = Zen_+u_+ - en_-u_-
$$
Given that the overall charge must be neutral ($Zen_+ = en_-$), we can simplify our expression to:

$$
j_e = en_-(u_+-u_-) = en_-\Delta u
$$

Using values for the solar convection zone, we get $\Delta u \sim 10^{-12} \hspace{0.2cm} cm \hspace{0.2cm} s^{-1}$, meaning that drift velocities need not to be too large to cause signficant magnetic fields. 

Now, actually calculating $j_e$ amounts to deriving Ohm's law for this problem. For that, consider that the net force in the rest frame of the ions we have:

$$
m\frac{dv'}{dt} = -e\bigg( E' +\frac{v'}{c}\times B' \bigg) - m\nu v'+ F_g + F_I
$$

Where the first term is the electric and magnetic forces, the second term is the transfer of momentum due to collisions between ions and electrons, the third term is the gravitational force and the last term is the intertial force, since this is potentially a non-inertial frame of reference. 

Here is where more assumptions are found. First, we can assume that the second term in parenthesis is equal to zero because there aren't small-scale structures within the magnetic field. Next, we can assume that the gravitational force and inertial are negligible in this case. Assuming no change in momentum, this yields:

$$
-eE' -m_e\nu v' = 0 
$$

Therefore, the terminal velocity is

$$
v' = -\frac{eE'}{m_e\nu}
$$
Given Ohm's Law $j_e = \sigma E$, and using that in this new frame of reference $j_e' = -en_ev'$, we can conclude that

$$
\sigma = \frac{n_ee^2}{m_e \nu}
$$

Using transformations to go back to the lab's reference frame and Maxwell's fourth law, we get:

$$
E = \frac{c}{4\pi \sigma} \nabla\times B - \frac{u_i}{c} \times B
$$

We can use this expression for the electric field and plug it into Maxwell's second Law and get:

$$
\nabla \times \bigg( \frac{c}{4\pi \sigma} \nabla\times B - \frac{u_i}{c} \times B \bigg) = - \frac{1}{c} \frac{dB}{dt}
$$

Which is equivalent to

$$
\frac{dB}{dt} + \nabla \times (B \times u_i) = - \nabla \times (\eta \nabla \times B) 
$$

Where $\eta$ is the electrical resistivity. 

## Flux Freezing Equation

As we had said, one of our assumptions is that collisions between charged particles are rare. If you look closely at the derivation in the previous section, the electrical resistivity $\eta \propto \nu$, where $\nu$ is the frequency of collisions. This means that we can approximate the electric resistivity to 0, which simplifies our expression and gives us the *Flux Freezing Equation*:

$$
\frac{dB}{dt} +\nabla \times (B \times v) = 0
$$

To see why it recieves that name, consider a magnetic flux through a surface:

$$
\Phi_B = \int B \cdot dS
$$

Taking the derivative with respect to time and manipulating the expression gives us

$$
\frac{d \Phi_B}{dt} = \int_S\frac{dB}{dt} + \nabla \times (B \times v) \hspace{0.2 cm} dS = 0
$$

## Charge separation

