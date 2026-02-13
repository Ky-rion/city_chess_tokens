

![[Pasted image 20260206202049.png]]

This is getting exciting! Now we are moving from the abstract concept of a "sphere" to a real, physical crystal structure.

In **Part (a)**, we found the general formula for the radius of the Fermi sphere:

$$k_F = (3\pi^2 n)^{1/3}$$

In **Part (b)**, our job is to find what that little $n$ (electron density) actually **is** for specific metals like Copper, Silver, or Gold (the noble metals).

Let's break down the solution step-by-step, just like we would on a blackboard.

---

### **1. Decoding the Terms**

To solve this, we need to understand two key words in the question: **"Monovalent"** and **"fcc-structure"**.

- **Monovalent:** This means "valence of one."
    
    - Each atom in the metal gives up exactly **one** electron to the free electron sea.
        
    - Therefore: **Number of Electrons ($N$) = Number of Atoms ($N_{\text{atoms}}$)**.
        
- **FCC-Structure (Face-Centered Cubic):**
    
    - Imagine a cube with side length $a$. This is our "Unit Cell."
        
    - The volume of this cube is easy: $V = a^3$.
        
    - The tricky part is counting how many atoms are inside this cube.
        

### **2. The "Magic" Number 4**

Look at Equation (1) in the solution image. It says $n = 4/a^3$.

You might ask: **"Where did the 4 come from?"**

This is the classic solid-state physics calculation of counting atoms in a unit cell. Let's count them:

1. **The Corners:** An FCC cube has 8 corners. There is an atom at every corner. However, that atom is shared by 8 adjacent cubes! So, inside _our_ specific cube, we only get $1/8$ of each corner atom.
    
    - $8 \text{ corners} \times \frac{1}{8} \text{ atom} = \mathbf{1 \text{ atom}}$
        
2. **The Faces:** An FCC cube has 6 faces (like a die). There is an atom in the center of every face. Each face atom is shared between just 2 cubes (ours and the one next to it). So we get $1/2$ of each face atom.
    
    - $6 \text{ faces} \times \frac{1}{2} \text{ atom} = \mathbf{3 \text{ atoms}}$
        

**Total Atoms in the Unit Cell:** $1 + 3 = \mathbf{4}$

Because the metal is **monovalent**, 4 atoms means we have **4 free electrons** in this volume.

### **3. Calculating the Density ($n$)**

Now we can write the formula for electron density ($n$), which is simply "stuff per volume":

$$n = \frac{N}{V} = \frac{\text{4 electrons}}{a^3}$$

This matches **Equation (1)** in your professor's solution.

### **4. The Final Substitution**

Now, we just plug this specific density back into our general formula from Part (a).

- **General Formula:**
    
    $$k_F = \sqrt[3]{3\pi^2 n}$$
    
- **Substitute $n = \frac{4}{a^3}$:**
    
    $$k_F = \sqrt[3]{3\pi^2 \cdot \frac{4}{a^3}}$$
    
- **Simplify the math ($3 \cdot 4 = 12$):**
    
    $$k_F = \sqrt[3]{\frac{12\pi^2}{a^3}}$$
    

This matches **Equation (2)** in the solution exactly.

### **Why is this cool?**

You have just derived a powerful tool! If you hand me a piece of Copper and tell me the distance between its atoms ($a$, which we can measure with X-rays), I can instantly tell you the radius of its Fermi Sphere using this formula. No other information needed!

**Ready for the next part of the question? (Or would you like to verify this for a specific metal like Copper?)**