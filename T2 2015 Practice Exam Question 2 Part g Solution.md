

This is part (g) of the problem. You need to **argue** that the minimum $\mathbf{\hat{L}}_z$ eigenvalue factor, $\tilde{l}$, must be equal to $-l$ (where $\hbar l$ is the maximum eigenvalue), and subsequently confirm the total angular momentum eigenvalue $\lambda = \hbar^2 l(l+1)$.

## 1. Relate Maximum and Minimum Eigenvalues

From part (f), we established the relationship between the highest $\mathbf{\hat{L}}_z$ factor ($l$) and the lowest $\mathbf{\hat{L}}_z$ factor ($\tilde{l}$):

$$l(l + 1) = \tilde{l}(\tilde{l} - 1)$$

To solve for $\tilde{l}$, we treat this as a quadratic equation in $\tilde{l}$:

$$l^2 + l = \tilde{l}^2 - \tilde{l}$$

$$\tilde{l}^2 - \tilde{l} - (l^2 + l) = 0$$

We can find the roots of this equation by factoring. Notice that if we set $\tilde{l} = -l$, we get:

$$(-l)^2 - (-l) - (l^2 + l) = l^2 + l - l^2 - l = 0$$

So, $\tilde{l} = -l$ is one solution.

Alternatively, notice that if we set $\tilde{l} = l+1$, we get:

$$(l+1)^2 - (l+1) - (l^2+l) = (l^2+2l+1) - l - 1 - l^2 - l = 0$$

So, $\tilde{l} = l+1$ is the other solution.

The two mathematical solutions for $\tilde{l}$ are:

$$\tilde{l} = -l \quad \text{and} \quad \tilde{l} = l+1$$

## 2. Physical Argument

We now use the physical constraints established by the ladder operator formalism to choose the correct solution:

1.  **$l$ is the factor for the maximum eigenvalue:** $\mu_{\text{max}} = \hbar l$.
    
2.  **$\tilde{l}$ is the factor for the minimum eigenvalue:** $\mu_{\text{min}} = \hbar \tilde{l}$.
    

Since $\mu_{\text{max}}$ must be greater than or equal to $\mu_{\text{min}}$, we must have:

$$l \ge \tilde{l}$$

We test the two mathematical solutions against this physical constraint:

-   Solution 1: $\tilde{l} = l+1$
    
    If $\tilde{l} = l+1$, then $l < l+1$. This means the minimum eigenvalue factor is greater than the maximum eigenvalue factor, which is physically impossible.
    
-   Solution 2: $\tilde{l} = -l$
    
    Since $\mathbf{\hat{L}}_z^2 \le \mathbf{\hat{L}}^2$ (from part (d)), the $\mathbf{\hat{L}}_z$ eigenvalues must be symmetric around zero, with $l \ge 0$. In the case where $\tilde{l} = -l$, the minimum eigenvalue factor is $-l$, and $l \ge -l$ is always true for $l \ge 0$. This solution is physically required for the $\mathbf{\hat{L}}_z$ spectrum to be bounded by the total angular momentum.
    

Therefore, we conclude that the only physically allowed solution is:

$$\mathbf{\tilde{l} = -l}$$

## 3. Final Conclusion on $\lambda$

Now that we have confirmed $\tilde{l} = -l$, we substitute this back into the expression for the total angular momentum eigenvalue $\lambda$ found in part (f):

$$\lambda = \hbar^2 l (l + 1)$$

This confirms the standard result for the eigenvalue of the total angular momentum squared operator $\mathbf{\hat{L}}^2$:

$$\mathbf{\hat{L}}^2 |l, m\rangle = \hbar^2 l(l+1) |l, m\rangle$$

where $l$ is a non-negative integer or half-integer, and the possible $\mathbf{\hat{L}}_z$ eigenvalues span from $-\hbar l$ to $+\hbar l$ in steps of $\hbar$.