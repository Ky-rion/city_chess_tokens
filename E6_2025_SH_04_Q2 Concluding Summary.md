

Here is your "Exam Cheat Sheet" for X-Ray Diffraction! I have condensed everything into the essentials you need to memorize.

---

### 📄 Cheat Sheet: X-Ray Diffraction (Cubic Systems)

#### 1. Fundamental Formulas

**Bragg's Law (The "Diffraction Condition")**

Connects the X-ray wavelength to the spacing between atomic layers.

$$n\lambda = 2 d_{hkl} \sin(\theta)$$

-   **Important:** Diffractograms usually show **$2\theta$** on the x-axis. You **MUST** divide by 2 to get $\theta$ before putting it in the $\sin()$ function.
    
-   **$n$:** Diffraction order (usually assume $n=1$ unless told otherwise).
    

**Interplanar Spacing (For Cubic Crystals)**

Connects the layer spacing ($d$) to the cube size ($a$) and the plane name $(hkl)$.

$$d_{hkl} = \frac{a}{\sqrt{h^2 + k^2 + l^2}}$$

**The "Quick Check" Formula**

If you combine the two formulas above (for $n=1$), you get this relation. It is useful for quickly checking if integer indices ($h,k,l$) fit your angle:

$$\sin^2(\theta) = \frac{\lambda^2}{4a^2} (h^2 + k^2 + l^2)$$

---

#### 2. The "Fingerprint" Rules (Extinction Conditions)

This is the decision tree to identify the lattice type (sc, bcc, or fcc) based on which peaks appear.

![[Pasted image 20260126204441.png]]

**Common Peak Sequences (First few peaks you will see):**

-   **SC:** (100), (110), (111), (200), (210)... _(1, 2, 3, 4, 5, 6...)_
    
-   **BCC:** (110), (200), (211), (220)... _(Sum is even)_
    
-   **FCC:** (111), (200), (220), (311)... _(All odd or all even)_
    

---

#### 3. Step-by-Step Exam Strategy

1.  **Read the Graph:** Identify the $2\theta$ values for the peaks.
    
2.  **Convert:** Divide by 2 to get $\theta$.
    
3.  **Calculate $d$:** Use $d = \frac{\lambda}{2\sin\theta}$.
    
4.  **Find Integers:** Use $\sqrt{h^2+k^2+l^2} = \frac{a}{d}$. Square the result to find the integer sum (e.g., $\approx 2$, $\approx 4$, etc.).
    
5.  **Identify Structure:** Look at the indices you found.
    
    -   Do you have a (100)? $\rightarrow$ Likely **SC**.
        
    -   Is the first peak (110)? $\rightarrow$ Likely **BCC**.
        
    -   Is the first peak (111)? $\rightarrow$ Likely **FCC**.
        

---

#### 4. Useful Constants & Units

-   **Ångström (Å):** $1 \text{ \AA} = 10^{-10} \text{ m}$
    
-   **Nanometer (nm):** $1 \text{ nm} = 10^{-9} \text{ m}$
    
-   **Conversion:** $1 \text{ nm} = 10 \text{ \AA}$
    

Would you like me to give you a quick "practice problem" with just numbers to test if you can use this cheat sheet correctly?