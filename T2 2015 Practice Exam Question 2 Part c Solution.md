

This is part (c) of the angular momentum problem. You need to show that the state $\mathbf{\hat{L}}_{\pm}|f\rangle$ is an **eigenvector of $\mathbf{\hat{L}}_z$ with the eigenvalue $\mu \pm \hbar$** (or the resulting state vanishes).

We start with the same conditions as before:

1.  $\mathbf{\hat{L}}^2 |f\rangle = \lambda |f\rangle$
    
2.  $\mathbf{\hat{L}}_z |f\rangle = \mu |f\rangle$
    

The proof relies on the **commutation relation** between $\mathbf{\hat{L}}_z$ and the ladder operators $\mathbf{\hat{L}}_{\pm}$.

---

## 1. Commutation Relation $[\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_{\pm}]$

The ladder operators are defined as $\mathbf{\hat{L}}_{\pm} = \mathbf{\hat{L}}_x \pm i \mathbf{\hat{L}}_y$. We compute the commutator:

$$\begin{aligned} [\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_{\pm}] &= [\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_x \pm i \mathbf{\hat{L}}_y] \\ &= [\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_x] \pm i [\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_y] \end{aligned}$$

Using the fundamental angular momentum commutation relations:

-   $[\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_x] = i \hbar \mathbf{\hat{L}}_y$
    
-   $[\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_y] = - i \hbar \mathbf{\hat{L}}_x$
    

Substituting these back:

$$\begin{aligned} [\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_{\pm}] &= (i \hbar \mathbf{\hat{L}}_y) \pm i (-i \hbar \mathbf{\hat{L}}_x) \\ &= i \hbar \mathbf{\hat{L}}_y \mp i^2 \hbar \mathbf{\hat{L}}_x \\ &= i \hbar \mathbf{\hat{L}}_y \mp (-\hbar) \mathbf{\hat{L}}_x \\ &= i \hbar \mathbf{\hat{L}}_y \pm \hbar \mathbf{\hat{L}}_x \\ &= \hbar (\mathbf{\hat{L}}_x \pm i \mathbf{\hat{L}}_y) \end{aligned}$$

Thus, the commutation relation is:

$$[\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_{\pm}] = \hbar \mathbf{\hat{L}}_{\pm}$$

---

## 2. Applying the Commutator to the Eigenvector

The commutator definition gives the operator relation:

$$\mathbf{\hat{L}}_z \mathbf{\hat{L}}_{\pm} - \mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}_z = \hbar \mathbf{\hat{L}}_{\pm}$$

We rearrange this to get an expression for $\mathbf{\hat{L}}_z \mathbf{\hat{L}}_{\pm}$:

$$\mathbf{\hat{L}}_z \mathbf{\hat{L}}_{\pm} = \mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}_z + \hbar \mathbf{\hat{L}}_{\pm}$$

Now, apply $\mathbf{\hat{L}}_z$ to the state $\mathbf{\hat{L}}_{\pm}|f\rangle$:

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{\pm}|f\rangle) = (\mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}_z + \hbar \mathbf{\hat{L}}_{\pm}) |f\rangle$$

Distribute $|f\rangle$:

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{\pm}|f\rangle) = \mathbf{\hat{L}}_{\pm} (\mathbf{\hat{L}}_z |f\rangle) + \hbar (\mathbf{\hat{L}}_{\pm} |f\rangle)$$

Next, substitute the eigenvalue equation for $|f\rangle$: $\mathbf{\hat{L}}_z |f\rangle = \mu |f\rangle$:

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{\pm}|f\rangle) = \mathbf{\hat{L}}_{\pm} (\mu |f\rangle) + \hbar (\mathbf{\hat{L}}_{\pm} |f\rangle)$$

Since $\mu$ is a scalar (the eigenvalue), we pull it out:

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{\pm}|f\rangle) = \mu (\mathbf{\hat{L}}_{\pm}|f\rangle) + \hbar (\mathbf{\hat{L}}_{\pm}|f\rangle)$$

Finally, factor out the state $\mathbf{\hat{L}}_{\pm}|f\rangle$:

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{\pm}|f\rangle) = (\mu + \hbar) (\mathbf{\hat{L}}_{\pm}|f\rangle)$$

Wait, we need to consider both $\mathbf{\hat{L}}_+$ and $\mathbf{\hat{L}}_-$ operators:

### For $\mathbf{\hat{L}}_{+}$ (Raising Operator):

$$[\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_{+}] = \hbar \mathbf{\hat{L}}_{+}$$

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{+}|f\rangle) = (\mu + \hbar) (\mathbf{\hat{L}}_{+}|f\rangle)$$

The new eigenvalue is $\mu + \hbar$.

### For $\mathbf{\hat{L}}_{-}$ (Lowering Operator):

$$[\mathbf{\hat{L}}_z, \mathbf{\hat{L}}_{-}] = -\hbar \mathbf{\hat{L}}_{-}$$

$$\mathbf{\hat{L}}_z \mathbf{\hat{L}}_{-} = \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_z - \hbar \mathbf{\hat{L}}_{-}$$

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{-}|f\rangle) = \mathbf{\hat{L}}_{-} (\mu |f\rangle) - \hbar (\mathbf{\hat{L}}_{-}|f\rangle)$$

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{-}|f\rangle) = (\mu - \hbar) (\mathbf{\hat{L}}_{-}|f\rangle)$$

The new eigenvalue is $\mu - \hbar$.

---

## Conclusion

The result

$$\mathbf{\hat{L}}_z (\mathbf{\hat{L}}_{\pm}|f\rangle) = (\mu \pm \hbar) (\mathbf{\hat{L}}_{\pm}|f\rangle)$$

proves that $\mathbf{\hat{L}}_{\pm}|f\rangle$ is an eigenvector of $\mathbf{\hat{L}}_z$ with the eigenvalue $\mu \pm \hbar$, or it vanishes (i.e., $\mathbf{\hat{L}}_{\pm}|f\rangle = 0$).

The ladder operators $\mathbf{\hat{L}}_{\pm}$ thus **raise or lower the $\mathbf{\hat{L}}_z$ eigenvalue by $\hbar$** while leaving the $\mathbf{\hat{L}}^2$ eigenvalue ($\lambda$) unchanged.