

This is the final and often most challenging concept in this section: the **Integrating Factor**. It directly addresses how physicists deal with inexact differentials in real-world problems, especially in thermodynamics (where, for example, $\delta Q$ can be made exact by dividing by the temperature $T$).

The question asks us to find the **integrating factor** $u(\mathbf{X})$ for the **inexact differential (6)** from the previous task, which was:

$$\mathbf{d}f = yx \, dx + x^2 \, dy$$

---

## The Concept of the Integrating Factor

An **inexact differential** $\mathbf{d}f = \sum \nu_j \, dX_j$ cannot be integrated path-independently, because it does not correspond to the total differential of any state function.

An **Integrating Factor** $u(\mathbf{X})$ is a scalar function that, when multiplied by the inexact differential, transforms it into an **exact differential** $\mathbf{d}F$:

$$\mathbf{d}F = u(\mathbf{X}) \mathbf{d}f = u(\mathbf{X}) \sum \nu_j \, dX_j$$

The new differential $\mathbf{d}F$ now _can_ be integrated path-independently, meaning there exists a **new state function** $F(\mathbf{X})$ such that $\mathbf{d}F = \mathbf{d}F(\mathbf{X})$.

The condition for the new differential to be exact is the generalized **Integrability Condition** (Equation 7), where the new coefficients are $P' = u \nu_x$ and $Q' = u \nu_y$:

$$\frac{\partial (u\nu_i)}{\partial X_j} = \frac{\partial (u\nu_j)}{\partial X_i} \quad \forall i, j$$

## Applying the Integrating Factor Method (for $N=2$)

### 1. Identify the Inexact Differential Components

From differential (6), $\mathbf{d}f = P dx + Q dy$:

-   $\nu_x = P = yx$
    
-   $\nu_y = Q = x^2$
    

The new coefficients, including the factor $u(x, y)$, are:

-   $P' = u P = u(x, y) yx$
    
-   $Q' = u Q = u(x, y) x^2$
    

### 2. Set up the Integrability Condition

For $N=2$ (with $X_1 = x$ and $X_2 = y$), the Integrability Condition (7) is:

$$\frac{\partial P'}{\partial y} = \frac{\partial Q'}{\partial x}$$

Substitute $P'$ and $Q'$:

$$\frac{\partial}{\partial y} (u yx) = \frac{\partial}{\partial x} (u x^2)$$

### 3. Solve the Partial Differential Equation (The Product Rule)

We use the product rule for differentiation on both sides: $\frac{\partial (uv)}{\partial z} = u \frac{\partial v}{\partial z} + v \frac{\partial u}{\partial z}$.

**Left Side (LHS):** Differentiate $u(x, y) yx$ with respect to $y$. Treat $x$ as a constant.

$$\text{LHS} = u \frac{\partial (yx)}{\partial y} + (yx) \frac{\partial u}{\partial y} = u(x) + (yx) \frac{\partial u}{\partial y}$$

**Right Side (RHS):** Differentiate $u(x, y) x^2$ with respect to $x$. Treat $y$ as a constant.

$$\text{RHS} = u \frac{\partial (x^2)}{\partial x} + (x^2) \frac{\partial u}{\partial x} = 2x u + (x^2) \frac{\partial u}{\partial x}$$

### 4. Simplify the Equation

Equate LHS and RHS:

$$u x + (yx) \frac{\partial u}{\partial y} = 2x u + (x^2) \frac{\partial u}{\partial x}$$

**Rearrange:**

$$(yx) \frac{\partial u}{\partial y} - (x^2) \frac{\partial u}{\partial x} = 2x u - u x = x u$$

This is a **linear first-order partial differential equation** for $u(x, y)$.

### 5. Find a Simple Solution

Finding the most general solution to this PDE is complex, but often, the required integrating factor is a simple function (e.g., $u(x)$, $u(y)$, or $u(x^n y^m)$). Let's **test a hypothesis**:

Since the equation is relatively simple in powers of $x$ and $y$, we hypothesize that the integrating factor $u$ might depend **only on $x$**, so $u(x, y) = u(x)$.

If $u$ depends only on $x$, then $\frac{\partial u}{\partial y} = 0$ (since $u$ is constant with respect to $y$).

Substitute $\frac{\partial u}{\partial y} = 0$ into the simplified PDE:

$$(yx) (0) - (x^2) \frac{d u}{d x} = x u$$

(Note: $\frac{\partial u}{\partial x}$ becomes the total derivative $\frac{d u}{d x}$ since $u$ only depends on $x$).

$$- x^2 \frac{d u}{d x} = x u$$

### 6. Solve the Ordinary Differential Equation (ODE) for $u(x)$

We now have a **separable first-order ODE** for $u(x)$:

$$\frac{1}{u} \frac{d u}{d x} = - \frac{x}{x^2} = - \frac{1}{x}$$

Integrate both sides with respect to $x$:

$$\int \frac{1}{u} \, d u = \int - \frac{1}{x} \, d x$$

$$\ln|u| = - \ln|x| + C' = \ln|x|^{-1} + C'$$

Let $C'$ be $\ln|C|$, where $C$ is an arbitrary constant.

$$\ln|u| = \ln\left| \frac{C}{x} \right|$$

Exponentiating gives the integrating factor $u(x)$:

$$u(x) = \frac{C}{x}$$

Since the integrating factor is only required up to a multiplicative constant, we can choose the simplest form by setting $C=1$.

$$\mathbf{u(x) = \frac{1}{x}}$$

---

## Verification of the Result

We found the integrating factor $u(x) = 1/x$. The new differential $\mathbf{d}F$ must be exact.

1.  **Construct the new differential $\mathbf{d}F$:**
    
    $$\mathbf{d}F = u(x) \mathbf{d}f = \frac{1}{x} (yx \, dx + x^2 \, dy)$$
    
    $$\mathbf{d}F = y \, dx + x \, dy$$
    
2.  **Check the Integrability Condition on $\mathbf{d}F$:**
    
    -   New $P' = y$
        
    -   New $Q' = x$
        
    -   $\frac{\partial P'}{\partial y} = \frac{\partial}{\partial y}(y) = 1$
        
    -   $\frac{\partial Q'}{\partial x} = \frac{\partial}{\partial x}(x) = 1$
        

Since $1 = 1$, the condition is satisfied. The new differential $\mathbf{d}F$ **is exact**.

### Physical Significance (The New State Function)

The new exact differential is $\mathbf{d}F = y \, dx + x \, dy$. This is precisely differential (5) from the previous task, whose potential function we found to be $F(x, y) = xy$.

Thus, the integrating factor $u(x) = 1/x$ successfully converted the inexact differential into the exact differential of the state function $F(x, y) = xy$.

In thermodynamics, the most famous example is making the inexact differential of heat ($\delta Q$) exact:

$$\mathbf{d}S = \frac{1}{T} \delta Q \quad (\text{at constant volume})$$

Here, **Temperature ($T$)** is the coefficient of the inexact part, and $\mathbf{u} = \mathbf{1/T}$ is the integrating factor that converts the path function $\delta Q$ into the state function **Entropy ($S$)**.