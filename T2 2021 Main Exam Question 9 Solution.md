

Welcome back to our virtual lecture! This is a wonderfully rigorous algebraic exercise. Here, we are peeling back the curtain to see _why_ the spherical harmonics $Y_l^m$ are the eigenfunctions of angular momentum, specifically for the $m=0$ case, using the raw differential operators.

Let's start by translating the German text to ensure we are on the exact same page:

> **Show by explicit application of the angular momentum operators in the coordinates $\phi, \eta$ (V18/S4), that $Y_l^0(\phi, \eta)$ are eigenfunctions of $\hat{L}^2, \hat{L}_z$ with eigenvalues $l(l+1)$ and $m=0$.**
> 
> _Hint: First use the formula for the derivative of the Legendre polynomials:_
> 
> $$(\eta^2 - 1)\partial_\eta P_l(\eta) = l\eta P_l(\eta) - l P_{l-1}(\eta)$$
> 
> _and then_
> 
> $$P_0(\eta) = 1, \quad P_1(\eta) = \eta, \quad l P_l(\eta) = (2l - 1)\eta P_{l-1}(\eta) - (l - 1)P_{l-2}(\eta)$$
> 
> _Hint: This task requires some algebra to complete fully, write down your approach and finish if time remains._

Let's dive into the physics and the algebra.

### Setting the Stage: Coordinates and Operators

In this problem, we are using the coordinate $\eta = \cos\theta$. The spherical harmonic for $m=0$ has no azimuthal angular dependence (no $\phi$ dependence) and is entirely proportional to the Legendre polynomials:

$$Y_l^0(\phi, \eta) = N_l P_l(\eta)$$

_(where $N_l$ is just a normalization constant)._

In terms of our new variable $\eta$, the standard angular momentum operators (setting $\hbar = 1$ as is customary when eigenvalues are written as $l(l+1)$) become:

1. **The z-component:** $\hat{L}_z = -i \frac{\partial}{\partial \phi}$
    
2. **The magnitude squared:** $\hat{L}^2 = \frac{\partial}{\partial \eta} \left( (\eta^2 - 1)\frac{\partial}{\partial \eta} \right) - \frac{1}{1-\eta^2} \frac{\partial^2}{\partial \phi^2}$
    

---

### Part 1: Proving the $\hat{L}_z$ Eigenvalue ($m=0$)

This part is very straightforward. We apply the $\hat{L}_z$ operator to our state $Y_l^0$:

$$\hat{L}_z Y_l^0(\phi, \eta) = -i \frac{\partial}{\partial \phi} \left( N_l P_l(\eta) \right)$$

Because $P_l(\eta)$ depends _only_ on $\eta$ and has absolutely no $\phi$ dependence, the partial derivative with respect to $\phi$ is simply zero:

$$\hat{L}_z Y_l^0(\phi, \eta) = 0 = 0 \cdot Y_l^0(\phi, \eta)$$

This perfectly matches the eigenvalue equation $\hat{L}_z Y_l^m = m Y_l^m$ for the specific case where **$m = 0$**.

---

### Part 2: Proving the $\hat{L}^2$ Eigenvalue ($l(l+1)$)

Here is where we need to roll up our sleeves and use the hints provided. We want to evaluate $\hat{L}^2 P_l(\eta)$.

Because there is no $\phi$ dependence, the second term of the $\hat{L}^2$ operator vanishes, leaving us with:

$$\hat{L}^2 P_l(\eta) = \frac{\partial}{\partial \eta} \left( (\eta^2 - 1)\frac{\partial}{\partial \eta} P_l(\eta) \right)$$

**Step 2.1: Use the First Hint**

Look at the bracketed term. It exactly matches the left side of your first hint! Let's substitute the hint directly into our operator equation:

$$\hat{L}^2 P_l(\eta) = \frac{\partial}{\partial \eta} \left[ l\eta P_l(\eta) - l P_{l-1}(\eta) \right]$$

Now, we execute the $\eta$ derivative using the product rule on the first term:

$$\hat{L}^2 P_l(\eta) = l P_l(\eta) + l\eta P'_l(\eta) - l P'_{l-1}(\eta)$$

