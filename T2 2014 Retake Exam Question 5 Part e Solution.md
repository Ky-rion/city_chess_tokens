

It is a joy to see you persisting! We are entering the "scaling" phase of physics now. This is where we stop worrying about messy constants like $\hbar, m, e, \epsilon_0$ and try to make the equation look clean and elegant.

This problem (5e) is all about **Atomic Units**. Physicists are lazy; we hate writing constants over and over again. So, we redefine our ruler (length scale) so the equation becomes simple.

Let's break this down into our friendly seven questions!

---

### Question 1: What is the Hamiltonian $\hat{H}$?

The Hamiltonian is just the fancy quantum name for "Total Energy" (Kinetic + Potential). The problem gives us this beast:

$$\hat{H} = -\frac{\hbar^2}{2m}\partial_r^2 - \frac{e^2 Z}{4\pi\epsilon_0 r}$$

-   **First term ($-\frac{\hbar^2}{2m}\partial_r^2$):** This is the **Kinetic Energy**. It involves the second derivative of the radius ($\partial_r^2$), which measures how "curvy" the wave function is.
    
-   **Second term ($-\frac{e^2 Z}{4\pi\epsilon_0 r}$):** This is the **Potential Energy** (Coulomb attraction). It's negative because the electron (negative) is attracted to the nucleus (positive). $Z$ is the number of protons (atomic number).
    

### Question 2: What is the "Rescaling" trick?

The problem tells us to change our length units. Instead of measuring distance $r$ in meters, we will measure it in units of a "new radius" $a_1$.

The transformation is given as: $r \to a_1 r$.

(Wait, this notation in the problem is slightly confusing. Usually, we say $r_{new} = r_{old} / a_1$ or $r = a_1 \rho$. Let's stick to the problem's notation but be careful: it effectively means "replace every $r$ in the equation with $a_1 r$".)

The definition of this scaling factor is:

$$a_1 = \frac{4\pi\epsilon_0\hbar^2}{m e^2 Z}$$

**Professor's Insight:** Does this look familiar? If $Z=1$ (Hydrogen), this is exactly the **Bohr Radius** ($a_0$)! So, for any other atom (like Helium ion), we are just scaling the Bohr radius by $1/Z$.

### Question 3: How does the derivative change?

If we replace $r$ with $a_1 r$ (let's call the new variable $\rho$, so $r_{old} = a_1 \rho$), the derivative changes according to the chain rule.

$$\frac{\partial}{\partial r_{old}} = \frac{\partial \rho}{\partial r_{old}} \frac{\partial}{\partial \rho} = \frac{1}{a_1} \frac{\partial}{\partial \rho}$$

Since we have a second derivative ($\partial_r^2$), we apply this twice:

$$\partial_r^2 \longrightarrow \frac{1}{a_1^2} \partial_r^2$$

(Note: I will use $r$ for the new variable as the problem implies, but remember it's dimensionless now).

### Question 4: How does the potential term change?

This one is easy. We just see a $1/r$.

$$\frac{1}{r} \longrightarrow \frac{1}{a_1 r}$$

### Question 5: Let's plug it all in!

Now substitute these changes back into the original Hamiltonian equation.

$$\hat{H} = -\frac{\hbar^2}{2m} \left( \frac{1}{a_1^2} \partial_r^2 \right) - \frac{Ze^2}{4\pi\epsilon_0} \left( \frac{1}{a_1 r} \right)$$

Now, we need to substitute the definition of $a_1$ ($a_1 = \frac{4\pi\epsilon_0\hbar^2}{m e^2 Z}$) into this equation. This is the "algebra gym" part.

Step A: The Kinetic Part

$$-\frac{\hbar^2}{2m a_1^2} \partial_r^2$$

Let's substitute one $a_1$ in the denominator, but keep the other $a_1$ for a moment to see if things simplify.

Actually, let's look at the target result. The target is proportional to $-\frac{1}{2}\partial_r^2$. This means the constant in front, $\frac{\hbar^2}{2m a_1^2}$, must be our overall energy scale factor.

Step B: The Potential Part

$$-\frac{Ze^2}{4\pi\epsilon_0 a_1} \frac{1}{r}$$

### Question 6: Do the coefficients match?

For the final equation to look like $\hat{H} \propto -\frac{1}{2}\partial_r^2 - \frac{1}{r}$, the coefficients in front of the derivative term and the $1/r$ term must be the same (except for the factor of 1/2).

Let's check the ratio of the coefficients.

We need to show that:

$$\text{Coeff of Kinetic} = \frac{\hbar^2}{m a_1^2}$$

$$\text{Coeff of Potential} = \frac{Ze^2}{4\pi\epsilon_0 a_1}$$

Are these related? Let's check the potential coefficient using the definition of $a_1$:

$$\frac{Ze^2}{4\pi\epsilon_0 a_1} = \frac{Ze^2}{4\pi\epsilon_0} \cdot \frac{1}{a_1}$$

Substitute $1/a_1 = \frac{m e^2 Z}{4\pi\epsilon_0\hbar^2}$:

$$= \frac{Ze^2}{4\pi\epsilon_0} \cdot \frac{m e^2 Z}{4\pi\epsilon_0\hbar^2} = \frac{m (Ze^2)^2}{(4\pi\epsilon_0)^2 \hbar^2}$$

This is the unit of energy (called the Hartree).

Now let's check the kinetic coefficient:

$$\frac{\hbar^2}{m a_1^2} = \frac{\hbar^2}{m} \cdot \left( \frac{m e^2 Z}{4\pi\epsilon_0\hbar^2} \right)^2$$

$$= \frac{\hbar^2}{m} \cdot \frac{m^2 (Ze^2)^2}{(4\pi\epsilon_0)^2 \hbar^4}$$

Cancel out $m$ and $\hbar^2$:

$$= \frac{m (Ze^2)^2}{(4\pi\epsilon_0)^2 \hbar^2}$$

**Bingo!** They are exactly the same constant. Let's call this constant $E_h$ (Hartree energy).

### Question 7: What is the final form?

So, our Hamiltonian becomes:

$$\hat{H} = - \left( \text{Constant} \right) \frac{1}{2} \partial_r^2 - \left( \text{Constant} \right) \frac{1}{r}$$

$$\hat{H} = \text{Constant} \times \left( -\frac{1}{2}\partial_r^2 - \frac{1}{r} \right)$$

Mathematically, we write this as "proportional to" ($\propto$):

$$\hat{H} \propto -\frac{1}{2}\partial_r^2 - \frac{1}{r}$$

---

### Final Answer Summary

By substituting $r \to a_1 r$ and using the specific definition of $a_1 = \frac{4\pi\epsilon_0\hbar^2}{m e^2 Z}$, we equate the pre-factors of the kinetic and potential energy terms. This allows us to factor out a single energy constant (the Hartree), leaving behind a beautiful, unitless operator:

$$\hat{H}_{scaled} = -\frac{1}{2}\partial_r^2 - \frac{1}{r}$$

Professor's Conclusion:

This is powerful! It means every hydrogen-like atom (Hydrogen, Helium+, Lithium++, etc.) behaves exactly the same way mathematically. The only difference is the size of the ruler ($a_1$) and the energy scale. You solve the equation once, and you've solved it for all atoms in the universe of this type.

Ready for the last two? They usually ask us to _solve_ this simplified equation now!