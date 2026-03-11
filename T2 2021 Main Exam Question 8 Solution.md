

Welcome back to my office! You have reached one of the most beautiful and quintessential topics in quantum mechanics: the addition of angular momentum. We are taking two isolated spin-$\frac{1}{2}$ particles and bringing them together to see how their combined "total spin" behaves.

Let's translate the premise to ensure we are completely aligned. The problem sets up the combined Hilbert space (the product space) of two spins, giving us four basis vectors:

$|1\rangle = |\uparrow\uparrow\rangle$

$|2\rangle = |\uparrow\downarrow\rangle$

$|3\rangle = |\downarrow\uparrow\rangle$

$|4\rangle = |\downarrow\downarrow\rangle$

_Note: The notation in the problem $|\frac{1}{2}, \frac{1}{2}\rangle$ implies we are using "natural units" where we set the reduced Planck constant $\hbar = 1$. We will stick to this convention to keep the math clean!_

Let's tackle this step-by-step.

---

### 1. Eigenvalues of the Total z-Component $\hat{S}_z$

**The Physics:** The total spin operator in the z-direction is simply the sum of the operators for each individual particle:

$$\hat{S}_z = \hat{S}_z^{(1)} + \hat{S}_z^{(2)}$$

When this operator acts on a product state, particle 1's operator only acts on the first slot, and particle 2's operator only acts on the second slot.

Let's apply it to our four basis states to find the total $s_z$ eigenvalues:

- $\hat{S}_z |1\rangle = \left(\frac{1}{2} + \frac{1}{2}\right) |\uparrow\uparrow\rangle = 1 |1\rangle \quad \rightarrow \quad s_z = 1$
    
- $\hat{S}_z |2\rangle = \left(\frac{1}{2} - \frac{1}{2}\right) |\uparrow\downarrow\rangle = 0 |2\rangle \quad \rightarrow \quad s_z = 0$
    
- $\hat{S}_z |3\rangle = \left(-\frac{1}{2} + \frac{1}{2}\right) |\downarrow\uparrow\rangle = 0 |3\rangle \quad \rightarrow \quad s_z = 0$
    
- $\hat{S}_z |4\rangle = \left(-\frac{1}{2} - \frac{1}{2}\right) |\downarrow\downarrow\rangle = -1 |4\rangle \quad \rightarrow \quad s_z = -1$
    

**Conclusion for Part 1:** The eigenvalues $s_z$ are $1, 0,$ and $-1$. The eigenvalue **$s_z = 0$ is doubly degenerate** because two different linearly independent states ($|2\rangle$ and $|3\rangle$) share this same eigenvalue.

### 2. Possible Eigenvalues of Total Spin $\hat{S}^2$

**The Physics:** When adding two quantum angular momenta $s_1$ and $s_2$, the total quantum number $s$ can take integer steps from $|s_1 - s_2|$ up to $(s_1 + s_2)$.

Here, $s_1 = \frac{1}{2}$ and $s_2 = \frac{1}{2}$.

- Minimum $s = |\frac{1}{2} - \frac{1}{2}| = 0$
    
- Maximum $s = \frac{1}{2} + \frac{1}{2} = 1$
    
    So, the possible total spin quantum numbers are $s = 0$ and $s = 1$.
    

However, the question specifically asks for the eigenvalues of the operator $\hat{S}^2$, which are given by the formula $s(s+1)$:

- For $s = 0$, the eigenvalue is $0(0+1) = \mathbf{0}$.
    
- For $s = 1$, the eigenvalue is $1(1+1) = \mathbf{2}$.
    

**Conclusion for Part 2:** The possible eigenvalues $s(s+1)$ of the total spin $\hat{S}^2$ are **0 and 2**.

### 3. Using the Commutator $[\hat{S}^2, \hat{S}_z] = 0$

