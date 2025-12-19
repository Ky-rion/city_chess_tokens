

You are absolutely right—these last two are "cute" little problems! They are short, but they test if you really understood the heavy lifting we did in the previous parts.

We are looking at **Problem 5f**: "How does the ground state energy scale with the nuclear charge number $Z$?"

Basically: If we swap the Hydrogen nucleus ($Z=1$) for a Helium nucleus ($Z=2$) or a Lithium nucleus ($Z=3$), how does the energy of the electron change?

Let's answer this in four quick questions.

---

### Question 1: Where is the energy hiding?

Recall what we did in **Problem 5e**. We took the complicated Hamiltonian and rewrote it as:

$$\hat{H} = \left( \text{Energy Constant} \right) \times \left[ -\frac{1}{2}\partial_\rho^2 - \frac{1}{\rho} \right]$$

That "Energy Constant" in front sets the scale for the whole system. If that constant doubles, the total energy doubles.

From our work in 5e, that constant (let's call it $E_{scale}$) was the coefficient of the potential energy term:

$$E_{scale} = \frac{Z e^2}{4\pi\epsilon_0 a_1}$$

### Question 2: How does the length $a_1$ depend on $Z$?

We also have the definition of our scaling length $a_1$ from problem 5e:

$$a_1 = \frac{4\pi\epsilon_0\hbar^2}{m e^2 \mathbf{Z}}$$

Notice where the $Z$ is? It is in the denominator.

This means:

$$a_1 \propto \frac{1}{Z}$$

**Physical Meaning:** As the nucleus gets more positively charged (higher $Z$), it pulls the electron in tighter. The atom gets _smaller_ by a factor of $1/Z$.

### Question 3: How do we combine them?

Now, let's substitute the relationship for $a_1$ (from Q2) into the energy scale (from Q1).

$$E_{scale} \propto \frac{Z}{a_1}$$

Since $a_1 \propto \frac{1}{Z}$, we get:

$$E_{scale} \propto \frac{Z}{(1/Z)}$$

$$E_{scale} \propto Z \cdot Z$$

$$E_{scale} \propto Z^2$$

### Question 4: Does this make physical sense?

Yes! Think about it:

1.  **Double whammy:** If you increase $Z$, the nucleus pulls harder on the electron (factor of $Z$).
    
2.  **Closer proximity:** Because it pulls harder, the electron moves closer (the radius decreases by $1/Z$).
    
3.  **Result:** Coulomb potential energy is $V \sim \frac{Charge}{Distance}$. If Charge goes up by $Z$ and Distance goes _down_ by $Z$, the Energy goes up by $Z \times Z = Z^2$.
    

---

### Final Answer for (5f)

The ground state energy scales with the square of the nuclear charge number:

$$E_{ground} \propto Z^2$$

_(Specifically, $E_n = -13.6 \text{ eV} \cdot \frac{Z^2}{n^2}$. So for Helium ($Z=2$), the electron is held $2^2 = 4$ times more tightly than in Hydrogen!)_

Professor's Check-in:

One last question to go! It's usually the "victory lap." Are you ready for 5g?