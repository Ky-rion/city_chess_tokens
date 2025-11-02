

This is part (b) of the quantum mechanics problem, asking you to show that when $\mathbf{\hat{L}}^2$ and $\mathbf{\hat{L}}_z$ share an eigenvector $|f\rangle$ with eigenvalues $\lambda$ and $\mu$ respectively, the state $\mathbf{\hat{L}}_{\pm}|f\rangle$ is also an eigenvector of $\mathbf{\hat{L}}^2$ with the same eigenvalue $\lambda$ (or the resulting state is the zero vector, i.e., it vanishes).

The given starting conditions are:

1.  $\mathbf{\hat{L}}^2 |f\rangle = \lambda |f\rangle$
    
2.  $\mathbf{\hat{L}}_z |f\rangle = \mu |f\rangle$
    

The operator $\mathbf{\hat{L}}^2$ is the total angular momentum squared operator, and $\mathbf{\hat{L}}_{\pm} = \mathbf{\hat{L}}_x \pm i \mathbf{\hat{L}}_y$ are the **raising and lowering operators** (or ladder operators).

The proof relies on the **commutation relation** between $\mathbf{\hat{L}}^2$ and $\mathbf{\hat{L}}_{\pm}$.

---

## 1. Commutation Relation

The fundamental commutation relations for angular momentum are:

$$[\mathbf{\hat{L}}_i, \mathbf{\hat{L}}_j] = i \hbar \epsilon_{ijk} \mathbf{\hat{L}}_k$$

We need to calculate the commutator $[\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_{\pm}]$:

$$\begin{aligned} [\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_{\pm}] &= [\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_x \pm i \mathbf{\hat{L}}_y] \\ &= [\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_x] \pm i [\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_y] \end{aligned}$$

From the previous result (or the general property that $\mathbf{\hat{L}}^2$ commutes with all components of $\mathbf{\hat{L}}$), we know that:

$$[\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_x] = 0$$

$$[\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_y] = 0$$

$$[\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_z] = 0$$

Therefore, the commutator is:

$$[\mathbf{\hat{L}}^2, \mathbf{\hat{L}}_{\pm}] = 0 \pm i(0) = 0$$

The total angular momentum squared operator $\mathbf{\hat{L}}^2$ **commutes** with the ladder operators $\mathbf{\hat{L}}_{\pm}$.

---

## 2. Applying the Commutator to the Eigenvector

Since the commutator is zero, we can write the operator relation:

$$\mathbf{\hat{L}}^2 \mathbf{\hat{L}}_{\pm} - \mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}^2 = 0 \quad \implies \quad \mathbf{\hat{L}}^2 \mathbf{\hat{L}}_{\pm} = \mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}^2$$

Now, apply $\mathbf{\hat{L}}^2$ to the state $\mathbf{\hat{L}}_{\pm}|f\rangle$:

$$\mathbf{\hat{L}}^2 (\mathbf{\hat{L}}_{\pm}|f\rangle) = (\mathbf{\hat{L}}^2 \mathbf{\hat{L}}_{\pm}) |f\rangle$$

Using the commuting property:

$$\mathbf{\hat{L}}^2 (\mathbf{\hat{L}}_{\pm}|f\rangle) = (\mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}^2) |f\rangle$$

Next, substitute the eigenvalue equation for $|f\rangle$: $\mathbf{\hat{L}}^2 |f\rangle = \lambda |f\rangle$:

$$\mathbf{\hat{L}}^2 (\mathbf{\hat{L}}_{\pm}|f\rangle) = \mathbf{\hat{L}}_{\pm} (\mathbf{\hat{L}}^2 |f\rangle)$$

$$\mathbf{\hat{L}}^2 (\mathbf{\hat{L}}_{\pm}|f\rangle) = \mathbf{\hat{L}}_{\pm} (\lambda |f\rangle)$$

Since $\lambda$ is a scalar (the eigenvalue), it can be pulled out:

$$\mathbf{\hat{L}}^2 (\mathbf{\hat{L}}_{\pm}|f\rangle) = \lambda (\mathbf{\hat{L}}_{\pm}|f\rangle)$$

This result shows that when the operator $\mathbf{\hat{L}}^2$ acts on the state $\mathbf{\hat{L}}_{\pm}|f\rangle$, the result is the state itself multiplied by the scalar $\lambda$.

---

## Conclusion

The equation

$$\mathbf{\hat{L}}^2 (\mathbf{\hat{L}}_{\pm}|f\rangle) = \lambda (\mathbf{\hat{L}}_{\pm}|f\rangle)$$

proves that $\mathbf{\hat{L}}_{\pm}|f\rangle$ is an eigenvector of $\mathbf{\hat{L}}^2$ with the eigenvalue $\lambda$, unless the resulting state is the zero vector ($\mathbf{\hat{L}}_{\pm}|f\rangle = 0$), in which case it "vanishes" (verschwindet).