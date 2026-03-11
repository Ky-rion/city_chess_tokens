

Welcome to theoretical physics! It is fantastic to have a curious student eager to dive into the beautiful machinery of quantum mechanics. Angular momentum is one of the most elegant and foundational topics we cover, so you are in for a treat.

First, let's translate the German text from your assignment:

- **"Drehimpulsalgebra"** translates to **"Angular Momentum Algebra"**.
    
- **"Zeigen Sie, dass $\langle \hat{L}^2 \rangle \ge 0$"** translates to **"Show that the expectation value of $\hat{L}^2$ is greater than or equal to 0."**
    

Let's break down the proof step-by-step. Don't worry if this is your first time seeing it; we will rely purely on the fundamental axioms of quantum mechanics.

### 1. Understanding the Operator

In quantum mechanics, $\hat{L}^2$ is the operator representing the square of the total orbital angular momentum. Just like in classical mechanics where the magnitude squared of a vector $\vec{L}$ is $L^2 = L_x^2 + L_y^2 + L_z^2$, the quantum mechanical operator is defined by its components:

$$\hat{L}^2 = \hat{L}_x^2 + \hat{L}_y^2 + \hat{L}_z^2$$

Here, $\hat{L}_x$, $\hat{L}_y$, and $\hat{L}_z$ are the operators for the angular momentum projected along the $x$, $y$, and $z$ axes, respectively.

### 2. Setting Up the Expectation Value

The notation $\langle \hat{L}^2 \rangle$ represents the "expectation value" (the average measurable value) of the operator in some arbitrary quantum state, which we will call $|\psi\rangle$.

Using Dirac (bra-ket) notation, we write this as:

$$\langle \hat{L}^2 \rangle = \langle \psi | \hat{L}^2 | \psi \rangle$$

Now, substitute our definition from Step 1 into this expression:

$$\langle \psi | \hat{L}^2 | \psi \rangle = \langle \psi | (\hat{L}_x^2 + \hat{L}_y^2 + \hat{L}_z^2) | \psi \rangle$$

Because the inner product is linear, we can split this into three separate terms:

$$\langle \hat{L}^2 \rangle = \langle \psi | \hat{L}_x^2 | \psi \rangle + \langle \psi | \hat{L}_y^2 | \psi \rangle + \langle \psi | \hat{L}_z^2 | \psi \rangle$$

### 3. The Power of Hermiticity

This is where the physics comes in! In quantum mechanics, any operator that represents a physical, measurable quantity (an _observable_) must be **Hermitian**. Since we can physically measure the $x$, $y$, and $z$ components of angular momentum, the operators $\hat{L}_x$, $\hat{L}_y$, and $\hat{L}_z$ are Hermitian.

Mathematically, a Hermitian operator is equal to its own adjoint (or conjugate transpose):

$$\hat{L}_i^\dagger = \hat{L}_i$$

_(where $i$ can be $x$, $y$, or $z$)_

Let's look at just one of our expectation value terms, for example, the $x$-component: $\langle \psi | \hat{L}_x^2 | \psi \rangle$. We can rewrite $\hat{L}_x^2$ as $\hat{L}_x \hat{L}_x$:

$$\langle \psi | \hat{L}_x \hat{L}_x | \psi \rangle$$

Because $\hat{L}_x$ is Hermitian ($\hat{L}_x = \hat{L}_x^\dagger$), we can apply the adjoint of the first $\hat{L}_x$ operator to act on the "bra" $\langle \psi |$ instead of the "ket" $| \psi \rangle$:

$$\langle \psi | \hat{L}_x \hat{L}_x | \psi \rangle = \langle \hat{L}_x \psi | \hat{L}_x \psi \rangle$$

### 4. The Norm of a State

Now, let's define a new state vector $|\phi_x\rangle = \hat{L}_x | \psi \rangle$.

Our expression $\langle \hat{L}_x \psi | \hat{L}_x \psi \rangle$ is exactly the inner product of the state $|\phi_x\rangle$ with itself:

$$\langle \phi_x | \phi_x \rangle$$

By the foundational rules of linear algebra and quantum mechanics, the inner product of _any_ state vector with itself gives the square of its norm (its "length"), which must always be a real, non-negative number:

$$\langle \phi_x | \phi_x \rangle \ge 0$$

Therefore, we have proven that:

$$\langle \psi | \hat{L}_x^2 | \psi \rangle \ge 0$$

### 5. Conclusion

Since the exact same logic applies perfectly to the $y$ and $z$ components, we know that:

- $\langle \psi | \hat{L}_x^2 | \psi \rangle \ge 0$
    
- $\langle \psi | \hat{L}_y^2 | \psi \rangle \ge 0$
    
- $\langle \psi | \hat{L}_z^2 | \psi \rangle \ge 0$
    

Summing three numbers that are greater than or equal to zero must yield a result that is also greater than or equal to zero.

Thus, we arrive at our final proof:

$$\langle \hat{L}^2 \rangle \ge 0$$

---

Would you like me to walk you through how we use this algebraic foundation to find the actual eigenvalues, $l(l+1)\hbar^2$, using ladder operators?