

This is part (d) of the angular momentum problem. You are asked to show that the square of the $\mathbf{\hat{L}}_z$ eigenvalue ($\mu^2$) must be less than or equal to the $\mathbf{\hat{L}}^2$ eigenvalue ($\lambda$):

$$\mu^2 \le \lambda$$

This is a fundamental constraint in the quantum theory of angular momentum, meaning the magnitude of any single component of the angular momentum cannot exceed the magnitude of the total angular momentum.

## 1. Relate $\mathbf{\hat{L}}^2$ and $\mathbf{\hat{L}}_z$

The total angular momentum squared operator $\mathbf{\hat{L}}^2$ is defined in terms of its components:

$$\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 + \mathbf{\hat{L}}_z^2$$

We can rearrange this equation to express the sum of the squares of the $x$ and $y$ components:

$$\mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 = \mathbf{\hat{L}}^2 - \mathbf{\hat{L}}_z^2$$

## 2. Evaluate the Expectation Value

We use the common eigenvector $|f\rangle$ for $\mathbf{\hat{L}}^2$ and $\mathbf{\hat{L}}_z$, with eigenvalues $\lambda$ and $\mu$ respectively:

$$\mathbf{\hat{L}}^2 |f\rangle = \lambda |f\rangle$$

$$\mathbf{\hat{L}}_z |f\rangle = \mu |f\rangle$$

Now, consider the expectation value of the operator $\mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2$ in the state $|f\rangle$:

$$\langle f | (\mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2) |f \rangle = \langle f | (\mathbf{\hat{L}}^2 - \mathbf{\hat{L}}_z^2) |f \rangle$$

## 3. Apply Eigenvalue Equations

We evaluate the right-hand side (RHS) using the eigenvalue relations:

$$\begin{aligned} \text{RHS} &= \langle f | \mathbf{\hat{L}}^2 |f \rangle - \langle f | \mathbf{\hat{L}}_z^2 |f \rangle \\ &= \langle f | (\lambda |f \rangle) - \langle f | (\mu^2 |f \rangle) \end{aligned}$$

Note: Since $\mathbf{\hat{L}}_z^2 |f \rangle = \mathbf{\hat{L}}_z (\mu |f \rangle) = \mu (\mathbf{\hat{L}}_z |f \rangle) = \mu (\mu |f \rangle) = \mu^2 |f \rangle$.

Since $\lambda$ and $\mu^2$ are scalars:

$$\text{RHS} = \lambda \langle f | f \rangle - \mu^2 \langle f | f \rangle = (\lambda - \mu^2) \langle f | f \rangle$$

Assuming the eigenvector is normalized ($\langle f | f \rangle = 1$), the RHS simplifies to:

$$\langle f | (\mathbf{\hat{L}}^2 - \mathbf{\hat{L}}_z^2) |f \rangle = \lambda - \mu^2$$

## 4. Physical Constraint

The left-hand side (LHS) of the expectation value is:

$$\text{LHS} = \langle f | (\mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2) |f \rangle = \langle f | \mathbf{\hat{L}}_x^2 |f \rangle + \langle f | \mathbf{\hat{L}}_y^2 |f \rangle$$

The operators $\mathbf{\hat{L}}_x$ and $\mathbf{\hat{L}}_y$ are Hermitian. For any Hermitian operator $\mathbf{\hat{A}}$, the expectation value of its square, $\langle f | \mathbf{\hat{A}}^2 |f \rangle$, is always non-negative (greater than or equal to zero). This is because:

$$\langle f | \mathbf{\hat{A}}^2 |f \rangle = \langle f | \mathbf{\hat{A}}^{\dagger} \mathbf{\hat{A}} |f \rangle = \langle \mathbf{\hat{A}} f | \mathbf{\hat{A}} f \rangle = || \mathbf{\hat{A}} |f \rangle ||^2 \ge 0$$

where $|| \mathbf{\hat{A}} |f \rangle ||^2$ is the squared norm of the state $\mathbf{\hat{A}} |f \rangle$.

Therefore, we must have:

$$\langle f | \mathbf{\hat{L}}_x^2 |f \rangle \ge 0 \quad \text{and} \quad \langle f | \mathbf{\hat{L}}_y^2 |f \rangle \ge 0$$

which means the LHS must be non-negative:

$$\text{LHS} = \langle f | (\mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2) |f \rangle \ge 0$$

## 5. Conclusion

Equating the LHS and RHS:

$$\lambda - \mu^2 \ge 0$$

Rearranging the inequality gives the required result:

$$\mathbf{\mu^2 \le \lambda}$$