

![[Pasted image 20260206202126.png]]
![[Pasted image 20260206202157.png]]

Welcome back to class! You are doing great. We are now stepping out of "Real Space" (where atoms live) and fully into "Reciprocal Space" (where waves and momenta live).

This part of the question is all about **geometry** and **maps**.

### **Part (c): The Reciprocal Lattice and the $\Gamma$-$L$ Distance**

This question has two main tasks:

1. Identify the structure of the reciprocal lattice.
    
2. Calculate the distance from the center ($\Gamma$) to a specific point on the boundary ($L$).
    

Let's break down the solution provided by your professor.

---

### **1. What is the Reciprocal Lattice of an FCC Crystal?**

Imagine you have an FCC crystal in real space. If you perform the mathematical transformation to turn it into reciprocal space, the geometry flips.

- **The Rule:** The reciprocal lattice of a **Face-Centered Cubic (FCC)** lattice is a **Body-Centered Cubic (BCC)** lattice.
    
- _(Fun fact: It works the other way too. The reciprocal of BCC is FCC)._
    

**The Math (from the solution image):**

Your professor calculates the "Primitive Reciprocal Lattice Vectors" ($\vec{b}_1, \vec{b}_2, \vec{b}_3$).

- The real space vectors are $\vec{a}_1, \vec{a}_2, \vec{a}_3$ (length scale $a$).
    
- Using the cross-product formula for reciprocal vectors, he gets:
    
    $$\vec{b}_1 = \frac{2\pi}{a}(-1, 1, 1)$$
    
    $$\vec{b}_2 = \frac{2\pi}{a}(1, -1, 1)$$
    
    $$\vec{b}_3 = \frac{2\pi}{a}(1, 1, -1)$$
    

These three vectors form the basis of a **BCC lattice**.

However, the "cube" that holds this BCC structure has a side length of $\frac{4\pi}{a}$.

> **Key Takeaway:** The map of an FCC metal is a BCC grid in reciprocal space with a cube size of $\frac{4\pi}{a}$.

---

### **2. Calculating the Distance $\Gamma L$**

We need to find the distance from the center of the zone ($\Gamma$) to the point $L$.

**Where is L?**

- Look at the diagram in your problem (the funny-looking shape is a **Truncated Octahedron**).
    
- **$\Gamma$ (Gamma)** is the exact center point $(0,0,0)$.
    
- **$L$** is the center of one of the hexagonal faces.
    
- The question tells us $L$ lies along the **$[111]$ direction** (the diagonal).
    

The solution offers **two methods** to calculate this distance. Both give the same answer, but they visualize it differently.

#### **Method 1: The Vector Approach (The Formal Way)**

1. **Find the Neighbor:** In reciprocal space, we look for the nearest lattice point along the diagonal direction $[111]$.
    
    If we add the three basis vectors together ($\vec{b}_1 + \vec{b}_2 + \vec{b}_3$), we get a vector pointing straight along the diagonal:
    
    $$\text{Vector sum} = \frac{2\pi}{a}(1, 1, 1)$$
    
2. **The Brillouin Zone Boundary:** The definition of the Brillouin Zone boundary is the **perpendicular bisector** between the center point and the next lattice point.
    
    - This means the boundary is exactly **halfway** to the next point.
        
3. **Calculate the Length:**
    
    - The length of the full vector $\frac{2\pi}{a}(1, 1, 1)$ is:
        
        $$\text{Length} = \frac{2\pi}{a} \sqrt{1^2 + 1^2 + 1^2} = \frac{2\pi\sqrt{3}}{a}$$
        
    - Since $L$ is halfway, we divide by 2:
        
        $$\text{Distance } \Gamma L = \frac{1}{2} \cdot \frac{2\pi\sqrt{3}}{a} = \frac{\sqrt{3}\pi}{a}$$
        

#### **Method 2: The Geometry Approach (The Visual Way)**

1. **Imagine the Cube:** Remember that the reciprocal lattice is a **BCC cube** with side length $A_{rec} = \frac{4\pi}{a}$.
    
2. **Locate the Points:**
    
    - $\Gamma$ is at the very center of this cube.
        
    - The nearest lattice points are at the **corners** of the cube.
        
3. **The Diagonal:** The full diagonal of a cube with side $A_{rec}$ is $A_{rec}\sqrt{3}$.
    
    $$\text{Diagonal} = \frac{4\pi}{a}\sqrt{3}$$
    
4. **The Fraction:**
    
    - The distance from the center ($\Gamma$) to the corner is **half** the diagonal.
        
    - The Brillouin Zone boundary ($L$) cuts that distance in **half again**.
        
    - So, the distance to $L$ is **one quarter** ($1/4$) of the full space diagonal.
        
        $$\text{Distance } \Gamma L = \frac{1}{4} \cdot \left( \frac{4\pi}{a}\sqrt{3} \right) = \frac{\sqrt{3}\pi}{a}$$
        

---

### **The Final Answer**

The distance from the center $\Gamma$ to the $L$-point is:

$$\Gamma L = \frac{\sqrt{3}\pi}{a}$$

This result is crucial for the next step. Usually, in these problems, we compare the **Fermi Radius ($k_F$)** we found in Part (a) with this **Distance to the Boundary ($\Gamma L$)**.

- If $k_F < \Gamma L$, the electrons fit inside the sphere.
    
- If $k_F > \Gamma L$, the sphere crashes into the boundary and the metal behaves very differently!
    

**Would you like to move on to the final part where we (likely) compare these two values?**