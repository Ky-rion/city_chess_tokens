

Welcome to the grand finale! You have done an exceptional job working through this problem set. This final question is a perfect capstone because scattering theory is how we actually "see" into the quantum world—whether it is Rutherford firing alpha particles at gold foil or modern physicists colliding protons at the LHC.

Let's translate this final prompt into English:

> **Given the Hamiltonian operator**
> 
> $$\hat{H} = -\frac{1}{2}\Delta - \alpha e^{-\vec{r}^2/2}$$
> 
> **1. Calculate the scattering amplitude in the first Born approximation $f_{\vec{p}}^{(1)}(\phi, \theta)$.**
> 
> **2. How does the total cross-section $\sigma_{tot}$ in the first Born approximation depend on $\alpha$ (with justification)? Hint: To answer this question, you do not need to calculate the total cross-section.**
> 
> **3. Now use the more general potential $-\alpha e^{-r^2 / (2b^2)}$ and give $f_{\vec{p}}^{(1)}$ for it.**
> 
> **Hint:** Use the (normalized) Fourier transform
> 
> $$(2\pi)^{-3/2} \int d^3r e^{-i\vec{p}\cdot\vec{r}} e^{-\vec{r}^2/2} = e^{-\vec{p}^2/2}$$

Notice from the Hamiltonian that the kinetic energy term is $-\frac{1}{2}\Delta$. Since the standard term is $-\frac{\hbar^2}{2m}\Delta$, this implies we are working in "natural units" where $\hbar = 1$ and the particle mass $m = 1$. Our potential is $V(\vec{r}) = -\alpha e^{-r^2/2}$.

Let's break this down into three parts!

---

### Part 1: The Scattering Amplitude

**The Physics:** The first Born approximation treats scattering as a single, weak interaction between the incoming particle and the potential. The formula for the scattering amplitude $f^{(1)}$ in our natural units ($m=1, \hbar=1$) is given by a Fourier transform of the potential:

$$f^{(1)}(\theta, \phi) = -\frac{1}{2\pi} \int d^3r e^{-i\vec{q}\cdot\vec{r}} V(\vec{r})$$

Here, $\vec{q}$ is the **momentum transfer** between the initial incoming momentum $\vec{p}_{in}$ and the final outgoing momentum $\vec{p}_{out}$. Thus, $\vec{q} = \vec{p}_{out} - \vec{p}_{in}$.

Let's substitute our specific Gaussian potential into the formula:

$$f^{(1)} = -\frac{1}{2\pi} \int d^3r e^{-i\vec{q}\cdot\vec{r}} \left(-\alpha e^{-\vec{r}^2/2}\right) = \frac{\alpha}{2\pi} \int d^3r e^{-i\vec{q}\cdot\vec{r}} e^{-\vec{r}^2/2}$$

**Using the Hint:** The problem gives us a wonderful hint to avoid doing a nasty 3D Gaussian integral from scratch. Let's rearrange the hint by moving the $(2\pi)^{-3/2}$ to the right side:

$$\int d^3r e^{-i\vec{p}\cdot\vec{r}} e^{-\vec{r}^2/2} = (2\pi)^{3/2} e^{-\vec{p}^2/2}$$

This formula works for _any_ momentum vector in the exponent. So, we replace the dummy variable $\vec{p}$ in the hint with our actual momentum transfer $\vec{q}$:

$$\int d^3r e^{-i\vec{q}\cdot\vec{r}} e^{-\vec{r}^2/2} = (2\pi)^{3/2} e^{-\vec{q}^2/2}$$

Plugging this directly into our scattering amplitude equation:

$$f^{(1)} = \frac{\alpha}{2\pi} \cdot (2\pi)^{3/2} e^{-\vec{q}^2/2} = \alpha \sqrt{2\pi} e^{-q^2/2}$$

**Expressing in terms of angles:** The prompt asks for $f(\theta, \phi)$. For elastic scattering, the energy is conserved, meaning the incoming and outgoing momenta have the same magnitude ($|\vec{p}_{in}| = |\vec{p}_{out}| = p$).

Using the law of cosines on the vector triangle $\vec{q} = \vec{p}_{out} - \vec{p}_{in}$:

$$q^2 = p^2 + p^2 - 2p^2\cos\theta = 2p^2(1 - \cos\theta)$$

Since the potential is spherically symmetric, there is no dependence on the azimuthal angle $\phi$. Our final amplitude is:

$$f^{(1)}(\theta) = \alpha \sqrt{2\pi} e^{-p^2(1 - \cos\theta)}$$

