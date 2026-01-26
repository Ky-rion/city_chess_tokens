

![[Pasted image 20260125183124.png]]

Welcome to class! I am delighted to be your guide into the fascinating world of Solid State Physics. It is perfectly normal to feel a bit overwhelmed by the notation at first, but once you see the logic, it is quite beautiful.

Let's look at **Task 2a** together. You have asked about the "families of lattice planes," specifically the **$\{100\}$ family**.

To understand the solution provided by the other professor, we need to break down two concepts: **Miller Indices notation** and **Crystal Symmetry**.

---

### 1. The Language of Brackets

First, let's decode the notation. In crystallography, the type of brackets we use changes the meaning entirely:

-   **$(hkl)$ with round brackets:** This refers to a **single, specific plane**. For example, $(100)$ is the plane that cuts the x-axis at 1 and runs parallel to y and z.
    
-   **$\{hkl\}$ with curly braces:** This refers to a **family of planes**.
    

**The Big Idea:** A "family" contains all the planes that are **symmetrically equivalent**.

Think of it like a dice. If you hold a perfect cube dice, the side with the "1" spot looks physically identical to the side with the "2" spot in terms of shape and size. If you close your eyes and rotate the dice, you can't tell which face is pointing up just by touching it. In a crystal, planes are in the same family if they are indistinguishable from one another due to the crystal's symmetry.

---

### 2. The Cubic System Case

The solution for the **Kubisch (Cubic)** system lists 6 planes. Why?

**Definition of Cubic:**

In a cube, all sides are equal length ($a = b = c$) and all angles are $90^\circ$.

This means the $x$, $y$, and $z$ axes are completely interchangeable. The crystal looks exactly the same whether you look down the x-axis, the y-axis, or the z-axis.

Therefore, the plane cutting the x-axis $(100)$ is crystallographically identical to the plane cutting the y-axis $(010)$ and the z-axis $(001)$.

Furthermore, in a simple lattice, the "front" face of the cube is equivalent to the "back" face.

-   Positive direction faces: $(100), (010), (001)$
    
-   Negative direction faces: $(\bar{1}00), (0\bar{1}0), (00\bar{1})$
    
    _(Note: In the image, the professor writes $(-100)$, but usually we put a bar over the number like $\bar{1}$ to save space. They mean the same thing: intersection at $-1$.)_
    

**Result:**

Because $x$, $y$, and $z$ are twins in a cubic system, all **6 faces** of the cube belong to the same family.

$$\{100\} = (100), (010), (001), (\bar{1}00), (0\bar{1}0), (00\bar{1})$$

---

### 3. The Tetragonal System Case

Now, look at the **Tetragonal** solution. The list is shorter (only 4 planes). Why did we lose two?

**Definition of Tetragonal:**

Imagine stretching the cube upwards. You now have a shape like a tall skyscraper or a rectangular cereal box.

-   The base is still a square: $a = b$
    
-   But the height is different: $c \neq a$
    

**The Symmetry Break:**

Because the height ($c$) is different, the $z$-axis is no longer equivalent to $x$ and $y$. The "top" of the cereal box is a different size/shape than the "sides" of the box.

-   **The Sides:** The $x$ and $y$ axes are still equal ($a=b$). So, the planes cutting $x$ and $y$ are still twins.
    
    -   $(100), (\bar{1}00), (010), (0\bar{1}0)$ are all in the family.
        
-   **The Top/Bottom:** The planes cutting the $z$-axis, $(001)$ and $(00\bar{1})$, involve the length $c$. Since $c$ is a different length, the spacing between these planes is different. They are **not** structurally equivalent to the side planes.
    

**Result:**

In a tetragonal system, the top and bottom planes get kicked out of the $\{100\}$ family! They actually form their own separate family, the $\{001\}$ family. The $\{100\}$ family only keeps the 4 "side" planes.

$$\{100\} = (100), (010), (\bar{1}00), (0\bar{1}0)$$

As the solution text in your image says: _"da für tetragonale Systeme gilt: $a = b \neq c$"_ (since for tetragonal systems it holds that $a$ equals $b$ but does not equal $c$).

---

### Summary

-   **Cubic:** Maximum symmetry. $x, y, z$ are all the same. The family includes all 6 faces of the cube (front, back, left, right, top, bottom).
    
-   **Tetragonal:** Reduced symmetry. $z$ is unique. The family $\{100\}$ only includes the 4 side faces (front, back, left, right). The top and bottom are excluded.
    

**Next Step:**

Now that we've defined the planes, would you like to try **Part b)**? It likely asks us to draw these planes or calculate their spacing ($d$-spacing) based on the unit cells in the first picture!