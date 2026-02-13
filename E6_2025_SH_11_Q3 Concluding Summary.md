

Here is your "Cheat Sheet" summary specifically for **Question 3: Group Velocity & Transport**. This covers the derivatives, direction comparisons, and physical interpretation.

### **Topic 4: Group Velocity ($\vec{v}_g$)**

- **The Golden Rule:** Velocity is the gradient (slope) of the energy band.
    
    $$\vec{v}_g(\vec{k}) = \frac{1}{\hbar} \nabla_{\vec{k}} E(\vec{k})$$
    
- **The Calculation (Square Lattice):**
    
    - **Energy:** $E = -t[\cos(k_x a) + \cos(k_y a) - 2]$
        
    - **Derivative:** $\frac{d}{dk} \cos(ka) = -a \sin(ka)$.
        
    - **Result Vector:**
        
        $$\vec{v}_g = \frac{ta}{\hbar} \begin{pmatrix} \sin(k_x a) \\ \sin(k_y a) \end{pmatrix}$$
        

---

### **Directional Comparison ([10] vs [11])**

|**Feature**|**[10] Direction (Along Axis)**|**[11] Direction (Diagonal)**|
|---|---|---|
|**Constraint**|$k_y = 0$|$k_x = k_y$|
|**Velocity Magnitude**|$|\vec{v}|
|**Max Speed Location**|$k_x = \frac{\pi}{2a}$ (Middle of path)|$k_x = \frac{\pi}{2a}$ (Middle of path)|
|**Max Speed Value**|$v_{max} = \frac{ta}{\hbar}$|$v_{max} = \mathbf{\sqrt{2}} \frac{ta}{\hbar}$|

- **Comparison Result:** The maximum velocity is **$\sqrt{2}$ times larger** along the diagonal ([11]) than along the axes ([10]).
    

---

### **Physical Interpretation (The "Why it Matters")**

- **Anisotropy:** The velocity depends on the direction of travel.
    
- **Current Density ($J$):**
    
    $$J = -e \sum_k v_g(k) f(E)$$
    
    - Since $v_g$ is anisotropic, the current $J$ (and thus conductivity $\sigma$) is also **anisotropic**.
        
    - **Takeaway:** The crystal conducts electricity better along the diagonal than along the lattice axes.
        

---

### **Exam Strategy Tips for Q3**

1. **Don't forget the $\hbar$:** It's easy to drop the $1/\hbar$ in the velocity formula.
    
2. **Chain Rule:** Remember that the derivative of $\cos(kx \cdot a)$ pulls out an extra factor of **$a$**. This is where the unit dimensions come from.
    
3. **Vector Magnitude:** When calculating $|v|$ for the diagonal, remember $\sqrt{x^2 + x^2} = \sqrt{2x^2} = x\sqrt{2}$. That's where the factor $\sqrt{2}$ comes from.
    

You are all set! You now have a complete set of notes for the Geometry, the Energy Bands, and the Transport properties. Good luck with the exam!