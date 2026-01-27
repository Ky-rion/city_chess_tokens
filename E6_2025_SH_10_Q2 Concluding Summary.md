

Here is your "Exam Survival" Cheat Sheet. It condenses everything we just covered into the essential formulas and rules you need to memorize.

### **Solid State Physics Cheat Sheet: The Nearly Free Electron Model**

#### **1. The Fundamental Formulas**

-   **Free Electron Energy Dispersion:**
    
    $$E_k = \frac{\hbar^2 k^2}{2m}$$
    
    -   _Note:_ This forms a parabola.
        
-   **Fermi Radius ($k_F$):**
    
    In this specific problem, the electron density is given by the radius:
    
    $$k_F = 1.2 \frac{\pi}{a}$$
    
    -   _Significance:_ This is your "water level." Everything below this energy is occupied.
        

---

#### **2. Brillouin Zone (BZ) Boundaries**

The "walls" of the first zone are critical. If $k_F$ is larger than the boundary, electrons spill into the next band.

-   **1D Chain & 3D Simple Cubic along [100]:**
    
    $$k_{\text{boundary}} = \pm \frac{\pi}{a}$$
    
    -   _Check:_ $1.2 \frac{\pi}{a} > 1.0 \frac{\pi}{a}$.
        
    -   _Result:_ **Metal-like behavior.** Electrons occupy the 1st Band and the bottom of the 2nd Band.
        
-   **3D Simple Cubic along [111] (Diagonal):**
    
    $$k_{\text{boundary}} = \pm \frac{\sqrt{3}\pi}{a} \approx \pm 1.73 \frac{\pi}{a}$$
    
    -   _Check:_ $1.2 \frac{\pi}{a} < 1.73 \frac{\pi}{a}$.
        
    -   _Result:_ **Insulator-like behavior (in this direction).** Electrons fit entirely inside the 1st Band. The 2nd Band is empty.
        

---

#### **3. Drawing the Zones (The "Folding" Trick)**

-   **Extended Zone Scheme:** Just draw the parabola $E = k^2$. Mark the zones with vertical lines at $n\frac{\pi}{a}$.
    
-   **Reduced Zone Scheme:** Everything must fit between $-\frac{\pi}{a}$ and $+\frac{\pi}{a}$.
    
    -   **Band 1:** The bottom of the parabola (unchanged).
        
    -   **Band 2:** The sections from the 2nd zone ($\frac{\pi}{a}$ to $\frac{2\pi}{a}$) are shifted by $\frac{2\pi}{a}$ towards the center. They form a "cup" shape sitting on top of Band 1.
        

---

#### **4. Adding a Periodic Potential (The "Real" Crystal)**

When the lattice potential is turned on (Part c), three things happen at the Zone Boundaries ($k = \pm \pi/a$):

1.  **Energy Splitting (The Gap):** The single energy point splits into two. One moves up, one moves down. The space between is the "Forbidden Zone" or Band Gap ($E_g$).
    
2.  **Zero Slope:** The curve must become horizontal (flat) as it touches the boundary.
    
    $$\frac{dE}{dk} = 0 \quad \text{at } k = \pm \frac{\pi}{a}$$
    
    -   _Physical Reason:_ Standing waves have zero group velocity.
        
3.  **Orthogonal Intersection:** Surfaces of constant energy must intersect the zone boundaries at right angles ($90^{\circ}$).
    

---

### **Professor's Exam "Pro-Tip"**

If you are asked to sketch these plots in an exam:

1.  **Draw the empty box first:** Mark your $x$-axis from $-\pi/a$ to $+\pi/a$.
    
2.  **Draw the vertical dashed lines** for the boundaries.
    
3.  **For "Free Electrons":** Draw sharp cusps where the bands meet.
    
4.  **For "Periodic Potential":** Erase the sharp cusps. Draw a gap. Make the lines curve smoothly into the boundary so they are flat.
    

Good luck! You now have the tools to solve 1D and 3D electron gas problems. Would you like to try a practice calculation to see if you can derive the band width?