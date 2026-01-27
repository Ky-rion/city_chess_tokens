

Here is a "Solid State Physics 101" cheat sheet based on this specific problem. This covers the essential formulas and logic traps you are likely to see on an exam.

### 🎓 Exam Cheat Sheet: The Free Electron Gas

#### 1. The "Parking Lot" (Geometry in k-Space)

To count electrons, we move to momentum space (k-space), where states form a grid.

-   **Fermi Wave Vector ($k_F$):** The radius of the sphere that encloses all filled states at $T=0$.
    
    $$k_F = (3\pi^2 n)^{1/3}$$
    
    _(Where $n$ is electron density)_.
    
-   **Size of One State ("Parking Spot"):** The volume occupied by a single spatial state in k-space.
    
    $$V_{state} = \left(\frac{2\pi}{L}\right)^3 = \frac{8\pi^3}{V_{real}}$$
    
    _(Where $L$ is the edge length of the sample)_.
    
-   **Counting States ($N$):** Number of unique spatial k-vectors inside the sphere.
    
    $$N = \frac{V_{sphere}}{V_{state}} = \frac{\frac{4}{3}\pi k_F^3}{(2\pi/L)^3}$$
    
-   **Counting Electrons ($N_e$):** The golden rule of spin.
    
    $$N_e = 2 \times N$$
    
    _(Because of Spin Up $\uparrow$ and Spin Down $\downarrow$, every state holds 2 electrons)_.
    

---

#### 2. The "Traffic Rules" (Energy & Statistics)

How likely is a specific state to be full?

-   **Energy of a State:**
    
    $$E = \frac{\hbar^2 k^2}{2m}$$
    
    _(Energy scales with $k^2$)_.
    
-   **Fermi-Dirac Distribution ($f_{FD}$):** Probability a state at energy $E$ is **occupied**.
    
    $$f_{FD}(E) = \frac{1}{e^{\frac{E - \mu}{k_B T}} + 1}$$
    
    _(Usually assume chemical potential $\mu \approx E_F$)_.
    
-   **The "Half-Full" Rule:**
    
    If a state is exactly **on the Fermi Surface** ($E = E_F$), the probability is always **50%** ($f_{FD} = 0.5$), regardless of temperature (as long as $T > 0$). This is because the exponent becomes $e^0 = 1$.
    

---

#### 3. Scattering Logic (The "Can I Move?" Check)

When an electron tries to move from state $A$ to state $B$:

-   **Pauli-Forbidden:** If state $B$ is already full.
    
-   **Allowed Probability:** The chance that state $B$ is **empty**.
    
    $$P_{allowed} = 1 - f_{FD}(E_{final})$$
    
    _(Don't forget the "1 minus"! The distribution $f_{FD}$ gives the filled chance; you need the empty chance)_.
    
-   **Calculating $\Delta E$ for Small Shifts:**
    
    If you shift $k$ by a small amount $\Delta k$, the energy change is approximately:
    
    $$\Delta E \approx \frac{\hbar^2}{2m} (2k_F \Delta k)$$
    
    _(Use this if $\Delta k \ll k_F$ to avoid messy squares)_.
    

---

**Would you like to try a "practice quiz" question using these formulas to make sure they stick?**