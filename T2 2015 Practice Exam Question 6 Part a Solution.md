

Hello! An excellent question. This is the perfect place to start our study of perturbation theory. The whole idea is to begin with a simple system we _can_ solve (the "unperturbed" case) and then see how its properties (like energy) change when we add a small, complicated part (the "perturbation").

This question, part (a), is all about understanding that simple starting point.

Let's break it down.

### 1. The Hamiltonian at $\lambda = 0$

The problem gives us the full Hamiltonian for the system, which depends on the parameter $\lambda$:

$$\hat{H}_\lambda = \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix} + \lambda \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix}$$

This is in the standard form for perturbation theory, $\hat{H} = \hat{H}_0 + \lambda \hat{V}$.

-   $\hat{H}_0 = \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix}$ is the **unperturbed Hamiltonian**. This describes the simple system we know how to solve.
    
-   $\lambda \hat{V} = \lambda \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix}$ is the **perturbation**. This is the small, complex part. $\lambda$ is a "knob" that we use to turn this perturbation on or off.
    

The question asks us to look at the specific case where **$\lambda = 0$**. This means we are "turning off" the perturbation completely. Let's see what the Hamiltonian becomes:

$$\hat{H}_{\lambda=0} = \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix} + 0 \cdot \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix}$$

$$\hat{H}_{\lambda=0} = \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix}$$

So, for $\lambda = 0$, our system is just described by the simple, unperturbed Hamiltonian $\hat{H}_0$.

---

### 2. Finding the Energies (Eigenvalues)

Now, we need to find the "energies" of this system. In quantum mechanics, the allowed energies of a system are the **eigenvalues** of its Hamiltonian matrix.

We are looking for the eigenvalues of this matrix:

$$\hat{H}_0 = \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix}$$

This is a **diagonal matrix**, which makes our job very easy!

> **Key Concept:** For any diagonal matrix, the eigenvalues are simply the numbers on the main diagonal.

So, just by looking at the matrix, we can immediately see that the eigenvalues (energies) are:

-   $E_1 = a$
    
-   $E_2 = b$
    

This is exactly what the problem asked us to show!

---

### 3. Finding the Eigenfunctions (Eigenstates)

The problem also mentions the "energies of the eigenfunctions" (or eigenstates). Let's quickly find the corresponding eigenstates for these energies. Remember, the problem states we are using the basis $\{|1\rangle, |2\rangle\}$.

In this basis, the basis vectors are represented by:

-   $|1\rangle = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$
    
-   $|2\rangle = \begin{pmatrix} 0 \\ 1 \end{pmatrix}$
    

Let's apply our Hamiltonian $\hat{H}_0$ to these basis states:

-   For state $|1\rangle$:
    
    $$\hat{H}_0 |1\rangle = \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \begin{pmatrix} a \cdot 1 + 0 \cdot 0 \\ 0 \cdot 1 + b \cdot 0 \end{pmatrix} = \begin{pmatrix} a \\ 0 \end{pmatrix} = a \begin{pmatrix} 1 \\ 0 \end{pmatrix} = a |1\rangle$$
    
    This is the very definition of an eigenvalue equation: $\hat{H}_0 |\psi\rangle = E |\psi\rangle$. We see that $|1\rangle$ is the eigenstate (eigenfunction) with energy $E = a$.
    
-   For state $|2\rangle$:
    
    $$\hat{H}_0 |2\rangle = \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \begin{pmatrix} a \cdot 0 + 0 \cdot 1 \\ 0 \cdot 0 + b \cdot 1 \end{pmatrix} = \begin{pmatrix} 0 \\ b \end{pmatrix} = b \begin{pmatrix} 0 \\ 1 \end{pmatrix} = b |2\rangle$$
    
    Similarly, we see that $|2\rangle$ is the eigenstate (eigenfunction) with energy $E = b$.
    

---

### 4. Justifying the Notation

Finally, the question asks why the notation $a = E_1^{(0)}$ and $b = E_2^{(0)}$ is justified.

This is the standard language of perturbation theory:

-   **$E$** stands for energy.
    
-   The **subscript** ($1$ or $2$) labels the quantum state. We just found that state $|1\rangle$ has energy $a$ and state $|2\rangle$ has energy $b$.
    
-   The **superscript $(0)$** (read as "zero" or "zeroth-order") means this is the value for the **unperturbed system**, i.e., the value at $\lambda = 0$.
    

So:

-   $E_1^{(0)}$ means "The zeroth-order energy of the first state." We just showed this is **$a$**.
    
-   $E_2^{(0)}$ means "The zeroth-order energy of the second state." We just showed this is **$b$**.
    

Thus, the notation is perfectly justified. We have successfully found the energies and eigenstates for our "starting" system before we add any perturbation.

I hope that makes everything clear! This unperturbed system is our foundation, and everything else in perturbation theory will be about calculating _corrections_ to these starting energies and states.

Would you like to move on and discuss what happens when we _do_ turn on the perturbation (meaning, when $\lambda$ is small but not zero)?