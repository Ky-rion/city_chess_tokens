

This is an excellent question! In part (e), we found that the _average_ position and momentum were both zero. This is like saying a pendulum, on average, is at its center point.

But "average" doesn't tell the whole story. The pendulum is clearly swinging back and forth! The quantities $\langle n | \hat{x}^2 | n \rangle$ and $\langle n | \hat{p}^2 | n \rangle$ measure the _spread_ or _variance_ of the position and momentum. They tell us _how far_ the pendulum swings, on average. We expect these to be non-zero.

Let's calculate them. This will require us to be very careful with the operator algebra.

---

## 📏 Calculation of $\langle n | \hat{x}^2 | n \rangle$ (Position-Squared)

### Step 1: Write down the $\hat{x}^2$ operator

We start with the definition of $\hat{x}$ and square it.

$\hat{x}^2 = \left( \frac{1}{\sqrt{2}}(\hat{a}^\dagger + \hat{a}) \right)^2 = \frac{1}{(\sqrt{2})^2} (\hat{a}^\dagger + \hat{a})(\hat{a}^\dagger + \hat{a})$

$\hat{x}^2 = \frac{1}{2} (\hat{a}^\dagger + \hat{a})(\hat{a}^\dagger + \hat{a})$

### Step 2: Expand the operator (The most important step!)

We must be careful to keep the operator order, since $\hat{a}$ and $\hat{a}^\dagger$ do not commute!

$\hat{x}^2 = \frac{1}{2} \left( \hat{a}^\dagger(\hat{a}^\dagger + \hat{a}) + \hat{a}(\hat{a}^\dagger + \hat{a}) \right)$

$\hat{x}^2 = \frac{1}{2} \left( \hat{a}^\dagger\hat{a}^\dagger + \hat{a}^\dagger\hat{a} + \hat{a}\hat{a}^\dagger + \hat{a}\hat{a} \right)$

### Step 3: Put this into the expectation value

Now we "sandwich" this operator between $\langle n |$ and $| n \rangle$:

$\langle n | \hat{x}^2 | n \rangle = \frac{1}{2} \langle n | \left( \hat{a}^\dagger\hat{a}^\dagger + \hat{a}^\dagger\hat{a} + \hat{a}\hat{a}^\dagger + \hat{a}\hat{a} \right) | n \rangle$

Let's split this into four separate terms:

$= \frac{1}{2} \left( \langle n | \hat{a}^\dagger\hat{a}^\dagger | n \rangle + \langle n | \hat{a}^\dagger\hat{a} | n \rangle + \langle n | \hat{a}\hat{a}^\dagger | n \rangle + \langle n | \hat{a}\hat{a} | n \rangle \right)$

### Step 4: Evaluate each term using our rules from part (c)

-   Term 1: $\langle n | \hat{a}^\dagger\hat{a}^\dagger | n \rangle$
    
    Let's have the $\hat{a}^\dagger$ act on $|n\rangle$ twice:
    
    $\hat{a}^\dagger\hat{a}^\dagger | n \rangle = \hat{a}^\dagger (\sqrt{n+1} |n+1\rangle) = \sqrt{n+1} (\hat{a}^\dagger |n+1\rangle) = \sqrt{n+1} \sqrt{n+2} |n+2\rangle$
    
    So, the expectation value is: $\sqrt{n+1}\sqrt{n+2} \langle n | n+2 \rangle$.
    
    Because the states are orthogonal, $\langle n | n+2 \rangle = 0$. So, Term 1 = 0.
    
-   Term 2: $\langle n | \hat{a}^\dagger\hat{a} | n \rangle$
    
    This is the Number Operator $\hat{N}$!
    
    $\hat{a} | n \rangle = \sqrt{n} |n-1\rangle$
    
    $\hat{a}^\dagger \hat{a} | n \rangle = \hat{a}^\dagger (\sqrt{n} |n-1\rangle) = \sqrt{n} (\hat{a}^\dagger |n-1\rangle) = \sqrt{n} (\sqrt{(n-1)+1} |(n-1)+1\rangle) = \sqrt{n} \sqrt{n} |n\rangle = n |n\rangle$.
    
    So, the expectation value is: $\langle n | n | n \rangle = n \langle n | n \rangle = n(1)$.
    
    Term 2 = $n$.
    
-   Term 3: $\langle n | \hat{a}\hat{a}^\dagger | n \rangle$
    
    We can use the commutator: $\hat{a}\hat{a}^\dagger = \hat{a}^\dagger\hat{a} + 1$.
    
    $\langle n | (\hat{a}^\dagger\hat{a} + 1) | n \rangle = \langle n | \hat{a}^\dagger\hat{a} | n \rangle + \langle n | 1 | n \rangle = n + \langle n | n \rangle = n + 1$.
    
    Term 3 = $n+1$.
    
-   Term 4: $\langle n | \hat{a}\hat{a} | n \rangle$
    
    Let's have $\hat{a}$ act on $|n\rangle$ twice:
    
    $\hat{a} \hat{a} | n \rangle = \hat{a} (\sqrt{n} |n-1\rangle) = \sqrt{n} (\hat{a} |n-1\rangle) = \sqrt{n} \sqrt{n-1} |n-2\rangle$.
    
    So, the expectation value is: $\sqrt{n}\sqrt{n-1} \langle n | n-2 \rangle$.
    
    Because of orthogonality, $\langle n | n-2 \rangle = 0$. So, Term 4 = 0.
    

