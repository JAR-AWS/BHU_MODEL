There is an implementation of the Homologous Dust Collapse, a 'pressure-less' configuration that collapses under its own gravity as a test problem in the CASTRO code. The test problem uses an analytic solution that describes the radius of the sphere as a function of time, as found in Colgate and White (1966).  This problem is also found in the FLASH User's Guide and Mönchmeyer and Müller (1989).

We have modified this test problem by adding an infall velocity, which then gives us a Newtonian solution that matches approximately with the corresponding GR solution to the problem for k=0 (flat space) with zero pressure. Later, we also solve the Newtonian problem for $p \ne 0$ and try to map it to a GR solution with k $\ne 0$.

A low-density, $\rho_0$, is placed inside a sphere of radius $r_0$.  The pressure should be negligible, formally, $p_0 << 4 \pi G \rho_0^2 r_0^2 / \gamma$ (see Flash Users Guide). It is not clear what value of $p_0$ different papers use, so we use $p_0 = 1e10$ << $p_0 = 1e19$ that comes from the RHS of the inequality above.

We simulate the collapse starting from 100 times the gravitational radius and evolve until t = tc (collapse time). We use the following initial conditions:

$$\rho_0 = 2.8e8\ g/cm^3$$
 
$$r_0 = 2.39e8\ cm$$
 
$$u_0 = -2.99e9\ cm/s\ (\text{which is } 0.1c)$$
	
We find that the simulation results follow approximately the theoretical GR solution until Black Hole formation, which is marked by the radius of the cloud crossing the Schwarzschild radius (for the GR solution) and the coordinate velocity crossing the speed of light.
