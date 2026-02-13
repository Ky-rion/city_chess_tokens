

Here is a concise **"Solid State Physics Cheat Sheet"** based on this specific problem set. You can copy this directly onto your exam reference sheet.

### **1. The Fermi Sphere (General)**

- **Concept:** A sphere in reciprocal space containing all occupied electron states at $T=0$.
    
- **Radius ($k_F$):**
    
    $$k_F = (3\pi^2 n)^{1/3}$$
    
    - **Where:** $n = \frac{N}{V}$ is the electron density.
        
    - **Unit:** $m^{-1}$.
        
- **Derivation Logic:**
    
    $$N = 2 \times \frac{V_{\text{sphere}}}{V_{\text{state}}} = 2 \cdot \frac{\frac{4}{3}\pi k_F^3}{(2\pi)^3/V}$$
    

---

### **2. Crystal Structure (FCC Metal)**

- **Monovalent Assumption:** 1 free electron per atom.
    
- **Real Space (FCC):**
    
    - Unit Cell Volume: $V = a^3$.
        
    - Atoms per Cell: $4$ (Corners contribute $8 \times 1/8$, Faces contribute $6 \times 1/2$).
        
    - **Electron Density ($n$):**
        
        $$n = \frac{4}{a^3}$$
        
- **Resulting Fermi Radius ($k_F$):**
    
    $$k_F = \sqrt[3]{\frac{12\pi^2}{a^3}} = \frac{1}{a}(12\pi^2)^{1/3}$$
    

---

### **3. Reciprocal Space Geometry**

- **Lattice Transformation:**
    
    - Real Space: **FCC** $\rightarrow$ Reciprocal Space: **BCC**.
        
    - Reciprocal Cube Side: $A_{rec} = \frac{4\pi}{a}$.
        
- **Brillouin Zone Boundary (L-Point):**
    
    - Direction: Along the space diagonal $[111]$.
        
    - Distance $\Gamma \rightarrow L$ (Center to Face):
        
        $$\Gamma L = \frac{\sqrt{3}\pi}{a}$$
        
    - _Tip:_ This is exactly $1/4$ of the full BCC body diagonal ($\frac{4\pi}{a}\sqrt{3}$).
        

---

### **4. Does it Fit? (The Ratio Test)**

- To check if electrons touch the zone boundary, compare $k_F$ to $\Gamma L$.
    
    $$\frac{k_F}{\Gamma L} = \frac{(12\pi^2)^{1/3}}{\sqrt{3}\pi} \approx 0.90$$
    
- **Condition:** Since $0.90 < 1$, the sphere **fits inside** the first Brillouin Zone for noble metals (assuming free electron model).
    

---

### **5. Physical Interpretation (Qualitative)**

- **Curvature of Surface:**
    
    - High Curvature $\rightarrow$ **Small Effective Mass** ($m^*$) $\rightarrow$ High Mobility.
        
    - Flat Surface $\rightarrow$ **Large Effective Mass** ($m^*$) $\rightarrow$ Low Mobility.
        
- **Shape Complexity:**
    
    - Sphere $\rightarrow$ Isotropic (properties same in all directions).
        
    - Distorted $\rightarrow$ Anisotropic.
        
    - Large Surface Area $\rightarrow$ High Density of States ($DOS$) near $E_F$ $\rightarrow$ High Reactivity/Specific Heat.
        
- **Modifying the Surface:**
    
    - **Doping:** Changes $E_F$ (pumps the balloon up/down) $\rightarrow$ Major change.
        
    - **Pressure:** Changes $a$ and band structure $\rightarrow$ Distorts shape.
        
    - **Temperature:** Blurs/softens the surface edge (does not change the shape much).
        

Good luck with your exam! You have the math and the physics down solid now.