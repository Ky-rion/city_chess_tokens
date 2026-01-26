

![[Pasted image 20260125185520.png]]
![[Pasted image 20260125185527.png]]

Welcome back to class! You are doing great. We are now shifting gears from "Coordinate Systems" (Miller Indices) to **"Territory."**

In Part (c), we are asked to construct the **Wigner-Seitz Cell**. This is one of the most famous concepts in solid-state physics.

### What is a Wigner-Seitz Cell?

Imagine every atom in the crystal is a person standing in a crowded room. The Wigner-Seitz cell is that person's **"Personal Space."**

Mathematically, it is defined as: **The region of space that is closer to _this_ specific lattice point than to any other lattice point.**

If you were an electron flying through the crystal and you entered this cell, you would "belong" to the atom in the center.

---

### The "Recipe" (German Solution Translation)

Your professor provided a 3-step recipe in the solution text. Let's translate and break down exactly what that German text says:

1.  **"Nächste Gitterpunkte wählen"**
    
    -   _Translation:_ Choose the nearest lattice points.
        
    -   _Action:_ Look at your central atom (the origin). Who are its immediate neighbors?
        
2.  **"Verbindungslinie"**
    
    -   _Translation:_ [Draw] the connecting line.
        
    -   _Action:_ Draw an imaginary line connecting your center atom to a neighbor.
        
3.  **"Mittelsenkrechte ziehen"**
    
    -   _Translation:_ Draw the perpendicular bisector.
        
    -   _Action:_ Go exactly to the middle of that connecting line and draw a wall perpendicular ($90^\circ$) to it.
        

**"Einschließende Fläche ist Wiegner Seitz"**

-   _Translation:_ The enclosing area is the Wigner-Seitz [Cell].
    
-   _Meaning:_ Once you draw these walls for all neighbors, the trapped area in the middle is your cell.
    

---

### Constructing Your Cell (Step-by-Step)

Let's apply the recipe to your specific grid. We have a **Square Lattice**.

-   $\vec{a_1}$ points right (x-axis).
    
-   $\vec{a_2}$ points up (y-axis).
    

#### Step 1: The Right Neighbor

-   **Connect:** Draw a line from the center $(0,0)$ to the neighbor on the right $(a, 0)$.
    
-   **Bisect:** The middle of this line is at $x = a/2$. Draw a vertical wall there.
    
-   _Result:_ This forms the **right wall** of your box.
    

#### Step 2: The Left Neighbor

-   **Connect:** Draw a line to the neighbor on the left $(-a, 0)$.
    
-   **Bisect:** The middle is at $x = -a/2$. Draw a vertical wall there.
    
-   _Result:_ This forms the **left wall**.
    

#### Step 3: The Top Neighbor

-   **Connect:** Draw a line to the neighbor above $(0, a)$.
    
-   **Bisect:** The middle is at $y = a/2$. Draw a horizontal wall there.
    
-   _Result:_ This forms the **ceiling**.
    

#### Step 4: The Bottom Neighbor

-   **Connect:** Draw a line to the neighbor below $(0, -a)$.
    
-   **Bisect:** The middle is at $y = -a/2$. Draw a horizontal wall there.
    
-   _Result:_ This forms the **floor**.
    

### The Result

When you combine these four "walls" (bisectors), you get a perfect square centered on the origin.

-   This square is shown as the blue box in your solution image.
    
-   This is the **Primitive Unit Cell** for this lattice.
    

> **Professor's Insight:** Why didn't we check the diagonal neighbors?
> 
> We actually _did_ check them mentally! But the diagonal neighbors are further away. If you drew walls between them and the center, those walls would be too far out—they would fall _behind_ the square walls we already built. The Wigner-Seitz cell is always the **smallest** enclosed volume.

---

**Next Step for you:**

To test your intuition: Imagine if we stretched the lattice so the atoms were very far apart horizontally, but close together vertically (a tall, skinny rectangle lattice). What would happen to the shape of the Wigner-Seitz cell? Would it become a tall rectangle or a wide rectangle? (Think about where the "halfway" walls would be!).