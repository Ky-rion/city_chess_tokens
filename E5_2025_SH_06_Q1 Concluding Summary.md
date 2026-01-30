

Here is your "Exam Survival Kit" for Nuclear Form Factors. These are the key takeaways, formulas, and mathematical tricks you should have ready to go.

### 1. General Definitions

-   **The Form Factor ($F(q)$):** A measure of the internal charge distribution of a particle. It is essentially the **Fourier Transform** of the charge density $\rho(r)$.
    
    $$F(\vec{q}) = \frac{1}{Ze} \int \rho(\vec{r}) e^{i\vec{q}\cdot\vec{r}/\hbar} dV$$
    
-   **Normalization:** We divide by $Ze$ so that $F(0) = 1$. This means at zero momentum transfer (no scattering), the probability is 100%.
    

### 2. The Spherical Case (Crucial Calculation)

If the nucleus is a sphere (depends only on $r$), the 3D integral simplifies to a 1D integral. You don't need to re-derive this every time, but remember the result:

$$F(q) = \frac{4\pi\hbar}{Zeq} \int_0^\infty \rho(r) r \sin\left(\frac{qr}{\hbar}\right) dr$$

-   **Key feature:** The complex exponential $e^{i\dots}$ turns into a real sine function $\sin(\dots)$.
    

### 3. The "Low Energy" Limit ($q \to 0$)

This is the most common exam question topic. If the electron hits the nucleus softly (small $q$), we can approximate $F(q)$ using a Taylor series.

$$F(q) \approx 1 - \frac{q^2 \langle r^2 \rangle}{6\hbar^2}$$

-   **$\langle r^2 \rangle$**: The "Mean Square Radius" (the physical size of the nucleus).
    

### 4. The "Master Formula" for Radius

This relates the **slope** of the form factor graph to the **size** of the nucleus.

$$\langle r^2 \rangle = -6\hbar^2 \left. \frac{dF}{d(q^2)} \right|_{q=0}$$

-   **Physical Meaning:** A steeper slope at $q=0$ means a larger nucleus (larger $\langle r^2 \rangle$).
    
-   **Note on derivative:** The derivative is with respect to $q^2$, not $q$.
    

### 5. Special Case: Gaussian Distribution

If the charge distribution is a Gaussian, the Form Factor is also a Gaussian.

-   **Form Factor:** $F(q) = \exp\left(-\frac{q^2}{2a^2\hbar^2}\right)$
    
-   **Radius:** $\langle r^2 \rangle = \frac{3}{a^2}$
    

### 6. Mathematical "Toolbox" (Tricks needed for derivation)

If you are asked to derive these from scratch, these are the tools you need:

1.  **Coordinate System:** Use Spherical Coordinates ($dV = r^2 \sin\theta dr d\theta d\phi$).
    
2.  **Alignment:** Align the $z$-axis with $\vec{q}$ so $\vec{q}\cdot\vec{r} = qr\cos\theta$.
    
3.  **Substitution:** Use $u = \cos\theta$ to solve the angular integral.
    
4.  **Taylor Expansion:** $\sin(x) \approx x - x^3/6$ is the key to finding the radius.
    

Good luck with your studies! You now have the full picture of how we measure the size of the atomic nucleus.