_(Note: I am using the prime notation $P'$ to mean $\partial_\eta P$ to keep things clean)._

Our goal is to show that this entire expression equals $l(l+1)P_l(\eta)$, which expands to $l^2 P_l + l P_l$. We already have the $l P_l$ piece! This means we must prove that the remaining terms equal $l^2 P_l$:

**Target to prove:** $l\eta P'_l(\eta) - l P'_{l-1}(\eta) = l^2 P_l(\eta)$

**Step 2.2: Finding $P'_{l-1}$**

To prove our target, we need expressions for the derivatives. We can get $P'_l$ by simply rearranging the first hint:

$$P'_l(\eta) = \frac{l\eta P_l(\eta) - l P_{l-1}(\eta)}{\eta^2 - 1}$$

But we also need $P'_{l-1}$. Let's take the first hint and _shift the index_ down by one (replace every $l$ with $l-1$):

$$(\eta^2 - 1)P'_{l-1}(\eta) = (l-1)\eta P_{l-1}(\eta) - (l-1)P_{l-2}(\eta)$$

Now, look at your **second hint**. It contains a term $(l-1)P_{l-2}(\eta)$. Let's isolate it:

$$(l-1)P_{l-2}(\eta) = (2l - 1)\eta P_{l-1}(\eta) - l P_l(\eta)$$

Substitute this into our shifted equation:

$$(\eta^2 - 1)P'_{l-1}(\eta) = (l-1)\eta P_{l-1}(\eta) - \left[ (2l - 1)\eta P_{l-1}(\eta) - l P_l(\eta) \right]$$

$$(\eta^2 - 1)P'_{l-1}(\eta) = \left( (l - 1) - (2l - 1) \right)\eta P_{l-1}(\eta) + l P_l(\eta)$$

$$(\eta^2 - 1)P'_{l-1}(\eta) = -l\eta P_{l-1}(\eta) + l P_l(\eta)$$

Dividing by $(\eta^2 - 1)$, we now have our expression for $P'_{l-1}$:

$$P'_{l-1}(\eta) = \frac{l P_l(\eta) - l\eta P_{l-1}(\eta)}{\eta^2 - 1}$$

**Step 2.3: The Grand Cancellation**

Now we plug our expressions for $P'_l$ and $P'_{l-1}$ back into our "Target to prove" expression from Step 2.1:

$$l\eta P'_l(\eta) - l P'_{l-1}(\eta) = l\eta \left[ \frac{l\eta P_l - l P_{l-1}}{\eta^2 - 1} \right] - l \left[ \frac{l P_l - l\eta P_{l-1}}{\eta^2 - 1} \right]$$

Since they share a denominator, we can combine the numerators:

$$= \frac{1}{\eta^2 - 1} \left[ l^2\eta^2 P_l - l^2\eta P_{l-1} - l^2 P_l + l^2\eta P_{l-1} \right]$$

Look at that! The mixed terms $l^2\eta P_{l-1}$ perfectly cancel each other out, leaving:

$$= \frac{1}{\eta^2 - 1} \left[ l^2\eta^2 P_l - l^2 P_l \right]$$

$$= \frac{1}{\eta^2 - 1} \left[ l^2 P_l (\eta^2 - 1) \right]$$

The $(\eta^2 - 1)$ terms cancel out entirely, leaving exactly:

$$= l^2 P_l(\eta)$$

**Step 2.4: Final Result**

Substitute this beautiful result back into our equation from Step 2.1:

$$\hat{L}^2 P_l(\eta) = l P_l(\eta) + \left[ l^2 P_l(\eta) \right]$$

$$\hat{L}^2 P_l(\eta) = (l^2 + l) P_l(\eta)$$

$$\hat{L}^2 P_l(\eta) = l(l+1) P_l(\eta)$$

This confirms that $Y_l^0$ is indeed an eigenfunction of $\hat{L}^2$ with the eigenvalue $l(l+1)$.

Would you like me to show you how these Legendre polynomials actually dictate the 3D visual shapes of the atomic orbitals (like the $s$, $p_z$, and $d_{z^2}$ orbitals) that you encounter in chemistry?