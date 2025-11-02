

This is part (f) of the quantum mechanics problem, which uses the results from the ladder operator formalism to find the relationship between the maximum and minimum eigenvalues of $\mathbf{\hat{L}}_z$.

The problem introduces:

-   $|f_t\rangle$: The top state, which is the eigenvector of $\mathbf{\hat{L}}_z$ with the maximum eigenvalue, $\mu_{\text{max}} = \hbar l$.
    
    $$\mathbf{\hat{L}}_z |f_t\rangle = \hbar l |f_t\rangle$$
    
-   $|f_b\rangle$: The bottom state, which is the eigenvector of $\mathbf{\hat{L}}_z$ with the minimum eigenvalue, $\mu_{\text{min}} = \hbar \tilde{l}$.
    
    $$\mathbf{\hat{L}}_z |f_b\rangle = \hbar \tilde{l} |f_b\rangle$$
    

The states $|f_t\rangle$ and $|f_b\rangle$ are also eigenvectors of $\mathbf{\hat{L}}^2$ with the common eigenvalue $\lambda$:

$$\mathbf{\hat{L}}^2 |f_t\rangle = \lambda |f_t\rangle$$

$$\mathbf{\hat{L}}^2 |f_b\rangle = \lambda |f_b\rangle$$

## 1. Action of Ladder Operators on Boundary States

By definition, the raising operator $\mathbf{\hat{L}}_{+}$ acting on the highest state $|f_t\rangle$ must yield the zero vector, as there are no higher states:

$$\mathbf{\hat{L}}_{+} |f_t\rangle = 0$$

Similarly, the lowering operator $\mathbf{\hat{L}}_{-}$ acting on the lowest state $|f_b\rangle$ must yield the zero vector:

$$\mathbf{\hat{L}}_{-} |f_b\rangle = 0$$

---

## 2. Calculation of $\mathbf{\hat{L}}^2 |f_t\rangle$

We use the identity derived in part (e) that involves the product $\mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+}$:

$$\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} + \mathbf{\hat{L}}_z^2 + \hbar \mathbf{\hat{L}}_z$$

Now, apply this operator to the top state $|f_t\rangle$:

$$\mathbf{\hat{L}}^2 |f_t\rangle = \left(\mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} + \mathbf{\hat{L}}_z^2 + \hbar \mathbf{\hat{L}}_z\right) |f_t\rangle$$

$$\mathbf{\hat{L}}^2 |f_t\rangle = \mathbf{\hat{L}}_{-} (\mathbf{\hat{L}}_{+} |f_t\rangle) + \mathbf{\hat{L}}_z^2 |f_t\rangle + \hbar \mathbf{\hat{L}}_z |f_t\rangle$$

Substitute the boundary condition $\mathbf{\hat{L}}_{+} |f_t\rangle = 0$:

$$\mathbf{\hat{L}}^2 |f_t\rangle = \mathbf{\hat{L}}_{-} (0) + \mathbf{\hat{L}}_z^2 |f_t\rangle + \hbar \mathbf{\hat{L}}_z |f_t\rangle$$

$$\mathbf{\hat{L}}^2 |f_t\rangle = 0 + \mathbf{\hat{L}}_z (\mathbf{\hat{L}}_z |f_t\rangle) + \hbar (\mathbf{\hat{L}}_z |f_t\rangle)$$

Substitute the $\mathbf{\hat{L}}_z$ eigenvalue $\mathbf{\hat{L}}_z |f_t\rangle = \hbar l |f_t\rangle$:

$$\mathbf{\hat{L}}^2 |f_t\rangle = \mathbf{\hat{L}}_z (\hbar l |f_t\rangle) + \hbar (\hbar l |f_t\rangle)$$

$$\mathbf{\hat{L}}^2 |f_t\rangle = \hbar l (\mathbf{\hat{L}}_z |f_t\rangle) + \hbar^2 l |f_t\rangle$$

$$\mathbf{\hat{L}}^2 |f_t\rangle = \hbar l (\hbar l |f_t\rangle) + \hbar^2 l |f_t\rangle$$

