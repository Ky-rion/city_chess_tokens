

This is a fantastic question! In parts (a) and (b), we figured out _what kind_ of state $\hat{a}^\dagger|n\rangle$ and $\hat{a}|n\rangle$ are (they are eigenstates). Now, we're going to find out _exactly_ what they are, including the precise numerical factor in front.

This requires us to use a new piece of information that was given in the problem statement: the states $\{|n\rangle\}$ are **orthonormal**. This is a compact way of saying two things:

1.  **Ortho- (Orthogonal):** Any two _different_ energy states are totally independent. The "overlap" between them is zero. $\langle m | n \rangle = 0$ if $m \neq n$.
    
2.  **-Normal (Normalized):** Each state vector has a "length" of 1. $\langle n | n \rangle = 1$.
    

We can combine these two facts into a single powerful equation using the Kronecker delta, $\delta_{mn}$:

$\langle m | n \rangle = \delta_{mn}$

(This is 1 if $m=n$, and 0 otherwise).

We will use this property to find the unknown constants.

---

### 1. Proof for the Creation Operator ($\hat{a}^\dagger$)

**Goal:** Show that $\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$.

#### Step 1: Relate the States

From part (a), we proved that $\hat{H}(\hat{a}^\dagger|n\rangle) = (n+1+\frac{1}{2})(\hat{a}^\dagger|n\rangle)$.

This means that the state $\hat{a}^\dagger|n\rangle$ is the eigenstate of $\hat{H}$ with energy $E_{n+1}$.

From Equation (8), we know that the _normalized_ eigenstate with this energy is called $|n+1\rangle$.

Since $\hat{a}^\dagger|n\rangle$ and $|n+1\rangle$ are both eigenstates with the _same energy_, they must describe the same physical state. This means they can only differ by a constant numerical factor. Let's call this constant $c_n$:

$\hat{a}^\dagger|n\rangle = c_n |n+1\rangle$

Our goal is to prove that $c_n = \sqrt{n+1}$.

#### Step 2: Use Normalization to Find $c_n$

The easiest way to find $c_n$ is to calculate the "squared norm" (or length-squared) of both sides of this equation. By convention, we'll choose $c_n$ to be a positive real number.

Let's look at the squared norm of the right side first, as it's simpler.

-   Norm of the Right Hand Side (RHS):
    
    The squared norm of $c_n|n+1\rangle$ is found by multiplying its "bra" by its "ket":
    
    $\left( c_n^* \langle n+1 | \right) \left( c_n |n+1\rangle \right) = |c_n|^2 \langle n+1 | n+1 \rangle$
    
    Since $|n+1\rangle$ is normalized, $\langle n+1 | n+1 \rangle = 1$.
    
    So, the squared norm of the RHS is just $|c_n|^2$.
    
-   Norm of the Left Hand Side (LHS):
    
    The squared norm of $\hat{a}^\dagger|n\rangle$ is $\left( \langle n | \hat{a} \right) \left( \hat{a}^\dagger | n \rangle \right) = \langle n | \hat{a} \hat{a}^\dagger | n \rangle$.
    
    (Remember: to turn the ket $|\psi\rangle = \hat{a}^\dagger|n\rangle$ into the bra $\langle \psi |$, you take the "Hermitian conjugate" ($\dagger$) of the whole thing, which reverses the order and daggers each part: $(\hat{a}^\dagger|n\rangle)^\dagger = \langle n | (\hat{a}^\dagger)^\dagger = \langle n | \hat{a}$.)
    

#### Step 3: Solve for the LHS Norm

We need to figure out what $\langle n | \hat{a} \hat{a}^\dagger | n \rangle$ is.

We can use our commutator from Equation (7): $[\hat{a}, \hat{a}^\dagger] = 1$, which means $\hat{a}\hat{a}^\dagger - \hat{a}^\dagger\hat{a} = 1$.

Let's rearrange this to solve for the operator we have, $\hat{a}\hat{a}^\dagger$:

$\hat{a}\hat{a}^\dagger = 1 + \hat{a}^\dagger\hat{a}$

Now, substitute this into our LHS expression:

$\langle n | \hat{a} \hat{a}^\dagger | n \rangle = \langle n | \left( 1 + \hat{a}^\dagger\hat{a} \right) | n \rangle$

