

This is part (e) of the quantum mechanics problem, asking you to prove the identity relating the total angular momentum squared operator ($\mathbf{\hat{L}}^2$) to the ladder operators ($\mathbf{\hat{L}}_{\pm}$) and the $\mathbf{\hat{L}}_z$ operator:

$$\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} + \mathbf{\hat{L}}_z^2 + \hbar \mathbf{\hat{L}}_z$$

or equivalently,

$$\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} + \mathbf{\hat{L}}_z^2 - \hbar \mathbf{\hat{L}}_z$$

_Note: The question states $\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}_{\mp} + \mathbf{\hat{L}}_z^2 \pm \hbar \mathbf{\hat{L}}_z$. Since $\mathbf{\hat{L}}_{\pm} \mathbf{\hat{L}}_{\mp}$ is ambiguous, we'll derive both forms involving the product $\mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-}$ and $\mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+}$. The structure of the identity is key to finding the relationship between $\lambda$ and $\mu_{\text{max}}$._

---

## 1. Definitions and Commutation Relations

We start with the definitions of the operators:

-   **Total Angular Momentum Squared:** $\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 + \mathbf{\hat{L}}_z^2$
    
-   **Ladder Operators:** $\mathbf{\hat{L}}_{\pm} = \mathbf{\hat{L}}_x \pm i \mathbf{\hat{L}}_y$
    

We need the product of the ladder operators, $\mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+}$ and $\mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-}$.

---

## 2. Deriving $\mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+}$

$$\begin{aligned} \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} &= (\mathbf{\hat{L}}_x - i \mathbf{\hat{L}}_y)(\mathbf{\hat{L}}_x + i \mathbf{\hat{L}}_y) \\ &= \mathbf{\hat{L}}_x^2 + i \mathbf{\hat{L}}_x \mathbf{\hat{L}}_y - i \mathbf{\hat{L}}_y \mathbf{\hat{L}}_x - i^2 \mathbf{\hat{L}}_y^2 \\ &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 + i (\mathbf{\hat{L}}_x \mathbf{\hat{L}}_y - \mathbf{\hat{L}}_y \mathbf{\hat{L}}_x) \\ &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 + i [\mathbf{\hat{L}}_x, \mathbf{\hat{L}}_y] \end{aligned}$$

Using the fundamental commutation relation $[\mathbf{\hat{L}}_x, \mathbf{\hat{L}}_y] = i \hbar \mathbf{\hat{L}}_z$:

$$\begin{aligned} \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 + i (i \hbar \mathbf{\hat{L}}_z) \\ &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 - \hbar \mathbf{\hat{L}}_z \quad \text{(since } i^2 = -1) \end{aligned}$$

We know $\mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 = \mathbf{\hat{L}}^2 - \mathbf{\hat{L}}_z^2$. Substituting this into the equation:

$$\begin{aligned} \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} &= (\mathbf{\hat{L}}^2 - \mathbf{\hat{L}}_z^2) - \hbar \mathbf{\hat{L}}_z \\ \implies \mathbf{\hat{L}}^2 &= \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} + \mathbf{\hat{L}}_z^2 + \hbar \mathbf{\hat{L}}_z \end{aligned}$$

This completes the first part of the proof (for the identity involving $\mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+}$).

---

## 3. Deriving $\mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-}$

$$\begin{aligned} \mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} &= (\mathbf{\hat{L}}_x + i \mathbf{\hat{L}}_y)(\mathbf{\hat{L}}_x - i \mathbf{\hat{L}}_y) \\ &= \mathbf{\hat{L}}_x^2 - i \mathbf{\hat{L}}_x \mathbf{\hat{L}}_y + i \mathbf{\hat{L}}_y \mathbf{\hat{L}}_x - i^2 \mathbf{\hat{L}}_y^2 \\ &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 - i (\mathbf{\hat{L}}_x \mathbf{\hat{L}}_y - \mathbf{\hat{L}}_y \mathbf{\hat{L}}_x) \\ &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 - i [\mathbf{\hat{L}}_x, \mathbf{\hat{L}}_y] \end{aligned}$$

Substituting $[\mathbf{\hat{L}}_x, \mathbf{\hat{L}}_y] = i \hbar \mathbf{\hat{L}}_z$:

$$\begin{aligned} \mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 - i (i \hbar \mathbf{\hat{L}}_z) \\ &= \mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 + \hbar \mathbf{\hat{L}}_z \end{aligned}$$

Substituting $\mathbf{\hat{L}}_x^2 + \mathbf{\hat{L}}_y^2 = \mathbf{\hat{L}}^2 - \mathbf{\hat{L}}_z^2$:

$$\begin{aligned} \mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} &= (\mathbf{\hat{L}}^2 - \mathbf{\hat{L}}_z^2) + \hbar \mathbf{\hat{L}}_z \\ \implies \mathbf{\hat{L}}^2 &= \mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} + \mathbf{\hat{L}}_z^2 - \hbar \mathbf{\hat{L}}_z \end{aligned}$$

---

## Conclusion

We have successfully shown the two forms of the identity, both of which are useful in solving the angular momentum eigenvalue problem:

1.  $$\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_{-} \mathbf{\hat{L}}_{+} + \mathbf{\hat{L}}_z^2 + \hbar \mathbf{\hat{L}}_z$$
    
2.  $$\mathbf{\hat{L}}^2 = \mathbf{\hat{L}}_{+} \mathbf{\hat{L}}_{-} + \mathbf{\hat{L}}_z^2 - \hbar \mathbf{\hat{L}}_z$$