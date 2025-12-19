

[Before we get to that question, can you derive what you just said mathematically? Specifically the part about having at least one bound state. Can you start at the Schroedinger equation and go from there?]


You've got it. This is a classic and very elegant proof. Let's walk through it step-by-step, starting from the Schrödinger equation.

### 1. ⚙️ Setting up the Problem

First, let's define our system. We have a 1D symmetric potential well of width $2a$ and depth $V_0$.

To make the math cleanest, we will set the potential **inside** the well to $V=0$ and the potential **outside** the well to $V=V_0$. (This is just shifting the energy axis; it's physically identical to the $-V_0$ to $0$ setup).

-   **Region I ($x < -a$):** $V(x) = V_0$
    
-   **Region II ($-a \le x \le a$):** $V(x) = 0$
    
-   **Region III ($x > a$):** $V(x) = V_0$
    

We are looking for bound states, which means the particle is trapped. Its total energy $E$ must be less than the potential at infinity.

Therefore, we are looking for solutions with $0 < E < V_0$.

### 2. ✍️ Solving the Schrödinger Equation

The time-independent Schrödinger equation (TISE) is:

$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + V(x)\psi(x) = E\psi(x)$$

We can rewrite this as:

$$\frac{d^2\psi}{dx^2} = \frac{2m}{\hbar^2}(V(x) - E)\psi(x)$$

Let's solve this for our regions:

-   **Region II (Inside the well, $|x| \le a$):**
    
    -   $V(x) = 0$. The TISE becomes: $\frac{d^2\psi_{II}}{dx^2} = \frac{2m}{\hbar^2}(-E)\psi_{II}$
        
    -   Since $E > 0$, this is a negative coefficient. Let's define a real, positive number $k$:
        
        $$k^2 = \frac{2mE}{\hbar^2}$$
        
    -   The equation is $\frac{d^2\psi_{II}}{dx^2} = -k^2\psi_{II}$, which has oscillating solutions:
        
        $\psi_{II}(x) = A \sin(kx) + B \cos(kx)$
        
-   **Regions I & III (Outside the well, $|x| > a$):**
    
    -   $V(x) = V_0$. The TISE becomes: $\frac{d^2\psi_{out}}{dx^2} = \frac{2m}{\hbar^2}(V_0 - E)\psi_{out}$
        
    -   Since $E < V_0$, the term $(V_0 - E)$ is positive. Let's define a real, positive number $\kappa$ (kappa):
        
        $$\kappa^2 = \frac{2m(V_0 - E)}{\hbar^2}$$
        
    -   The equation is $\frac{d^2\psi_{out}}{dx^2} = \kappa^2\psi_{out}$, which has real exponential solutions.
        
    -   **In Region I ($x < -a$):** The solution $\psi_I(x) = C e^{\kappa x} + D e^{-\kappa x}$ must go to 0 as $x \to -\infty$. This means $D=0$. So, $\psi_I(x) = C e^{\kappa x}$.
        
    -   **In Region III ($x > a$):** The solution $\psi_{III}(x) = F e^{\kappa x} + G e^{-\kappa x}$ must go to 0 as $x \to +\infty$. This means $F=0$. So, **$\psi_{III}(x) = G e^{-\kappa x}$**.
        

### 3. 🪞 Applying Symmetry

Because our potential $V(x)$ is symmetric, the solutions $\psi(x)$ _must_ be either **even** (symmetric) or **odd** (anti-symmetric). The lowest energy state (the ground state) is _always_ the even one. Let's focus on finding this **even solution**.

-   For $\psi(x)$ to be even, $\psi(x) = \psi(-x)$.
    
-   Inside the well, $\psi_{II}(x) = A \sin(kx) + B \cos(kx)$. For this to be an even function, the odd part ($A \sin(kx)$) must be zero. So, $A=0$.
    
    $\psi_{II}(x) = B \cos(kx)$
    
-   This also implies that the two outside solutions must be equal, so $C=G$.
    

### 4. 🤝 Matching the Boundaries

Now we "glue" the wave functions together at the boundary $x=a$. The wave function $\psi$ and its derivative $\psi'$ must be continuous.

1.  $\psi$ is continuous at $x=a$:
    
    $\psi_{II}(a) = \psi_{III}(a)$
    
    $$B \cos(ka) = G e^{-\kappa a} \quad \text{--- (Eq. 1)}$$
    
2.  $\psi'$ is continuous at $x=a$:
    
    $\frac{d\psi_{II}}{dx}\bigg|_{x=a} = \frac{d\psi_{III}}{dx}\bigg|_{x=a}$
    
    $-B k \sin(ka) = -G \kappa e^{-\kappa a}$
    
    $$B k \sin(ka) = G \kappa e^{-\kappa a} \quad \text{--- (Eq. 2)}$$
    

Now, to find the allowed energies, we divide (Eq. 2) by (Eq. 1). This handily eliminates the constants $B$ and $G$:

$$\frac{B k \sin(ka)}{B \cos(ka)} = \frac{G \kappa e^{-\kappa a}}{G e^{-\kappa a}}$$

$$k \tan(ka) = \kappa$$

This is the **transcendental equation** for the allowed energies of the **even states**. A valid solution (a bound state) exists if we can find an energy $E$ that satisfies this equation.

### 5. 📈 The Graphical Proof (The Final Step)

This equation $k \tan(ka) = \kappa$ is tricky because both $k$ and $\kappa$ depend on the energy $E$ we're looking for.

Let's introduce two dimensionless variables. Let:

-   $\xi = ka = a\frac{\sqrt{2mE}}{\hbar}$
    
-   $\eta = \kappa a = a\frac{\sqrt{2m(V_0 - E)}}{\hbar}$
    

Now let's rewrite our equations in terms of $\xi$ (xi) and $\eta$ (eta).

1.  **The "Condition" Equation:** $k \tan(ka) = \kappa$
    
    -   Multiply by $a$: $(ka) \tan(ka) = (\kappa a)$
        
    -   **$\eta = \xi \tan(\xi)$**
        
2.  **The "Well" Equation:** Let's find a relation between $\xi$ and $\eta$ that _doesn't_ depend on $E$.
    
    -   $\xi^2 + \eta^2 = (ka)^2 + (\kappa a)^2 = a^2(k^2 + \kappa^2)$
        
    -   $\xi^2 + \eta^2 = a^2 \left( \frac{2mE}{\hbar^2} + \frac{2m(V_0 - E)}{\hbar^2} \right)$
        
    -   $\xi^2 + \eta^2 = a^2 \left( \frac{2mV_0}{\hbar^2} \right)$
        
    -   This sum is a constant that only depends on the "strength" of the well (its depth $V_0$ and width $2a$). Let's call this constant $R^2$:
        
        $\xi^2 + \eta^2 = R^2$
        

A bound state exists if there is an intersection between these two equations in the first quadrant (since $\xi$ and $\eta$ must be positive).

**Let's plot them:**

-   Graph 1: $\xi^2 + \eta^2 = R^2$
    
    This is the equation of a circle centered at the origin $(0,0)$ with radius $R$. In the first quadrant, it's a quarter-circle that starts at $(0, R)$ on the $\eta$-axis and ends at $(R, 0)$ on the $\xi$-axis.
    
-   Graph 2: $\eta = \xi \tan(\xi)$
    
    Let's trace this function:
    
    -   At $\xi = 0$, $\eta = 0 \tan(0) = 0$. The graph starts at the **origin (0, 0)**.
        
    -   As $\xi$ increases, $\tan(\xi)$ is positive, so the graph rises.
        
    -   As $\xi \to \pi/2$, $\tan(\xi) \to +\infty$, so the graph shoots up to a vertical asymptote.
        

**The Conclusion:**

-   The "well" (the circle) is _any_ quarter-circle, no matter how small its radius $R$ is. As long as $V_0 > 0$ and $a > 0$, the radius $R$ is greater than zero, and this graph **always** starts at some point $(0, R)$ on the positive $\eta$-axis.
    
-   The "even solution" (the tangent curve) **always** starts at the origin $(0, 0)$ and rises.
    

Because one curve starts at $(0, R)$ (with $R>0$) and goes to $(R, 0)$, and the other curve starts at $(0, 0)$ and goes up to infinity, **they are mathematically guaranteed to intersect at least once.**

Each intersection point corresponds to a valid energy $E$.

Therefore, **a 1D symmetric finite potential well always has at least one bound state** (this even, symmetric, ground state).