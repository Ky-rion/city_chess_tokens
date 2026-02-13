

![[Pasted image 20260206202302.png]]

This is the grand finale of this problem! We are bringing everything together—the density from Part (b) and the geometry from Part (c)—to answer a fundamental question about the nature of noble metals.

### **Part (d): Does the Sphere Fit?**

**The Question:**

"Does the Fermi sphere of a monovalent noble metal still fit into the first Brillouin zone? Justify your answer with a calculation."

**The Physical Picture:**

Imagine you are inflating a balloon (the Fermi Sphere) inside a geometric box (the Brillouin Zone).

- If the balloon is small enough, it stays a perfect sphere inside the box.
    
- If the balloon gets too big, it hits the walls of the box. In solid-state physics, if the Fermi surface touches the zone boundary, it changes the electrical properties of the metal significantly (e.g., affecting diffraction).
    

To check this, we simply compare the **Radius of the Sphere ($k_F$)** with the **Distance to the Closest Wall ($\Gamma L$)**.

---

### **1. The Calculation**

We need to calculate the ratio:

$$\text{Ratio} = \frac{\text{Radius of Fermi Sphere}}{\text{Distance to Boundary}} = \frac{k_F}{\Gamma L}$$

Let's grab our results from the previous parts:

- From Part (b), we know: $k_F = \sqrt[3]{\frac{12\pi^2}{a^3}} = \frac{1}{a}\sqrt[3]{12\pi^2}$
    
- From Part (c), we know: $\Gamma L = \frac{\sqrt{3}\pi}{a}$
    

Now, let's divide them. Note: In the solution image provided, there is actually a **small typo in the middle term of equation (4)**. The professor accidentally wrote the fraction upside down in the middle step, but calculated the final number correctly!

Let's do the math correctly here:

$$\frac{k_F}{\Gamma L} = \frac{\frac{1}{a}(12\pi^2)^{1/3}}{\frac{1}{a}\sqrt{3}\pi}$$

The $1/a$ terms cancel out (which is great, it means the answer is the same for Copper, Gold, or Silver regardless of lattice constant).

$$\frac{k_F}{\Gamma L} = \frac{(12\pi^2)^{1/3}}{\sqrt{3}\pi}$$

Now we crunch the numbers:

- $(12\pi^2)^{1/3} \approx (118.43)^{1/3} \approx 4.910$
    
- $\sqrt{3}\pi \approx 1.732 \times 3.141 \approx 5.441$
    

$$\text{Ratio} = \frac{4.910}{5.441} \approx \mathbf{0.9025}$$

---

### **2. The Conclusion**

$$\frac{k_F}{\Gamma L} = 0.9025 < 1$$

Because the ratio is **less than 1**, the radius of the sphere is roughly **90%** of the distance to the boundary.

**Answer:**

**Yes, the Fermi sphere fits completely inside the first Brillouin Zone.** It does not touch the zone boundaries at the L-points (the closest points).

---

### **3. The "Professor's Insight" (Reality vs. Model)**

You have correctly solved the problem using the **Free Electron Model**. In this model, the electrons don't feel the atoms much, so they form a perfect sphere, and as we proved, that sphere fits in the box.

**However**, in **real** noble metals (like Copper), the electrons are negatively charged and the atomic cores are positively charged. There is an attractive force.

- As the electrons get close to the boundary (the L-point), the positive ions pull on them.
    
- This interaction stretches the "sphere" outwards along the [111] directions.
    
- In reality, the Fermi surface of Copper actually **does** touch the L-point, forming what we call **"Necks"**.
    

So, while the _theoretical sphere_ fits (as you calculated), the _real physical shape_ looks slightly like a sphere with 8 little tubes connecting it to the next zones!

**Would you like me to summarize the key formulas from this entire exercise for your cheat sheet?**