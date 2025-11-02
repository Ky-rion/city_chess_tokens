

That's a great next step! The formula you're asking to prove, Equation (13), is a fundamental rule for partial derivatives known as the **Reciprocity Relation** (or inverse rule). It states how to flip the variables in a partial derivative.

$$\left(\frac{\partial x}{\partial y}\right)_{z,f} = \frac{1}{\left(\frac{\partial y}{\partial x}\right)_{z,f}} \quad (13)$$

We can prove this using the exact same principles of **implicit differentiation** and constraints that we established in the previous step.

---

## Proof of the Reciprocity Relation (Equation 13)

The condition for the derivation is that the function $f(x, y, z)$ is held constant, and a variable, $z$, is also held constant.

### 1. Start with the Implied Constraint

In the last derivation, we imposed two constraints:

1.  **The function $f$ is constant** ($df=0$).
    
2.  **The variable $z$ is constant** ($dz=0$).
    

Under these two constraints, we derived the intermediate equation (which we called $10'$):

$$0 = \left(\frac{\partial f}{\partial x}\right)_{y,z} dx + \left(\frac{\partial f}{\partial y}\right)_{x,z} dy \quad (*)$$

### 2. Isolate the Ratio $dx/dy$

The goal of Equation (13) is to find the derivative $\left(\frac{\partial x}{\partial y}\right)_{z,f}$. This derivative is mathematically defined as the ratio of infinitesimal changes, $\frac{dx}{dy}$, under the specified constraints ($z$ and $f$ constant).

Let's rearrange equation $(*)$ to solve for the ratio $\frac{dx}{dy}$:

1.  Move the term with $dx$ to the left side:
    
    $$-\left(\frac{\partial f}{\partial x}\right)_{y,z} dx = \left(\frac{\partial f}{\partial y}\right)_{x,z} dy$$
    
2.  Divide both sides by $dy$ (to get $dx/dy$) and divide by $-\left(\frac{\partial f}{\partial x}\right)_{y,z}$:
    

$$\frac{dx}{dy} = - \frac{\left(\frac{\partial f}{\partial y}\right)_{x,z}}{\left(\frac{\partial f}{\partial x}\right)_{y,z}}$$

Since we are performing this operation under the constraints that **$z$ and $f$ are constant**, the ratio $\frac{dx}{dy}$ is, by definition, the partial derivative $\left(\frac{\partial x}{\partial y}\right)_{z,f}$:

$$\left(\frac{\partial x}{\partial y}\right)_{z,f} = - \frac{\left(\frac{\partial f}{\partial y}\right)_{x,z}}{\left(\frac{\partial f}{\partial x}\right)_{y,z}} \quad (**)$$

### 3. Apply the Result from Equation (12)

In the previous derivation, we found the expression for the derivative $\left(\frac{\partial y}{\partial x}\right)_{z,f}$ (which was Equation 12, just with the subscript $f$ added to the constraint):

$$\left(\frac{\partial y}{\partial x}\right)_{z,f} = - \frac{\left(\frac{\partial f}{\partial x}\right)_{y,z}}{\left(\frac{\partial f}{\partial y}\right)_{x,z}} \quad (12')$$

### 4. Comparison and Conclusion

Now, compare the result from step 2 (Equation $**$) with the result from step 3 (Equation $12'$):

-   Equation $()$: Derivative $\left(\frac{\partial x}{\partial y}\right)_{z,f}$
    
    $$\left(\frac{\partial x}{\partial y}\right)_{z,f} = - \frac{(\partial f / \partial y)_{x,z}}{(\partial f / \partial x)_{y,z}}$$
    
-   **Equation $(12')$: Derivative $\left(\frac{\partial y}{\partial x}\right)_{z,f}$
    
    $$\left(\frac{\partial y}{\partial x}\right)_{z,f} = - \frac{(\partial f / \partial x)_{y,z}}{(\partial f / \partial y)_{x,z}}$$
    

Notice that the expression for $\left(\frac{\partial x}{\partial y}\right)_{z,f}$ is exactly the **inverse** (reciprocal) of the expression for $\left(\frac{\partial y}{\partial x}\right)_{z,f}$!

Therefore, we can write:

$$\left(\frac{\partial x}{\partial y}\right)_{z,f} = \frac{1}{\left(\frac{\partial y}{\partial x}\right)_{z,f}} \quad \text{Q.E.D.}$$

This **Reciprocity Relation** is a key feature of partial derivatives. It essentially means that if a derivative is defined with certain variables held constant, simply inverting the ratio of the variables (from $y$ with respect to $x$ to $x$ with respect to $y$) results in the reciprocal of the derivative value, provided the constraints (the variables in the subscript, like $z$ and $f$) are kept the same.