We can split this into two parts:

$= \langle n | 1 | n \rangle + \langle n | \hat{a}^\dagger\hat{a} | n \rangle$

$= \langle n | n \rangle + \langle n | \hat{a}^\dagger\hat{a} | n \rangle$

The first part is easy: $\langle n | n \rangle = 1$ (by normalization).

For the second part, $\langle n | \hat{a}^\dagger\hat{a} | n \rangle$, we use the Hamiltonian from Equation (6):

$\hat{H} = \hat{a}^\dagger \hat{a} + \frac{1}{2} \implies \hat{a}^\dagger \hat{a} = \hat{H} - \frac{1}{2}$

Let's plug this in:

$\langle n | \hat{a}^\dagger\hat{a} | n \rangle = \langle n | \left( \hat{H} - \frac{1}{2} \right) | n \rangle$

$= \langle n | \hat{H} | n \rangle - \langle n | \frac{1}{2} | n \rangle$

$= \langle n | \hat{H} | n \rangle - \frac{1}{2} \langle n | n \rangle$

Now we use Equation (8): $\hat{H}|n\rangle = (n+\frac{1}{2})|n\rangle$.

$= \langle n | \left( (n+\frac{1}{2})|n\rangle \right) - \frac{1}{2} (1)$

$= (n+\frac{1}{2}) \langle n | n \rangle - \frac{1}{2}$

$= (n+\frac{1}{2})(1) - \frac{1}{2} = n$

So, the second part $\langle n | \hat{a}^\dagger\hat{a} | n \rangle$ is just **$n$**.

Let's go back to our full LHS expression:

$\langle n | \hat{a} \hat{a}^\dagger | n \rangle = \langle n | n \rangle + \langle n | \hat{a}^\dagger\hat{a} | n \rangle = 1 + n$

#### Step 4: Final Result

We have now shown:

-   Squared norm of RHS = $|c_n|^2$
    
-   Squared norm of LHS = $n+1$
    

Equating them gives:

$|c_n|^2 = n + 1 \implies c_n = \sqrt{n+1}$ (by convention, we pick the positive real root)

Therefore, we have proven:

$\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$

---

### 2. Proof for the Annihilation Operator ($\hat{a}$)

**Goal:** Show that $\hat{a}|n\rangle = \sqrt{n}|n-1\rangle$.

This proof is even faster because we can reuse our work.

#### Step 1: Relate the States

From part (b), we know $\hat{a}|n\rangle$ is the eigenstate with energy $E_{n-1}$. The normalized state with this energy is $|n-1\rangle$.

So, they must be proportional by a constant, let's call it $d_n$:

$\hat{a}|n\rangle = d_n |n-1\rangle$

#### Step 2: Use Normalization

We find the squared norm of both sides.

-   **Norm of RHS:** $\left( d_n^* \langle n-1 | \right) \left( d_n |n-1\rangle \right) = |d_n|^2 \langle n-1 | n-1 \rangle =$ $|d_n|^2$
    
-   **Norm of LHS:** $\left( \langle n | \hat{a}^\dagger \right) \left( \hat{a} | n \rangle \right) =$ **$\langle n | \hat{a}^\dagger \hat{a} | n \rangle$**
    

#### Step 3: Solve for the LHS Norm

We already solved this! In Step 3 of the first proof, we proved that:

$\langle n | \hat{a}^\dagger \hat{a} | n \rangle = n$

> (This operator, $\hat{N} = \hat{a}^\dagger \hat{a}$, is so important it has its own name: the **Number Operator**. When it acts on an energy state $|n\rangle$, its eigenvalue is just the number $n$ itself. This is why we call $|n\rangle$ the "n-th" state.)

#### Step 4: Final Result

Equating the squared norms of the LHS and RHS:

$|d_n|^2 = n \implies d_n = \sqrt{n}$


Therefore, we have proven:

$\hat{a}|n\rangle = \sqrt{n}|n-1\rangle$

This completes the proof and gives us the exact "ladder rules" for moving up and down the energy states.

Would you like to try using these new rules to calculate something, for example, the expectation value $\langle n | \hat{x} | n \rangle$ (which requires knowing how to write $\hat{x}$ in terms of $\hat{a}$ and $\hat{a}^\dagger$)?