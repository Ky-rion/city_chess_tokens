

Hello! Welcome to Quantum Mechanics 101. It is wonderful to have you here. I am absolutely delighted to be your guide through the fascinating world of the Hydrogen atom. Don't worry if this looks like a jumble of Greek letters and integrals right now; by the end of this, you will see the elegance hiding in the math.

We are going to solve **Problem 5a**, which asks us to calculate the **radial probability density** for the ground state of a hydrogen atom.

To make this digestible, let's break the solution down into **seven key questions** that we need to ask and answer to solve the problem.

---

### Question 1: What exactly are we looking at? (The Wave Function)

First, we need to understand the "ingredient" we are given. The problem gives us $\psi_{1,0,0}(r, \theta, \varphi)$, which is the **wave function** for the ground state of hydrogen.

$$\psi_{1,0,0}(r, \theta, \varphi) = \frac{e^{-\frac{r}{a_0}}}{\sqrt{\pi a_0^3}}$$

**Professor's Insight:** Notice something very special here? The variables $\theta$ (theta) and $\varphi$ (phi) represent angles in 3D space. However, they are **missing** from the right side of the equation! The function only depends on $r$ (distance from the nucleus) and constants ($\pi$ and the Bohr radius $a_0$).

This tells us the ground state is **spherically symmetric**. It looks the same from every angle.

### Question 2: What is the goal? (The Radial Probability Density)

The problem asks us to compute $P_{\psi_{1,0,0}}$. The problem sheet kindly gives us the definition formula:

$$P_\psi(r) := \int_0^\pi \sin \theta \, d\theta \int_0^{2\pi} d\varphi \, r^2 |\psi(r, \theta, \varphi)|^2$$

Professor's Insight:

You might ask, "Why do we need this integral?"

In quantum mechanics, $|\psi|^2$ gives us the probability density per unit volume. But we want the radial probability density—which means the probability of finding the electron at a specific distance $r$, regardless of the direction. To get that, we have to sum up (integrate) the probability over all possible angles ($\theta$ and $\varphi$).

### Question 3: How do we handle the "probability" part? (Squaring the Wave Function)

The formula requires $|\psi|^2$, which is the square of the absolute value of our wave function. Since our function is real (no imaginary numbers $i$), we can just square it normally.

$$|\psi|^2 = \left( \frac{e^{-\frac{r}{a_0}}}{\sqrt{\pi a_0^3}} \right)^2$$

When we square the numerator: $(e^{-r/a_0})^2 = e^{-2r/a_0}$.

When we square the denominator: $(\sqrt{\pi a_0^3})^2 = \pi a_0^3$.

So, our probability density is:

$$|\psi|^2 = \frac{1}{\pi a_0^3} e^{-\frac{2r}{a_0}}$$

### Question 4: How do we set up the integral?

Now, let's substitute our result from Question 3 into the main formula from Question 2.

$$P_{\psi}(r) = \int_0^\pi \sin \theta \, d\theta \int_0^{2\pi} d\varphi \, r^2 \left[ \frac{1}{\pi a_0^3} e^{-\frac{2r}{a_0}} \right]$$

This looks messy, but look closely! The term we just calculated ($\frac{1}{\pi a_0^3} e^{-2r/a_0}$) and the $r^2$ term **do not contain any angles**. They are constants as far as the integration is concerned.

### Question 5: Can we simplify the integration? (Separation of Variables)

Absolutely! Because the parts with $r$ don't depend on $\theta$ or $\varphi$, we can pull them _outside_ the integral signs. This separates the problem into an "easy angular part" and the "radial part."

$$P_{\psi}(r) = \left( r^2 \frac{1}{\pi a_0^3} e^{-\frac{2r}{a_0}} \right) \times \underbrace{ \left( \int_0^\pi \sin \theta \, d\theta \int_0^{2\pi} d\varphi \right) }_{\text{The Angular Part}}$$

### Question 6: What is the value of the "Angular Part"?

Now we just have to solve the integrals for the angles. This is a standard result in physics for anything spherically symmetric (like a ball).

1.  **The $\varphi$ integral:** $\int_0^{2\pi} d\varphi = 2\pi - 0 = 2\pi$.
    
2.  **The $\theta$ integral:** $\int_0^\pi \sin \theta \, d\theta = [-\cos \theta]_0^\pi = (-\cos \pi) - (-\cos 0) = -(-1) - (-1) = 1 + 1 = 2$.
    

So, the total angular part is just the product of these two:

$$\text{Angular Part} = 2 \times 2\pi = 4\pi$$

_(Note: This $4\pi$ represents the total solid angle of a sphere!)_

### Question 7: What is the final result?

Now we put the "Radial Part" and the "Angular Part" back together.

$$P_{\psi}(r) = \left( r^2 \frac{1}{\pi a_0^3} e^{-\frac{2r}{a_0}} \right) \cdot (4\pi)$$

Let's clean this up algebraically.

1.  Move the constants to the front: $4\pi \cdot \frac{1}{\pi a_0^3}$.
    
2.  Cancel the $\pi$ in the numerator and denominator.
    

$$P_{\psi}(r) = \frac{4}{a_0^3} r^2 e^{-\frac{2r}{a_0}}$$

---

### Final Answer

The radial probability density for the ground state of the hydrogen atom is:

$$P_{\psi_{1,0,0}}(r) = \frac{4 r^2}{a_0^3} e^{-\frac{2r}{a_0}}$$

Professor's Conclusion:

This result is fascinating! Even though the probability density $|\psi|^2$ is highest at the nucleus ($r=0$), the radial probability $P(r)$ is actually zero at the nucleus because of that $r^2$ term (the volume of the shell at $r=0$ is zero). The most likely distance to find the electron is actually at $r=a_0$, the Bohr radius.

**Would you like me to show you how to find that maximum point (taking the derivative) to prove the electron likes to hang out at the Bohr radius $a_0$?**