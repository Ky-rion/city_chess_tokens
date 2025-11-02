

That's an excellent observation! The identity you've presented is known as the **Cyclic Rule** or **Triple Product Rule** in partial differentiation (Equation 14). It is arguably the most elegant identity derived from the implicit differentiation technique, and it's essential for relating variables in thermodynamics.

The formula is:

$$\left(\frac{\partial x}{\partial y}\right)_{z,f} \cdot \left(\frac{\partial y}{\partial z}\right)_{x,f} \cdot \left(\frac{\partial z}{\partial x}\right)_{y,f} = -1 \quad (14)$$

We will prove this by using the result we derived previously (Equation 12/12'), which relates a partial derivative to the ratios of other partial derivatives, all under the constraint that $f$ is constant.

---

## Proof of the Cyclic Rule (Equation 14)

### 1. The Starting Point: Implicit Differentiation Formula

We will use the general formula derived from the constraint $df=0$ (Equation 12', with the $f$ constraint made explicit):

$$\left(\frac{\partial a}{\partial b}\right)_{c,f} = - \frac{\left(\frac{\partial f}{\partial b}\right)_{a,c}}{\left(\frac{\partial f}{\partial a}\right)_{b,c}}$$

Here, $a$, $b$, and $c$ are any cyclic permutation of $x$, $y$, and $z$. We will apply this formula to each of the three terms in Equation (14).

### 2. Express Each Term in the Product

We rewrite the three partial derivatives in the product using the formula above, always remembering that the constraint $f$ is constant is maintained across all derivatives ($\left(\frac{\partial f}{\partial a}\right)_{b,c}$ implies $b$ and $c$ are constant, but the function $f$ itself depends on all three variables).

**Term**

**Variables (a,b,c)**

**Formula Application**

**Term 1:** $\left(\frac{\partial x}{\partial y}\right)_{z,f}$

$a=x$, $b=y$, $c=z$

$\left(\frac{\partial x}{\partial y}\right)_{z,f} = - \frac{\left(\frac{\partial f}{\partial y}\right)_{x,z}}{\left(\frac{\partial f}{\partial x}\right)_{y,z}}$

**Term 2:** $\left(\frac{\partial y}{\partial z}\right)_{x,f}$

$a=y$, $b=z$, $c=x$

$\left(\frac{\partial y}{\partial z}\right)_{x,f} = - \frac{\left(\frac{\partial f}{\partial z}\right)_{y,x}}{\left(\frac{\partial f}{\partial y}\right)_{z,x}}$

**Term 3:** $\left(\frac{\partial z}{\partial x}\right)_{y,f}$

$a=z$, $b=x$, $c=y$

$\left(\frac{\partial z}{\partial x}\right)_{y,f} = - \frac{\left(\frac{\partial f}{\partial x}\right)_{z,y}}{\left(\frac{\partial f}{\partial z}\right)_{x,y}}$

**_Note on notation:_** The partial derivative $\left(\frac{\partial f}{\partial y}\right)_{x,z}$ is exactly the same as $\left(\frac{\partial f}{\partial y}\right)_{z,x}$—the order of the constant variables in the subscript does not matter.

### 3. Multiply the Three Expressions

Now, we substitute these three expressions back into the product in Equation (14):

$$\left(\frac{\partial x}{\partial y}\right)_{z,f} \cdot \left(\frac{\partial y}{\partial z}\right)_{x,f} \cdot \left(\frac{\partial z}{\partial x}\right)_{y,f} = \left[ - \frac{\left(\frac{\partial f}{\partial y}\right)_{x,z}}{\left(\frac{\partial f}{\partial x}\right)_{y,z}} \right] \cdot \left[ - \frac{\left(\frac{\partial f}{\partial z}\right)_{y,x}}{\left(\frac{\partial f}{\partial y}\right)_{z,x}} \right] \cdot \left[ - \frac{\left(\frac{\partial f}{\partial x}\right)_{z,y}}{\left(\frac{\partial f}{\partial z}\right)_{x,y}} \right]$$

### 4. Simplify the Product

Let's look at the signs first. We have the product of three negative signs:

$$(-1) \cdot (-1) \cdot (-1) = -1$$

Now, let's look at the partial derivatives (the fractions). Notice the remarkable structure: they form a **telescoping product** where every numerator has a matching denominator:

$$\text{Product} = (-1) \cdot \left[ \frac{(\partial f / \partial y)_{x,z}}{(\partial f / \partial x)_{y,z}} \cdot \frac{(\partial f / \partial z)_{y,x}}{(\partial f / \partial y)_{z,x}} \cdot \frac{(\partial f / \partial x)_{z,y}}{(\partial f / \partial z)_{x,y}} \right]$$

-   The numerator $(\partial f / \partial y)_{x,z}$ cancels out the denominator $(\partial f / \partial y)_{z,x}$.
    
-   The numerator $(\partial f / \partial z)_{y,x}$ cancels out the denominator $(\partial f / \partial z)_{x,y}$.
    
-   The numerator $(\partial f / \partial x)_{z,y}$ cancels out the denominator $(\partial f / \partial x)_{y,z}$.
    

Since all the fractions cancel out to $1$, the entire product simplifies to:

$$\left(\frac{\partial x}{\partial y}\right)_{z,f} \cdot \left(\frac{\partial y}{\partial z}\right)_{x,f} \cdot \left(\frac{\partial z}{\partial x}\right)_{y,f} = (-1) \cdot (1) = -1 \quad \text{Q.E.D.}$$

This **Cyclic Rule** is one of the most powerful tools in thermodynamic calculations, as it allows you to relate three derivatives, where the variables held constant are cycled for each term. This is often used to simplify complex partial derivatives involving state variables like pressure, volume, and temperature.