

Here is a summary cheat sheet tailored for this specific type of problem. It separates the **General Rules** (always true for spherical nuclei) from the **Specific Tricks** (needed for Gaussian distributions).

---

# 🎓 Particle Physics Cheat Sheet: Nuclear Radii

### 1. General Definitions (Always True)

-   **Charge Density:** $\rho(r) = Z \cdot e \cdot f(r)$
    
    -   $f(r)$ is the "shape function" (probability density).
        
    -   Normalization condition: $\int f(r) dV = 1$ (The total probability is 100%).
        
-   **Mean Squared Radius Definition:**
    
    $$\langle r^2 \rangle = \iiint r^2 f(r) \, dx \, dy \, dz$$
    

### 2. Spherical Coordinates Integration

-   **The Volume Element (Crucial!):**
    
    $$dV = r^2 \sin(\theta) \, dr \, d\theta \, d\phi$$
    
-   **Integration Limits:**
    
    -   $r \rightarrow 0 \text{ to } \infty$
        
    -   $\theta \rightarrow 0 \text{ to } \pi$
        
    -   $\phi \rightarrow 0 \text{ to } 2\pi$
        
-   **Simplified Formula for Spherically Symmetric Nuclei:**
    
    If the problem says "spherically symmetric," you can do the angular integrals immediately ($4\pi$) and use this shortcut:
    
    $$\langle r^2 \rangle = 4\pi \int_0^\infty r^4 f(r) \, dr$$
    
    -   _Note:_ It is $r^4$ because you have $r^2$ from the radius definition $\times$ $r^2$ from the volume element.
        

---

### 3. Gaussian Distribution Specifics (For Part B)

If given a Gaussian shape $f(r) \sim \exp(-br^2)$:

-   **The "Gaussian Integral" Trick:**
    
    Do not integrate by hand. Use the Gamma function identity:
    
    $$\int_0^\infty x^n \exp(-bx^2) \, dx = \frac{\Gamma\left( \frac{n+1}{2} \right)}{2 b^{\left( \frac{n+1}{2} \right)}}$$
    
-   **Key Gamma Values:**
    
    -   $\Gamma(1/2) = \sqrt{\pi}$
        
    -   $\Gamma(n+1) = n \cdot \Gamma(n)$
        
    -   $\Gamma(5/2) = \frac{3}{2} \cdot \frac{1}{2} \cdot \sqrt{\pi} = \frac{3\sqrt{\pi}}{4}$
        
-   **Final Result for 3D Gaussian:**
    
    For a shape defined by $a$ (width parameter):
    
    $$\langle r^2 \rangle = \frac{3}{a^2}$$
    
    -   _Interpretation:_ Larger $a$ $\rightarrow$ Smaller radius.
        

---

### ⚠️ Common Pitfalls to Avoid

1.  **Forgetting the Jacobian:** Never just write $dr \, d\theta \, d\phi$. You must include $r^2 \sin(\theta)$.
    
2.  **Confusing $n$:** In the radius calculation, the power of $r$ is usually $4$ (so $n=4$ in the integral formula), but for normalization calculations, the power is $2$ (so $n=2$).
    
3.  **Factorials:** Remember that $(2z)!$ means you calculate $2z$ first, then take the factorial. It is not $2 \times (z!)$.
    

Good luck with your studying! Would you like to try applying this cheat sheet to a different shape, like a "Hard Sphere" (constant density)?