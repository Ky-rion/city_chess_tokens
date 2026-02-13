

![[Pasted image 20260206203056.png]]
![[Pasted image 20260206203110.png]]

Welcome back! We are making excellent progress.

In the previous parts, we mapped out the "landscape" of energy (the hills and valleys). Now, in **Part 3**, we are going to look at the **traffic** on that landscape. specifically, how fast the electrons move.

This concept is called **Group Velocity** ($\vec{v}_g$).

### 1. The Physics Concept: Group Velocity

In quantum mechanics, an electron isn't just a point; it's a "wave packet." The speed at which this packet travels is determined by the slope of the energy band.

**The Golden Rule:**

$$\vec{v}_k = \frac{1}{\hbar} \nabla_{\vec{k}} E(\vec{k})$$

- **Translation:** Velocity is the gradient (slope) of the energy.
    
- **Intuition:** Steeper energy bands $\rightarrow$ faster electrons. Flat bands $\rightarrow$ slow (heavy) electrons.
    

---

### 2. Calculating the Velocity Vector (Equation 6)

We start with our energy equation from Part (b):

$$E(\vec{k}) = -t [\cos(k_x a) + \cos(k_y a) - 2]$$

To get velocity, we need to take the derivative (gradient) with respect to $k_x$ and $k_y$.

- **Derivative of $\cos(kx \cdot a)$:** It is $-\sin(kx \cdot a) \cdot a$.
    
- **Watch the signs:** We have a $-t$ in front and a minus sign from the derivative. They cancel out to become positive ($+ta$).
    

So, the velocity vector is:

$$\vec{v}_k = \frac{ta}{\hbar} \begin{pmatrix} \sin(k_x a) \\ \sin(k_y a) \end{pmatrix}$$

This matches **Equation (6)** in the solution.

---

### 3. Speed along the [10] Direction (Equation 7)

The **[10] direction** simply means moving along the x-axis.

- Condition: $k_y = 0$.
    
- Since $\sin(0) = 0$, the y-component of velocity disappears.
    

The magnitude (speed) is:

$$|v_{[10]}| = \frac{ta}{\hbar} \sqrt{\sin^2(k_x a) + 0}$$

$$|v_{[10]}| = \frac{ta}{\hbar} \sin(k_x a)$$

**Where is this fastest?**

The sine function is maximum (value = 1) when the angle is $90^\circ$ or $\pi/2$.

- Condition: $k_x a = \frac{\pi}{2} \implies k_x = \frac{\pi}{2a}$.
    
- **Max Speed:** $v_{max} = \frac{ta}{\hbar}$.
    

---

### 4. Speed along the [11] Direction (Equation 8)

The **[11] direction** means moving along the diagonal.

- Condition: $k_x = k_y$ (Let's just call it $k$).
    

Now both x and y components contribute to the speed:

$$|v_{[11]}| = \frac{ta}{\hbar} \sqrt{\sin^2(k a) + \sin^2(k a)}$$

$$|v_{[11]}| = \frac{ta}{\hbar} \sqrt{2 \sin^2(k a)}$$

$$|v_{[11]}| = \sqrt{2} \frac{ta}{\hbar} \sin(k a)$$

**Where is this fastest?**

Again, when the sine is 1 (at $k = \frac{\pi}{2a}$).

- **Max Speed:** $v_{max} = \sqrt{2} \frac{ta}{\hbar}$.
    

---

### 5. Comparing the Speeds (The "Aha!" Moment)

The question asks: _"In which direction is the velocity maximal?"_

Let's compare our two top speeds:

1. **Along x-axis ([10]):** $1.0 \times \frac{ta}{\hbar}$
    
2. **Along diagonal ([11]):** $1.41 \times \frac{ta}{\hbar}$ (because $\sqrt{2} \approx 1.41$)
    

**Conclusion:**

The electrons can move significantly faster along the diagonal of the crystal lattice than they can along the axes. The maximum velocity is reached in the **middle of the Brillouin Zone face** (at $k=\frac{\pi}{2a}$), not at the edge or the center.

---

### 6. Physical Consequences: Anisotropy & Current

The last part of the question asks for the interpretation regarding **Current Density ($J$)**.

The formula for current density is given in **Equation (9)**:

$$J = -e \sum_k v_g(k) f(E)$$

- $v_g(k)$: How fast electrons move.
    
- $f(E)$: The probability an electron is actually there (Fermi-Dirac distribution).
    

**The Insight:**

Because the velocity $v_g$ is different in different directions (it is **Anisotropic**), the current density $J$ will also be anisotropic.

If you apply a voltage $V$ across this crystal:

- If you apply it along the **diagonal**, you will get **more current** (higher conductivity).
    
- If you apply it along the **axis**, you will get **less current** (lower conductivity).
    

**Professor's Summary:**

This proves that even in a simple-looking square lattice, the electrical properties depend heavily on the direction you measure them. The crystal is not the same in all directions!

Would you like to move on to the final part of the exercise, or shall we review any of the math here?