$$\mathbf{\hat{L}}^2 |f_t\rangle = \hbar^2 l^2 |f_t\rangle + \hbar^2 l |f_t\rangle$$

$$\mathbf{\hat{L}}^2 |f_t\rangle = \hbar^2 l (l + 1) |f_t\rangle$$

Since $\mathbf{\hat{L}}^2 |f_t\rangle = \lambda |f_t\rangle$, we find the eigenvalue $\lambda$ in terms of $l$:

$$\lambda = \hbar^2 l (l + 1)$$

---

## 3. Calculation of $\mathbf{\hat{L}}^2 |f_b\rangle$

We use the other identity derived in part (e) that involves the product $\mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-}$:

$$\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} + \mathbf{\hat{L}}_z^2 - \hbar \mathbf{\hat{L}}_z$$

Now, apply this operator to the bottom state $|f_b\rangle$:

$$\mathbf{\hat{L}}^2 |f_b\rangle = \left(\mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} + \mathbf{\hat{L}}_z^2 - \hbar \mathbf{\hat{L}}_z\right) |f_b\rangle$$

$$\mathbf{\hat{L}}^2 |f_b\rangle = \mathbf{\hat{L}}_{+} (\mathbf{\hat{L}}_{-} |f_b\rangle) + \mathbf{\hat{L}}_z^2 |f_b\rangle - \hbar \mathbf{\hat{L}}_z |f_b\rangle$$

Substitute the boundary condition $\mathbf{\hat{L}}_{-} |f_b\rangle = 0$:

$$\mathbf{\hat{L}}^2 |f_b\rangle = \mathbf{\hat{L}}_{+} (0) + \mathbf{\hat{L}}_z^2 |f_b\rangle - \hbar \mathbf{\hat{L}}_z |f_b\rangle$$

$$\mathbf{\hat{L}}^2 |f_b\rangle = 0 + \mathbf{\hat{L}}_z (\mathbf{\hat{L}}_z |f_b\rangle) - \hbar (\mathbf{\hat{L}}_z |f_b\rangle)$$

Substitute the $\mathbf{\hat{L}}_z$ eigenvalue $\mathbf{\hat{L}}_z |f_b\rangle = \hbar \tilde{l} |f_b\rangle$:

$$\mathbf{\hat{L}}^2 |f_b\rangle = \mathbf{\hat{L}}_z (\hbar \tilde{l} |f_b\rangle) - \hbar (\hbar \tilde{l} |f_b\rangle)$$

$$\mathbf{\hat{L}}^2 |f_b\rangle = \hbar \tilde{l} (\mathbf{\hat{L}}_z |f_b\rangle) - \hbar^2 \tilde{l} |f_b\rangle$$

$$\mathbf{\hat{L}}^2 |f_b\rangle = \hbar \tilde{l} (\hbar \tilde{l} |f_b\rangle) - \hbar^2 \tilde{l} |f_b\rangle$$

$$\mathbf{\hat{L}}^2 |f_b\rangle = \hbar^2 \tilde{l}^2 |f_b\rangle - \hbar^2 \tilde{l} |f_b\rangle$$

$$\mathbf{\hat{L}}^2 |f_b\rangle = \hbar^2 \tilde{l} (\tilde{l} - 1) |f_b\rangle$$

Since $\mathbf{\hat{L}}^2 |f_b\rangle = \lambda |f_b\rangle$, we find the eigenvalue $\lambda$ in terms of $\tilde{l}$:

$$\lambda = \hbar^2 \tilde{l} (\tilde{l} - 1)$$

---

## 4. Conclusion

Since both $|f_t\rangle$ and $|f_b\rangle$ are eigenvectors of $\mathbf{\hat{L}}^2$ with the same eigenvalue $\lambda$, we must equate the expressions for $\lambda$ found in steps 2 and 3:

$$\hbar^2 l (l + 1) = \hbar^2 \tilde{l} (\tilde{l} - 1)$$

Dividing both sides by $\hbar^2$ yields the required result:

$$l(l + 1) = \tilde{l}(\tilde{l} - 1)$$