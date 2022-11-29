Return to [[Overview]]

## Questions:

- Relativistic motion
- Beaming
- Apparent superluminal motion
- 2 jets, one brighter than the other
- Angle $\theta$
- Doppler boost

## Relativistic motion

Bulk motion (that is, a united motion of a large quantity of matter as opposed to a single particle's motion) can be relativistic in certain astrophysical scenarios (as seen in blazars, quasars, gamma-ray bursts, etc.) This relativistic motion of macroscopic amounts of matter can produce apparent superluminal motions and the creation of beaming.

## Apparent Superluminal Motion.

Some high-energy objects (such as accreting BHs) usually show jets of mass being ejected at a speed similar to the escape velocity of the system. In some cases, if the central mass is a BH or a neutron star, this speeds can be relativistic, which can create an optical illusion of superluminal motion.

Consider the set up found in *page 6 of Lecture 6*, where the distance between the observer and the source is $d$, and an ejected particle moves from point $O$ at $t_0 = 0$ to a point $A$ at time $t_1$ with a velocity $v$. Notice there is an angle $\theta$ between the line of sight and the trajectory of the ejected particle. 

Now, we can calculate the time it takes for light to travel from both $O$ and $A$ to the observer:

$$
t_O = \frac{d}{c}
$$

$$
t_A = \frac{d-vt_1 cos\theta}{c}
$$


Furthermore, consider the transverse motion as seen from the observer $\Delta y$, which we know has to be:

$$
\Delta y = vt_1sin\theta
$$

However, the time over which the observer sees the particle move throgh such transverse displacement is:

$$
\Delta t = t_1 + t_A - t_O = t_1(1-\beta cos \theta)
$$

Where $\beta = v/c$. Therefore, the apparent transverse speed from the observer's point of view is:

$$
\frac{\Delta y}{c} = \frac{\Delta y}{\Delta t} \frac{1}{c} = \frac{vt_1sin\theta}{ct_1(1-\beta cos\theta)}
$$

Simplifying gives us:

$$
\beta_{t,app} = \frac{\beta sin \theta}{1 - \beta cos \theta}
$$

We can find the max of this function by taking the derivative with respect to $\theta$. By doing so, we realize that:

$$
\beta_{t,app,max} = \gamma \beta
$$

Which means that relativistic motion close to line of sight can produce high apparent transverse speeds that may be percieved as super luminal.

## Relativistic Beaming

The relativistic bulk motion tends to create beaming of radiation. This mainly happens due to the difference between lab frame and the moving frame. Using Lorentz Transfroms, we can find that the angle as observed in the lab frame $\theta$ is:

$$
cos\theta = \frac{\beta + cos\theta'}{1 + \beta cos \theta'}
$$

If we assume that in the moving frame, radiation has to be isotropic, then half of the photons would be radiated with an angle $\theta' < \pi/2$ and the other half with an angle $\theta' > \pi/2$. 

However, if $\gamma >>1$, we can use our relationship between the primed and the normal angle and find that what looks like an isotropic emission in the moving frame becomes a beamed emission into a cone with a half angle that is given by:

$$
\theta \sim \frac{1}{\gamma}
$$

Another consequence of beaming is that jets are usually paired, meaning that an object with ejecting matter will present two jets. Observations indicate that the approaching jet is always brighter than the receding one, and that can also be explained because of relativistic beaming.

### Doppler Boost

Lastly, the frequency of the light emitted within a relativistic flow also gets a Doppler boost, which we can find using time dilation:

$$
\nu_{obs} = \frac{\nu_{rest}}{\gamma (1-\beta cos \theta)} = \delta \nu_{rest}
$$

Where $\delta$ is the Doppler factor. We can find $\delta$ in terms of $\gamma$ by Taylor expanding $cos\theta$ and dropping high order terms and using the relationship between $\theta$ and $\gamma$. This yields:

$$
\delta \sim \gamma
$$

This is a good rule of thumb *Jets with a high Lorentz factor $\gamma$ produce an observed Doppler factor $\sim \gamma$*.