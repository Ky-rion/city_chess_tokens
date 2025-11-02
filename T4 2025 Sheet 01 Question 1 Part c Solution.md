

That's a perfect next step! We're now going from theory to practice by using the **Integrability Conditions** you just proved to test whether specific differential forms are **exact**, and then demonstrating the key consequence: **path independence**.

This problem is set for $N=2$ coordinates, which we'll call $x$ and $y$. The general differential form is $\mathbf{d}f = P(x, y) dx + Q(x, y) dy$.

---

## Part 1: Checking for Exactness (The Integrability Condition)

A differential $\mathbf{d}f = P dx + Q dy$ is **exact** if and only if there exists a potential function $f(x, y)$ such that $P = \frac{\partial f}{\partial x}$ and $Q = \frac{\partial f}{\partial y}$.

The **Integrability Condition** is the mathematical test for this:

$$\frac{\partial P}{\partial y} = \frac{\partial Q}{\partial x}$$

### Differential (5): $df = y \, dx + x \, dy$

1.  Identify $P$ and $Q$:
    
    $$P(x, y) = y \quad \text{and} \quad Q(x, y) = x$$
    
2.  **Apply the Integrability Condition:**
    
    -   Calculate the partial derivative of $P$ with respect to $y$:
        
        $$\frac{\partial P}{\partial y} = \frac{\partial}{\partial y}(y) = 1$$
        
    -   Calculate the partial derivative of $Q$ with respect to $x$:
        
        $$\frac{\partial Q}{\partial x} = \frac{\partial}{\partial x}(x) = 1$$
        
3.  Conclusion:
    
    Since $\frac{\partial P}{\partial y} = 1$ and $\frac{\partial Q}{\partial x} = 1$, the condition is satisfied.
    
    -   **Differential (5) is an exact differential.**
        
    -   The state function is $f(x, y) = xy$. (You can check: $\frac{\partial f}{\partial x} = y$ and $\frac{\partial f}{\partial y} = x$).
        

---

### Differential (6): $df = yx \, dx + x^2 \, dy$

1.  Identify $P$ and $Q$:
    
    $$P(x, y) = yx \quad \text{and} \quad Q(x, y) = x^2$$
    
2.  **Apply the Integrability Condition:**
    
    -   Calculate the partial derivative of $P$ with respect to $y$:
        
        $$\frac{\partial P}{\partial y} = \frac{\partial}{\partial y}(yx) = x$$
        
    -   Calculate the partial derivative of $Q$ with respect to $x$:
        
        $$\frac{\partial Q}{\partial x} = \frac{\partial}{\partial x}(x^2) = 2x$$
        
3.  Conclusion:
    
    Since $\frac{\partial P}{\partial y} = x$ and $\frac{\partial Q}{\partial x} = 2x$, and $x \neq 2x$ (for $x \neq 0$), the condition is NOT satisfied.
    
    -   **Differential (6) is an inexact differential.**
        
    -   In physics, this would be a path function like $\delta Q$ (heat) or $\delta W$ (work).
        

---

## Part 2: Path Independence Verification

Now we must construct two different paths ($C_1$ and $C_2$) between the initial point $\mathbf{X}(t_0) = (0, 0)^T$ and the final point $\mathbf{X}(t_1) = (x_1, y_1)^T$ and check if the integral for the **exact differential (5)** is the same for both paths.

Let the final point be $\mathbf{X}_1 = (2, 4)$ for a concrete calculation.

### Path 1 ($C_1$): Straight Line

The path is a straight line from $(0, 0)$ to $(2, 4)$.

-   **Parametrization:** $x(t) = 2t$ and $y(t) = 4t$, for $t$ from $0$ to $1$.
    
-   **Differentials:** $dx = 2 dt$ and $dy = 4 dt$.
    
-   Differential (5) in terms of $t$:
    
    $$df = y \, dx + x \, dy = (4t)(2 dt) + (2t)(4 dt) = 8t \, dt + 8t \, dt = 16t \, dt$$
    
-   The Integral $I_1$:
    
    $$I_1 = \int_{C_1} df = \int_{t=0}^{t=1} 16t \, dt = 16 \left[ \frac{t^2}{2} \right]_0^1 = 16 \left( \frac{1}{2} - 0 \right) = \mathbf{8}$$
    

---

### Path 2 ($C_2$): Two-Segment Path (x-axis then y-axis)

This path goes from $(0, 0)$ to $(2, 0)$ (horizontal) and then from $(2, 0)$ to $(2, 4)$ (vertical).

-   **Segment $C_{2a}$ (Horizontal):**
    
    -   From $(0, 0)$ to $(2, 0)$.
        
    -   $y = 0$, so $dy = 0$. $x$ goes from $0$ to $2$.
        
    -   $df = y \, dx + x \, dy = (0) \, dx + x (0) = 0$
        
    -   Integral over $C_{2a}$: $I_{2a} = \int_{C_{2a}} 0 = 0$.
        
-   **Segment $C_{2b}$ (Vertical):**
    
    -   From $(2, 0)$ to $(2, 4)$.
        
    -   $x = 2$, so $dx = 0$. $y$ goes from $0$ to $4$.
        
    -   $df = y \, dx + x \, dy = y (0) + 2 \, dy = 2 \, dy$
        
    -   Integral over $C_{2b}$: $I_{2b} = \int_{y=0}^{y=4} 2 \, dy = 2 [y]_0^4 = 2 (4 - 0) = 8$.
        
-   The Total Integral $I_2$:
    
    $$I_2 = I_{2a} + I_{2b} = 0 + 8 = \mathbf{8}$$
    

---

## Conclusion of Verification

The integral for the exact differential (5) yielded the same result for both paths: $I_1 = 8$ and $I_2 = 8$.

$$\int_{C_1} (y \, dx + x \, dy) = \int_{C_2} (y \, dx + x \, dy) = 8$$

This result **verifies** the fundamental property of an exact (or total) differential: **Path independence**. The integral only depends on the endpoints $(0, 0)$ and $(2, 4)$.

### Quick check using the potential function:

Since $f(x, y) = xy$ is the state function for $df = y \, dx + x \, dy$:

$$I(\mathbf{X}_0, \mathbf{X}_1) = f(2, 4) - f(0, 0) = (2 \cdot 4) - (0 \cdot 0) = 8 - 0 = \mathbf{8}$$

This confirms the physical meaning of the path-independent result!