**The Physics:** This is a fantastic mathematical proof that shows us _why_ we don't have to calculate a massive $4 \times 4$ matrix. It proves that states with different $s_z$ values do not mix!

Let's write out what the commutator being zero means:

$$\hat{S}^2\hat{S}_z - \hat{S}_z\hat{S}^2 = 0$$

Now, we "sandwich" this operator equation between the bra $\langle i|$ and the ket $|j\rangle$:

$$\langle i| (\hat{S}^2\hat{S}_z - \hat{S}_z\hat{S}^2) |j\rangle = 0$$

$$\langle i| \hat{S}^2\hat{S}_z |j\rangle - \langle i| \hat{S}_z\hat{S}^2 |j\rangle = 0$$

Because $|i\rangle$ and $|j\rangle$ are eigenstates of $\hat{S}_z$ (as proved in Part 1), we know that $\hat{S}_z |j\rangle = s_{zj} |j\rangle$. Similarly, acting to the left on the bra, $\langle i| \hat{S}_z = \langle i| s_{zi}$. Let's substitute these scalar eigenvalues into our equation:

$$\langle i| \hat{S}^2 (s_{zj} |j\rangle) - (\langle i| s_{zi}) \hat{S}^2 |j\rangle = 0$$

We can pull the scalar constants $s_{zj}$ and $s_{zi}$ out of the inner products:

$$s_{zj} \langle i| \hat{S}^2 |j\rangle - s_{zi} \langle i| \hat{S}^2 |j\rangle = 0$$

$$(s_{zj} - s_{zi}) \langle i| \hat{S}^2 |j\rangle = 0$$

**The logical leap:** The problem premise states that $\langle i|\hat{S}_z|i\rangle \neq \langle j|\hat{S}_z|j\rangle$. This is just a fancy way of saying $s_{zi} \neq s_{zj}$. Because they are not equal, the term $(s_{zj} - s_{zi})$ is _not_ zero. For the overall equation to equal zero, the other term must carry the burden:

**$\langle i| \hat{S}^2 |j\rangle = 0$**

### 4. Calculating the $2 \times 2$ Matrix for the $s_z = 0$ Subspace

Because of our proof in Part 3, we only need to look at how $\hat{S}^2$ mixes states with the _same_ $s_z$. The only degenerate states are $|2\rangle$ and $|3\rangle$. We need to calculate the elements $M_{ij} = \langle i|\hat{S}^2|j\rangle$.

First, let's expand the total spin operator squared using ladder operators ($\hat{S}_+$ and $\hat{S}_-$), which makes it much easier to act on our states:

$$\hat{S}^2 = (\hat{\vec{S}}^{(1)} + \hat{\vec{S}}^{(2)})^2 = (\hat{S}^{(1)})^2 + (\hat{S}^{(2)})^2 + 2\hat{S}_z^{(1)}\hat{S}_z^{(2)} + \hat{S}_+^{(1)}\hat{S}_-^{(2)} + \hat{S}_-^{(1)}\hat{S}_+^{(2)}$$

Let's apply this massive operator to state $|2\rangle = |\uparrow\downarrow\rangle$. Keep in mind that for a single spin-$\frac{1}{2}$ particle, $(\hat{S})^2$ yields $\frac{1}{2}(\frac{1}{2}+1) = \frac{3}{4}$.

- $(\hat{S}^{(1)})^2 |\uparrow\downarrow\rangle = \frac{3}{4} |\uparrow\downarrow\rangle$
    
- $(\hat{S}^{(2)})^2 |\uparrow\downarrow\rangle = \frac{3}{4} |\uparrow\downarrow\rangle$
    
- $2\hat{S}_z^{(1)}\hat{S}_z^{(2)} |\uparrow\downarrow\rangle = 2(\frac{1}{2})(-\frac{1}{2}) |\uparrow\downarrow\rangle = -\frac{1}{2} |\uparrow\downarrow\rangle$
    
