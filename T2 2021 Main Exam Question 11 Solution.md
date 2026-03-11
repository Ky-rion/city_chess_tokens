

Welcome back to the theoretical physics toolkit! This is a fantastic problem because it forms the bridge between basic quantum mechanics and solid-state physics. The Hamiltonian $\hat{H} = 1 - \cos p$ is incredibly common when modeling how electrons move through the periodic atomic lattice of a crystal (often called the tight-binding model).

Let's start by translating the German text into English so we can dissect the physics:

> **Given the Hamiltonian of a particle in one dimension and in momentum representation:**
> 
> $$\hat{H} = 1 - \cos p$$
> 
> **Consider a wave packet with momenta in a small neighborhood of $p_0 = \pi/4$:**
> 
> $$\tilde{\Psi}(p) = \frac{1}{\text{Norm}} \begin{cases} 1 - \left(\frac{p-p_0}{\epsilon}\right)^2 & \text{for } |p - p_0| < \epsilon \\ 0 & \text{otherwise} \end{cases}$$
> 
> **1. Expand $\hat{H}$ in a Taylor series up to order $\mathcal{O}((p - p_0)^2)$ in a small neighborhood of $p_0$.**
> 
> **2. What is the effective mass of the particle in this approximation?**
> 
> **3. What is the approximate velocity with which the wave packet as a whole moves in position space?**
> 
> _Hint: Use the formulas given in V12._

_Note: The presence of $p$ inside a cosine function implies we are using natural units where the reduced Planck constant $\hbar = 1$ and the lattice spacing $a = 1$. We will use these units throughout!_

---

### Part 1: Taylor Expansion of the Hamiltonian

**The Physics:** We have a wave packet sharply peaked around a specific momentum $p_0 = \pi/4$ (since $\epsilon$ is small). Because the momentum only has significant probability very close to $p_0$, we don't need the exact, complicated Hamiltonian for all possible momenta. We can approximate it locally using a Taylor series.

The Taylor series for a function $H(p)$ around a point $p_0$ up to second order is:

$$H(p) \approx H(p_0) + H'(p_0)(p - p_0) + \frac{1}{2}H''(p_0)(p - p_0)^2$$

Let's calculate the required pieces for $H(p) = 1 - \cos p$ at $p_0 = \pi/4$:

- **The 0th order (Value):**
    
    $$H(\pi/4) = 1 - \cos(\pi/4) = 1 - \frac{1}{\sqrt{2}}$$
    
- **The 1st order (First Derivative):**
    
    $$H'(p) = \sin p \implies H'(\pi/4) = \sin(\pi/4) = \frac{1}{\sqrt{2}}$$
    
- **The 2nd order (Second Derivative):**
    
    $$H''(p) = \cos p \implies H''(\pi/4) = \cos(\pi/4) = \frac{1}{\sqrt{2}}$$
    

Now, we just assemble the pieces into our Taylor series formula:

$$H(p) \approx \left(1 - \frac{1}{\sqrt{2}}\right) + \frac{1}{\sqrt{2}}(p - p_0) + \frac{1}{2\sqrt{2}}(p - p_0)^2$$

---

### Part 2: The Effective Mass ($m^*$)

**The Physics:** In a vacuum, the kinetic energy of a particle is strictly $E = p^2 / 2m$. If you take the second derivative of this energy with respect to momentum, you get $d^2E/dp^2 = 1/m$.

When a particle moves through a crystal lattice, the periodic potential alters its energy-momentum relationship (dispersion relation). Physicists cleverly bundle all these complicated lattice interactions into a single parameter called the **effective mass** ($m^*$), defined by the curvature of the energy band:

$$\frac{1}{m^*} = \frac{d^2E}{dp^2}\bigg|_{p_0}$$

Because our Hamiltonian _is_ the energy function $E(p)$, we can use the second derivative we just calculated in Part 1!

$$\frac{1}{m^*} = H''(\pi/4) = \frac{1}{\sqrt{2}}$$

Inverting this gives us the effective mass:

$$m^* = \sqrt{2}$$

_Insight: The effective mass is completely determined by the curvature of the Hamiltonian at the peak momentum of the wave packet!_

---

### Part 3: The Velocity of the Wave Packet

**The Physics:** A quantum wave packet is a "bundle" of many different plane waves (different momenta) superimposed on each other. There are two distinct velocities to think about:

1. **Phase velocity ($v_p$):** How fast the individual ripples inside the envelope move.
    
2. **Group velocity ($v_g$):** How fast the overall "envelope" or "packet" itself moves through space.
    

The question asks for the velocity of the wave packet _as a whole_, which is the group velocity. In classical mechanics, $v = p/m$. In quantum mechanics (with $\hbar = 1$), the group velocity is given by the first derivative of the energy with respect to momentum:

$$v_g = \frac{\partial E}{\partial p}\bigg|_{p_0}$$

Again, our Hamiltonian represents the energy $E(p)$, so we look right back at the first derivative we found in Part 1:

$$v_g = H'(\pi/4) = \frac{1}{\sqrt{2}}$$

Therefore, the wave packet moves through position space with an approximate velocity of $\frac{1}{\sqrt{2}}$.

---

### Summary for your Exam

Here is a concise way to structure your answers for grading:

- **1. Taylor Expansion:** $H(p) \approx (1 - \frac{1}{\sqrt{2}}) + \frac{1}{\sqrt{2}}(p - \pi/4) + \frac{1}{2\sqrt{2}}(p - \pi/4)^2$
    
- **2. Effective Mass:** The effective mass is defined as $m^* = (\partial^2 H / \partial p^2)^{-1}$ evaluated at $p_0$. Since $H''(p_0) = 1/\sqrt{2}$, the effective mass is $m^* = \sqrt{2}$.
    
- **3. Group Velocity:** The wave packet moves at the group velocity, given by the first derivative $v_g = \partial H / \partial p$ evaluated at $p_0$. Therefore, the velocity is $v_g = 1/\sqrt{2}$.
    

You tackled this brilliantly. Would you like me to explain the physical difference between group velocity and phase velocity in more detail, perhaps showing what happens when they are not equal (a phenomenon called dispersion)?