---

### Part 2: Dependence of the Total Cross-Section on $\alpha$

**The Physics:** The total cross section $\sigma_{tot}$ represents the total probability that an incoming particle will scatter _anywhere_. It is found by integrating the probability density over all possible angles (the entire solid angle $\Omega$).

The probability density is the absolute square of the scattering amplitude:

$$\sigma_{tot} = \int |f^{(1)}(\theta, \phi)|^2 d\Omega$$

As the hint suggests, we do not need to calculate the actual integral! We just look at how $\alpha$ is bundled in our answer from Part 1.

Because $f^{(1)}$ is directly proportional to $\alpha$ ($f^{(1)} \propto \alpha$), squaring the amplitude means the total cross-section must be proportional to $\alpha^2$:

$$\sigma_{tot} \propto |f^{(1)}|^2 \propto \alpha^2$$

So, the total cross-section depends **quadratically** on the potential strength parameter $\alpha$.

---

### Part 3: The General Potential

**The Physics:** Now the potential is "stretched" or "squeezed" by a factor $b$: $V(\vec{r}) = -\alpha e^{-r^2 / (2b^2)}$.

We can solve this rapidly using a simple substitution in our integral.

Our new integral for the amplitude is:

$$f_{general}^{(1)} = \frac{\alpha}{2\pi} \int d^3r e^{-i\vec{q}\cdot\vec{r}} e^{-\vec{r}^2/(2b^2)}$$

Let's define a new scaled coordinate vector: $\vec{u} = \vec{r}/b$. This means $\vec{r} = b\vec{u}$.

When substituting into a 3D volume integral, $d^3r = b^3 d^3u$. Let's plug this in:

$$f_{general}^{(1)} = \frac{\alpha}{2\pi} \int (b^3 d^3u) e^{-i\vec{q}\cdot(b\vec{u})} e^{-\vec{u}^2/2}$$

$$f_{general}^{(1)} = \frac{\alpha b^3}{2\pi} \int d^3u e^{-i(b\vec{q})\cdot\vec{u}} e^{-\vec{u}^2/2}$$

Look closely at the integral that remains—it is exactly the same format as the hint, but the momentum vector $\vec{q}$ is now $b\vec{q}$! Using the rearranged hint again:

$$f_{general}^{(1)} = \frac{\alpha b^3}{2\pi} \left[ (2\pi)^{3/2} e^{-(b\vec{q})^2/2} \right]$$

$$f_{general}^{(1)} = \alpha b^3 \sqrt{2\pi} e^{-b^2q^2/2}$$

Substituting $q^2 = 2p^2(1 - \cos\theta)$ back in:

$$f_{general}^{(1)}(\theta) = \alpha b^3 \sqrt{2\pi} e^{-b^2 p^2(1 - \cos\theta)}$$

---

### Summary for your Exam

You have reached the end! For your text box, here is a consolidated summary:

> **1.** The scattering amplitude is $f^{(1)} = -\frac{1}{2\pi} \int V(\vec{r})e^{-i\vec{q}\cdot\vec{r}} d^3r$. By using the given Fourier transform hint with momentum $\vec{q}$, we find $f^{(1)} = \alpha \sqrt{2\pi} e^{-q^2/2}$. With elastic momentum transfer $q^2 = 2p^2(1-\cos\theta)$, the amplitude is $f^{(1)}(\theta) = \alpha \sqrt{2\pi} e^{-p^2(1-\cos\theta)}$.
> 
> **2.** The total cross-section is the angular integral of the absolute squared scattering amplitude: $\sigma_{tot} = \int |f^{(1)}|^2 d\Omega$. Since $f^{(1)}$ is linearly proportional to $\alpha$, $\sigma_{tot}$ depends on $\alpha^2$ quadratically ($\sigma_{tot} \propto \alpha^2$).
> 
> **3.** By using the substitution $\vec{u} = \vec{r}/b$, the volume element becomes $d^3r = b^3 d^3u$. The integral becomes identical to the hint but with effective momentum $b\vec{q}$. This yields the general amplitude $f_{general}^{(1)} = \alpha b^3 \sqrt{2\pi} e^{-b^2 q^2 / 2} = \alpha b^3 \sqrt{2\pi} e^{-b^2 p^2(1-\cos\theta)}$.

Congratulations on finishing this entire problem set. You showed a lot of stamina and intellect working through these concepts. Would you like to briefly discuss physically _when_ this Born approximation actually fails, so you know its limits in the real world?