- $\hat{S}_+^{(1)}\hat{S}_-^{(2)} |\uparrow\downarrow\rangle = 0$ (You cannot raise an up-spin, and you cannot lower a down-spin).
    
- $\hat{S}_-^{(1)}\hat{S}_+^{(2)} |\uparrow\downarrow\rangle = (|\downarrow\rangle)(|\uparrow\rangle) = |\downarrow\uparrow\rangle = |3\rangle$
    

Adding these pieces together:

$$\hat{S}^2 |2\rangle = \left(\frac{3}{4} + \frac{3}{4} - \frac{1}{2}\right)|2\rangle + |3\rangle = 1|2\rangle + 1|3\rangle$$

By exact symmetry, if we apply it to $|3\rangle = |\downarrow\uparrow\rangle$, we get:

$$\hat{S}^2 |3\rangle = 1|3\rangle + 1|2\rangle$$

Now we construct the matrix elements:

- $M_{22} = \langle 2|\hat{S}^2|2\rangle = \langle 2|(1|2\rangle + 1|3\rangle) = 1$
    
- $M_{23} = \langle 2|\hat{S}^2|3\rangle = \langle 2|(1|3\rangle + 1|2\rangle) = 1$
    
- $M_{32} = \langle 3|\hat{S}^2|2\rangle = \langle 3|(1|2\rangle + 1|3\rangle) = 1$
    
- $M_{33} = \langle 3|\hat{S}^2|3\rangle = \langle 3|(1|3\rangle + 1|2\rangle) = 1$
    

**Conclusion for Part 4:** The matrix is:

$$M = \begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix}$$

### 5. Finding the Normalized Eigenkets (Singlet and Triplet)

To find the new states that have definite total spin $|s, s_z\rangle$, we must find the eigenvectors and eigenvalues of the matrix we just built.

We solve the characteristic equation $\det(M - \lambda I) = 0$:

$$\det\begin{pmatrix} 1-\lambda & 1 \\ 1 & 1-\lambda \end{pmatrix} = (1-\lambda)^2 - 1 = \lambda^2 - 2\lambda = \lambda(\lambda - 2) = 0$$

The eigenvalues are $\lambda = 0$ and $\lambda = 2$. Notice that these perfectly match the $s(s+1)$ values we predicted in Part 2!

**Case 1: $\lambda = 0$ (This corresponds to $s=0, s_z=0$)**

$$\begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix} \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \implies a + b = 0 \implies b = -a$$

To normalize the state, $a^2 + b^2 = 1 \implies 2a^2 = 1 \implies a = \frac{1}{\sqrt{2}}$.

The eigenvector is $\frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ -1 \end{pmatrix}$.

Translated back into our Dirac notation, this is the famous **Singlet state**:

$$|0, 0\rangle = \frac{1}{\sqrt{2}} (|2\rangle - |3\rangle) = \frac{1}{\sqrt{2}} (|\uparrow\downarrow\rangle - |\downarrow\uparrow\rangle)$$

**Case 2: $\lambda = 2$ (This corresponds to $s=1, s_z=0$)**

$$\begin{pmatrix} -1 & 1 \\ 1 & -1 \end{pmatrix} \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \implies -a + b = 0 \implies a = b$$

Normalizing this yields $a = \frac{1}{\sqrt{2}}$.

The eigenvector is $\frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ 1 \end{pmatrix}$.

Translated back, this is the middle state of the **Triplet**:

$$|1, 0\rangle = \frac{1}{\sqrt{2}} (|2\rangle + |3\rangle) = \frac{1}{\sqrt{2}} (|\uparrow\downarrow\rangle + |\downarrow\uparrow\rangle)$$

---

Excellent work following along with this derivation. This matrix diagonalization method is universally how physicists determine the Clebsch-Gordan coefficients for angular momentum!

Would you like to discuss why the singlet state is considered "antisymmetric" and what that implies for the spatial wavefunctions of fermions?