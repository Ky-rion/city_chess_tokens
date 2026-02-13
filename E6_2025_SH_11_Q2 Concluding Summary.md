

Here is a condensed "Cheat Sheet" summary of the concepts and formulas we covered. This is designed to be quick to read and easy to copy for your exam preparation.

### **Topic 1: Reciprocal Space & Brillouin Zones (Geometry)**

- **Lattice:** Square lattice with constant $a$.
    
- **Reciprocal Lattice Vector:** The spacing in k-space is $b = \frac{2\pi}{a}$.
    
- **1st Brillouin Zone (1. BZ):**
    
    - **Shape:** Square centered at $(0,0)$.
        
    - **Boundaries:** $k_x = \pm \frac{\pi}{a}$ and $k_y = \pm \frac{\pi}{a}$.
        
    - **Key Distances from Center $(0,0)$:**
        
        - To the **Edge** (X-point): $k = \frac{\pi}{a} \approx 1.0 \frac{\pi}{a}$.
            
        - To the **Corner** (M-point): $k = \sqrt{(\frac{\pi}{a})^2 + (\frac{\pi}{a})^2} = \sqrt{2}\frac{\pi}{a} \approx 1.41 \frac{\pi}{a}$.
            

---

### **Topic 2: Free Electron Model (The "Sphere")**

- **Dispersion Relation:** $E_k = \frac{\hbar^2 k^2}{2m}$ (Parabolic, depends only on magnitude $|k|$).
    
- **Fermi Surface:** A circle (2D) or sphere (3D) with radius $k_F$.
    
- **Filling the Zones:** Compare $k_F$ to the BZ boundaries.
    
    - **If $k_F < \frac{\pi}{a}$:** The sphere fits entirely inside the 1st BZ (Insulator/Semiconductor behavior if full).
        
    - **If $\frac{\pi}{a} < k_F < 1.41 \frac{\pi}{a}$:** The sphere spills over the edges into the 2nd BZ but leaves corners of the 1st BZ empty. (This was your specific case where $k_F = 1.2 \frac{\pi}{a}$).
        
- **Reduced Zone Scheme:**
    
    - **Hole Pockets:** Empty spaces in the 1st BZ (corners).
        
    - **Electron Pockets:** Filled spaces in the 2nd BZ (mapped back to the center).
        

---

### **Topic 3: Tight-Binding Model (The "Cosine Waves")**

- **Dispersion Relation (2D Square):**
    
    $$E(\vec{k}) = -t \left[ \cos(k_x a) + \cos(k_y a) - 2 \right]$$
    
    _(Note: Sometimes the "-2" is omitted, shifting the zero-point, but the bandwidth stays the same)._
    
- **Key Locations & Energies:**
    
    - **$\Gamma$-point (Center):** $(0,0)$ $\rightarrow$ $\cos(0)=1$.
        
        - $E_{min} = -t[1+1-2] = 0$.
            
    - **X-point (Edge):** $(\frac{\pi}{a}, 0)$ $\rightarrow$ $\cos(\pi)=-1, \cos(0)=1$.
        
        - $E = -t[-1+1-2] = 2t$ (Saddle point).
            
    - **M-point (Corner):** $(\frac{\pi}{a}, \frac{\pi}{a})$ $\rightarrow$ $\cos(\pi)=-1$.
        
        - $E_{max} = -t[-1-1-2] = 4t$.
            
- **Bandwidth ($W$):**
    
    $$W = E_{max} - E_{min} = 4t$$
    
    - _Concept:_ Larger hopping $t$ $\rightarrow$ Wider bandwidth $\rightarrow$ Faster electrons (lower effective mass).
        

---

### **Exam Strategy Tips**

1. **Check the Sign:** Look at the sign in front of $t$. If it is $-t$, the minimum is at $(0,0)$ (cosine is max). If it were $+t$, the minimum would be at the corners.
    
2. **Calculate Limits First:** Before drawing any curve, calculate the energy at $(0,0)$, $(\frac{\pi}{a}, 0)$, and $(\frac{\pi}{a}, \frac{\pi}{a})$. These are your "connect-the-dots" anchors.
    
3. **"Qualitative" Drawing:** When asked to draw "qualitatively," ensure the slope is flat (derivative is zero) at the high symmetry points ($0$ and $\pi/a$). The curve should look like a smooth wave, not sharp zig-zags.
    

Good luck with your studying! You have a solid grasp of these foundations now.