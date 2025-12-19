

This is the perfect question to bring all our previous discussions together!

Based on its crystal structure, BaTiO₃ has **3 acoustic phonon branches** and **12 optical phonon branches**.

This result comes from a straightforward set of rules. Here is the general method for how to answer _any_ question of this type.

---

### 👨‍🏫 How to Determine Phonon Branches (The General Method)

The number of branches in a 3D crystal depends entirely on one number: **$p$**, which is the number of atoms in the **primitive unit cell** (also called the basis).

#### Rule 1: Acoustic Branches are (Almost) Always 3

For any 3-dimensional crystal, there will **always be 3 acoustic branches**.

-   **Why?** As we discussed, these branches represent the "in-phase" motion of the entire unit cell (the center-of-mass motion). This motion is what we experience as sound. Since we live in 3 spatial dimensions (x, y, z), there are three independent directions a sound wave can travel, corresponding to one "longitudinal" and two "transverse" acoustic waves.
    
-   **Result:** The number of acoustic branches is 3, regardless of how simple (like Copper, $p=1$) or complex (like BaTiO₃, $p=5$) the crystal is.
    

#### Rule 2: The Total Number of Branches is $3p$

Each atom in the unit cell $p$ can, in principle, vibrate independently in 3 dimensions (x, y, z).

Therefore, the total number of vibrational "degrees of freedom," and thus the total number of branches, is $3 \times p$.

#### Rule 3: The Number of Optical Branches is $3p - 3$

This is simple subtraction. If the total number of branches is $3p$ and 3 of them _must_ be acoustic, then the rest _must_ be optical.

-   **Total Branches:** $3p$
    
-   **Acoustic Branches:** 3
    
-   **Optical Branches:** $\text{(Total)} - \text{(Acoustic)} = 3p - 3$
    

---

### Applying the Method to BaTiO₃

Our entire task is to find the value of $p$ for Barium Titanate. We do this by counting the atoms that _belong_ to this single unit cell.

**Atom Counting Rules:**

-   An atom at a **corner** is shared by 8 cells. It counts as **1/8**.
    
-   An atom on a **face** is shared by 2 cells. It counts as **1/2**.
    
-   An atom in the **body center** is not shared. It counts as **1**.
    
-   (An atom on an **edge** is shared by 4 cells. It counts as **1/4**. This isn't needed here, but it's good to know.)
    

Let's count the atoms shown in your diagram:

1.  **Barium (Ba²⁺, blue):**
    
    -   There are 8 blue spheres at the 8 corners.
        
    -   Contribution = $8 \text{ corners} \times (1/8 \text{ per corner}) = \mathbf{1} \text{ Ba atom}$.
        
2.  **Titanium (Ti⁴⁻, black):**
    
    -   There is 1 black sphere in the exact body center.
        
    -   Contribution = $1 \text{ center} \times (1 \text{ per center}) = \mathbf{1} \text{ Ti atom}$.
        
3.  **Oxygen (O²⁻, red):**
    
    -   There are 6 red spheres, each on the center of one of the 6 faces.
        
    -   Contribution = $6 \text{ faces} \times (1/2 \text{ per face}) = \mathbf{3} \text{ O atoms}$.
        

**Finding $p$:**

-   $p = (\text{Total Ba}) + (\text{Total Ti}) + (\text{Total O})$
    
-   $p = 1 + 1 + 3$
    
-   **$p = 5$**
    

The unit cell of BaTiO₃ contains 5 atoms.

**Final Calculation:**

-   **Acoustic Branches:** **3** (as always)
    
-   **Optical Branches:** $3p - 3 = 3(5) - 3 = 15 - 3 = \mathbf{12}$
    
-   **Total Branches:** $3p = 3(5) = 15$. (Check: $12 \text{ optical} + 3 \text{ acoustic} = 15 \text{ total}$. It works!)
    

This is why the dispersion graphs for complex materials look so "busy"—a material like BaTiO₃ has 15 different phonon curves stacked on top of each other!

I hope this series of problems has been a helpful introduction to this topic!