### Step 5: Sum the results

Let's plug these values back into our equation:

$\langle n | \hat{x}^2 | n \rangle = \frac{1}{2} ( 0 + n + (n+1) + 0 )$

$\langle n | \hat{x}^2 | n \rangle = \frac{1}{2} ( 2n + 1 )$

$\langle n | \hat{x}^2 | n \rangle = n + \frac{1}{2}$

---

## 💨 Calculation of $\langle n | \hat{p}^2 | n \rangle$ (Momentum-Squared)

The process is exactly the same.

### Step 1: Write down the $\hat{p}^2$ operator

$\hat{p}^2 = \left( \frac{i}{\sqrt{2}}(\hat{a}^\dagger - \hat{a}) \right)^2 = \frac{i^2}{(\sqrt{2})^2} (\hat{a}^\dagger - \hat{a})(\hat{a}^\dagger - \hat{a})$

$\hat{p}^2 = \frac{-1}{2} (\hat{a}^\dagger - \hat{a})(\hat{a}^\dagger - \hat{a})$

### Step 2: Expand the operator

$\hat{p}^2 = -\frac{1}{2} \left( \hat{a}^\dagger(\hat{a}^\dagger - \hat{a}) - \hat{a}(\hat{a}^\dagger - \hat{a}) \right)$

$\hat{p}^2 = -\frac{1}{2} \left( \hat{a}^\dagger\hat{a}^\dagger - \hat{a}^\dagger\hat{a} - \hat{a}\hat{a}^\dagger + \hat{a}\hat{a} \right)$

### Step 3: Put this into the expectation value

$\langle n | \hat{p}^2 | n \rangle = -\frac{1}{2} \langle n | \left( \hat{a}^\dagger\hat{a}^\dagger - \hat{a}^\dagger\hat{a} - \hat{a}\hat{a}^\dagger + \hat{a}\hat{a} \right) | n \rangle$

$= -\frac{1}{2} \left( \langle n | \hat{a}^\dagger\hat{a}^\dagger | n \rangle - \langle n | \hat{a}^\dagger\hat{a} | n \rangle - \langle n | \hat{a}\hat{a}^\dagger | n \rangle + \langle n | \hat{a}\hat{a} | n \rangle \right)$

### Step 4: Evaluate each term

We already did all the work! We can just reuse our results from above:

-   Term 1 = 0
    
-   Term 2 = $n$
    
-   Term 3 = $n+1$
    
-   Term 4 = 0
    

### Step 5: Sum the results

Let's be careful with the minus signs:

$\langle n | \hat{p}^2 | n \rangle = -\frac{1}{2} ( 0 - n - (n+1) + 0 )$

$\langle n | \hat{p}^2 | n \rangle = -\frac{1}{2} ( -n - n - 1 )$

$\langle n | \hat{p}^2 | n \rangle = -\frac{1}{2} ( -2n - 1 )$

$\langle n | \hat{p}^2 | n \rangle = n + \frac{1}{2}$

---

## 💡 Conclusion and Meaning

We found that:

-   **$\langle n | \hat{x}^2 | n \rangle = n + \frac{1}{2}$**
    
-   **$\langle n | \hat{p}^2 | n \rangle = n + \frac{1}{2}$**
    

This is a beautiful and symmetric result! It tells us that the "spread" of the particle's position and momentum are equal for any energy level $n$.

It also shows that as the energy $E_n = (n+\frac{1}{2})$ increases, the particle becomes "more spread out" in both position and momentum. This makes sense: a pendulum with more energy swings further ($x$ has a larger spread) and moves faster ($p$ has a larger spread).

This result is also a perfect demonstration of the **Heisenberg Uncertainty Principle**.

-   The uncertainty in $x$ is $\Delta x = \sqrt{\langle \hat{x}^2 \rangle - \langle \hat{x} \rangle^2} = \sqrt{(n+\frac{1}{2}) - 0^2} = \sqrt{n+\frac{1}{2}}$.
    
-   The uncertainty in $p$ is $\Delta p = \sqrt{\langle \hat{p}^2 \rangle - \langle \hat{p} \rangle^2} = \sqrt{(n+\frac{1}{2}) - 0^2} = \sqrt{n+\frac{1}{2}}$.
    
-   The uncertainty product is $\Delta x \Delta p = (n + \frac{1}{2})$.
    
-   The general principle states $\Delta x \Delta p \ge \frac{1}{2} | \langle [\hat{x}, \hat{p}] \rangle |$. From part (d), we know $[\hat{x}, \hat{p}] = i$, so $\Delta x \Delta p \ge \frac{1}{2}$.
    
-   Our result $\Delta x \Delta p = (n + \frac{1}{2})$ clearly obeys this for all $n \ge 0$. The lowest possible uncertainty is for the ground state ($n=0$), where $\Delta x \Delta p = \frac{1}{2}$, which is the absolute minimum allowed by quantum mechanics!
    

This is the last part of the problem set I have. Would you like to review any of these concepts, or perhaps discuss the connection to the physical pendulum?