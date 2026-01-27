

![[Pasted image 20260125185843.png]]
![[Pasted image 20260125185850.png]]

Welcome back to class! You are doing great. We have just counted how many "seats" are in the stadium (the Fermi sphere). Now, we are going to zoom in on **one specific seat** and ask: "What are the odds someone is sitting there?"

This question introduces the central engine of solid-state electronics: **The Fermi-Dirac Distribution**.

Here is the breakdown of Question 1(b).

---

### 1. Locating the "Parking Spot"

The question asks us to look at a specific state:

$$(k_F, 0, 0)_\uparrow$$

Let's decode this address:

-   **Direction:** The state is along the $k_x$ axis.
    
-   **Distance:** The distance from the center (magnitude) is $|\vec{k}| = \sqrt{k_F^2 + 0^2 + 0^2} = k_F$.
    
-   **Spin:** The little arrow $\uparrow$ just tells us we are looking at the "Spin Up" seat at this location.
    

**The Key Insight:**

Because the magnitude of this vector is exactly $k_F$, this electron sits exactly on the **surface** (the skin) of the Fermi Sphere.

Since energy $E$ is directly related to momentum $k$ (by $E \propto k^2$), if you are on the Fermi Surface ($k=k_F$), your energy is exactly the **Fermi Energy ($E_F$)**.

So, in terms of energy, this question is simply asking:

> _"What is the probability of finding an electron with Energy $E = E_F$?"_

---

### 2. The Statistical Rule: Fermi-Dirac Distribution

In the classical world (like gas molecules in a balloon), we use Boltzmann statistics. But electrons are **Fermions**, meaning they are antisocial—they hate being in the same state. They follow the **Fermi-Dirac Distribution**, which gives the probability $f(E)$ that a state at energy $E$ is occupied.

The formula is:

$$f(E) = \frac{1}{e^{\frac{E - \mu}{k_B T}} + 1}$$

-   $E$: The energy of the state we are checking.
    
-   $\mu$: The chemical potential (which the problem told us to assume is equal to the Fermi Energy, $E_F$).
    
-   $k_B$: Boltzmann constant.
    
-   $T$: Temperature.
    

---

### 3. Doing the Math

Now, we plug in the values for our specific state.

Since our state is on the surface, $E = E_F$. Also, we assume $\mu = E_F$.

$$f(E_F) = \frac{1}{e^{\frac{E_F - E_F}{k_B T}} + 1}$$

Look at the exponent:

$$\frac{E_F - E_F}{k_B T} = \frac{0}{k_B T} = 0$$

Now, evaluate the exponential term:

$$e^0 = 1$$

So the probability becomes:

$$f(E_F) = \frac{1}{1 + 1} = \frac{1}{2} = 0.5$$

**Result:** The probability is **50%**.

---

### 4. Why is it independent of Temperature?

The question asks: _"Why is the answer independent of temperature?"_

Look at the math we just did. We had $\frac{0}{k_B T}$.

As long as the temperature $T$ is not zero (which would make it undefined, $0/0$), the zero in the numerator "wins." It kills the temperature term completely.

**Visualizing the "Pivot Point"**

Look at the graph provided in your solution:

-   **The Grey Line ($T=0$):** It is a perfect step. Everything below $E_F$ is full (100%), everything above is empty (0%). At exactly the vertical line, it drops.
    
-   **The Purple/Red Lines ($T > 0$):** As you heat up the metal, electrons near the surface gain energy. Some electrons just below the surface jump to just above the surface.
    

Notice that the curve "smears out," getting softer and softer as $T$ increases. **However**, all these curves cross through exactly the same point: **$(E_F, 0.5)$**.

This is like a see-saw. As you change the temperature, the distribution tilts, but the fulcrum (the pivot point at $E_F$) never moves.

### Summary

1.  The state is exactly on the Fermi Surface, so its energy is $E_F$.
    
2.  The formula for occupation probability depends on the term $e^{(E-E_F)/k_B T}$.
    
3.  Since $E = E_F$, the exponent is 0.
    
4.  $e^0$ is always 1, regardless of what $T$ is.
    
5.  Therefore, the probability is always $1/(1+1) = 50\%$.
    

Would you like to try calculating the probability for an electron that is _slightly_ above the Fermi energy to see how temperature affects that?