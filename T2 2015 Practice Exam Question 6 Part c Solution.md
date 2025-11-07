

You've got it! This is the heart of perturbation theory.

In parts (a) and (b), we did two extremes:

-   **(a) $\lambda = 0$:** We found the "zeroth-order" energies, $E_1^{(0)} = a$ and $E_2^{(0)} = b$.
    
-   **(b) Exact Solution:** We found the exact, complicated formula for _any_ $\lambda$.
    

Now, in part (c), we'll do what perturbation theory is designed for: find an **approximation** that is much simpler than the exact solution but more accurate than the zeroth-order one.

We are looking for the "first-order approximation," which means we want to find the energy as a power series in $\lambda$ and keep only the terms up to the _first power_ of $\lambda$.

The energy $E_n$ for a state $n$ is written as:

$$E_n \approx E_n^{(0)} + \lambda E_n^{(1)}$$

-   $E_n^{(0)}$ is the **zeroth-order energy** (which we already found in part a!).
    
-   $E_n^{(1)}$ is the **first-order energy correction**.
    

---

### 1. The Formula for the First-Order Correction

For a system where the unperturbed energies are different (we assume $a \neq b$, which is called the **non-degenerate** case), the first-order correction to the energy $E_n$ is given by a wonderfully simple formula:

$$E_n^{(1)} = \langle n^{(0)} | \hat{V} | n^{(0)} \rangle$$

Let's unpack this:

-   $\hat{V}$ is the perturbation part of the Hamiltonian. From our problem, $\hat{H}_\lambda = \hat{H}_0 + \lambda \hat{V}$, so:
    
    $$\hat{V} = \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix}$$
    
-   $|n^{(0)}\rangle$ is the **unperturbed eigenstate** corresponding to the energy $E_n^{(0)}$.
    
-   $\langle n^{(0)} |$ is the "bra" vector, which is the conjugate transpose of the "ket" vector $|n^{(0)}\rangle$.
    

This formula tells us that the first-order _shift_ in energy is just the **expectation value of the perturbation** in the _unperturbed_ state. It's how much the original, simple state "feels" the perturbation, on average.

---

### 2. Identifying Our States and Energies

From part (a), we have our two unperturbed states and their energies:

-   **State 1:**
    
    -   Energy: $E_1^{(0)} = a$
        
    -   Eigenstate: $|1^{(0)}\rangle = |1\rangle = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$
        
    -   Bra vector: $\langle 1^{(0)} | = \begin{pmatrix} 1 & 0 \end{pmatrix}$
        
-   **State 2:**
    
    -   Energy: $E_2^{(0)} = b$
        
    -   Eigenstate: $|2^{(0)}\rangle = |2\rangle = \begin{pmatrix} 0 \\ 1 \end{pmatrix}$
        
    -   Bra vector: $\langle 2^{(0)} | = \begin{pmatrix} 0 & 1 \end{pmatrix}$
        

---

### 3. Calculating the First-Order Correction for $E_1$

Let's find $E_1^{(1)}$ using our formula:

$$E_1^{(1)} = \langle 1^{(0)} | \hat{V} | 1^{(0)} \rangle = \begin{pmatrix} 1 & 0 \end{pmatrix} \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix}$$

Let's do the matrix multiplication from right to left:

1.  First, the matrix times the ket vector:
    
    $$\begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \begin{pmatrix} (D_1 \cdot 1) + (C^* \cdot 0) \\ (C \cdot 1) + (D_2 \cdot 0) \end{pmatrix} = \begin{pmatrix} D_1 \\ C \end{pmatrix}$$
    
2.  Now, multiply the bra vector by that result:
    
    $$\begin{pmatrix} 1 & 0 \end{pmatrix} \begin{pmatrix} D_1 \\ C \end{pmatrix} = (1 \cdot D_1) + (0 \cdot C) = D_1$$
    

So, the first-order correction is simply **$E_1^{(1)} = D_1$**.

---

### 4. Calculating the First-Order Correction for $E_2$

Now we do the same for the second state:

$$E_2^{(1)} = \langle 2^{(0)} | \hat{V} | 2^{(0)} \rangle = \begin{pmatrix} 0 & 1 \end{pmatrix} \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix}$$

Again, from right to left:

1.  First, the matrix times the ket vector:
    
    $$\begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \begin{pmatrix} (D_1 \cdot 0) + (C^* \cdot 1) \\ (C \cdot 0) + (D_2 \cdot 1) \end{pmatrix} = \begin{pmatrix} C^* \\ D_2 \end{pmatrix}$$
    
2.  Now, multiply the bra vector by that result:
    
    $$\begin{pmatrix} 0 & 1 \end{pmatrix} \begin{pmatrix} C^* \\ D_2 \end{pmatrix} = (0 \cdot C^*) + (1 \cdot D_2) = D_2$$
    

So, the second correction is **$E_2^{(1)} = D_2$**.

---

### 5. Final Answer: The Approximate Eigenvalues

We now assemble our final answer by plugging these corrections back into the approximation $E_n \approx E_n^{(0)} + \lambda E_n^{(1)}$.

-   Approximate Eigenvalue 1:
    
    $$E_1(\lambda) \approx E_1^{(0)} + \lambda E_1^{(1)} = a + \lambda D_1$$
    
-   Approximate Eigenvalue 2:
    
    $$E_2(\lambda) \approx E_2^{(0)} + \lambda E_2^{(1)} = b + \lambda D_2$$
    

And that's it! Notice how simple this is. We didn't have to solve any quadratic equations or deal with any square roots. We just had to multiply our original, simple states against the perturbation matrix.

This is the power of perturbation theory. For a small $\lambda$, these simple linear formulas, $a + \lambda D_1$ and $b + \lambda D_2$, are an excellent approximation of the complicated exact solution we found in part (b).

The next step in perturbation theory is often to find the _second_-order correction (the $\lambda^2$ term) or to find the _first-order correction to the eigenstates_ (how the states $|1\rangle$ and $|2\rangle$ themselves change).

Would you like to discuss the second-order corrections to the energy?