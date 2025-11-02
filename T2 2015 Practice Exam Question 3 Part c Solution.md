

You are absolutely correct! The energy eigenvalues and their degeneracy are the next logical step in analyzing the 3D harmonic oscillator, and they reveal a beautiful structure in quantum mechanics.

This question asks: **"What are the eigenvalues of this system? Are there degenerate eigenvalues? How strong is the degeneracy of the eigenvalues?"**

---

## 💡 Energy Eigenvalues of the 3D Harmonic Oscillator

The **eigenvalues** of the Hamiltonian operator $\hat{H}$ correspond to the **possible total energy levels** of the quantum system.

### 1. The Energy Formula

As established by the separability of the Hamiltonian ($\hat{H} = \hat{H}_x + \hat{H}_y + \hat{H}_z$), the total energy $E$ is the sum of the energies from the three independent 1D harmonic oscillators.

The energy eigenvalues for a single 1D harmonic oscillator (in the $i$-direction) are:

$$E_{n_i} = \hbar \omega \left(n_i + \frac{1}{2}\right), \quad \text{where } n_i = 0, 1, 2, 3, \dots$$

Here, $\hbar$ is the reduced Planck constant, $\omega$ is the angular frequency, and $n_i$ is the quantum number for that dimension.

The total energy eigenvalues for the 3D system are:

$$E_{n_x, n_y, n_z} = E_{n_x} + E_{n_y} + E_{n_z}$$

Substituting the 1D formula:

$$E_{n_x, n_y, n_z} = \hbar \omega \left(n_x + \frac{1}{2}\right) + \hbar \omega \left(n_y + \frac{1}{2}\right) + \hbar \omega \left(n_z + \frac{1}{2}\right)$$

Factoring out $\hbar \omega$:

$$E_{n_x, n_y, n_z} = \hbar \omega \left(n_x + n_y + n_z + \frac{3}{2}\right)$$

### 2. Simplified Notation

It is standard to define the principal quantum number $N$ as the sum of the individual quantum numbers:

$$N = n_x + n_y + n_z, \quad \text{where } N = 0, 1, 2, 3, \dots$$

Using $N$, the energy eigenvalues are simplified to:

$$\mathbf{E_N = \hbar \omega \left(N + \frac{3}{2}\right)}$$

The **zero-point energy** (the minimum possible energy, when $N=0$) is $E_0 = \frac{3}{2}\hbar \omega$.

---

## 🌌 Degeneracy (Entartung)

### 1. Are There Degenerate Eigenvalues?

The answer is a definitive **Yes**. The energy depends _only_ on the total number of quanta, $N = n_x + n_y + n_z$. Any combination of non-negative integers $(n_x, n_y, n_z)$ that sums up to the same $N$ will result in the **same total energy $E_N$**.

**Degeneracy** means that two or more distinct quantum states (defined by different sets of quantum numbers $(n_x, n_y, n_z)$) have the exact same energy eigenvalue.

-   Example: $N=1$
    
    The total energy is $E_1 = \hbar \omega (1 + 3/2) = 5/2 \hbar \omega$.
    
    This energy can be achieved by three different states:
    
    1.  $(n_x, n_y, n_z) = (1, 0, 0)$
        
    2.  $(n_x, n_y, n_z) = (0, 1, 0)$
        
    3.  $(n_x, n_y, n_z) = (0, 0, 1)$
        

Since three distinct states share the same energy, the $N=1$ energy level is **three-fold degenerate**.

### 2. How Strong is the Degeneracy?

The degeneracy $d_N$ is the number of ways (the number of unique sets of non-negative integers $n_x, n_y, n_z$) to satisfy the constraint:

$$n_x + n_y + n_z = N$$

This is a classic combinatorial problem, equivalent to finding the number of solutions to this equation. We can solve this using the **stars and bars** method (or more formally, "combinations with replacement").

To distribute $N$ indistinguishable quanta (stars) into $k=3$ distinguishable "bins" ($x, y, z$ directions), we need $k-1=2$ dividers (bars). The number of ways to arrange $N$ stars and $k-1$ bars is given by the binomial coefficient:

$$d_N = \binom{N + k - 1}{k - 1} \quad \text{with } k=3$$

The degeneracy $d_N$ of the energy level $E_N$ is:

$$\mathbf{d_N = \binom{N + 3 - 1}{3 - 1} = \binom{N + 2}{2}}$$

This can be written in terms of factorials:

$$\mathbf{d_N = \frac{(N+2)!}{2! N!} = \frac{(N+2)(N+1)}{2}}$$

---

## 🔢 Summary and Examples

The table below shows the first few energy levels and their degeneracy:

**N=nx​+ny​+nz​**

**Energy EN​**

**Degeneracy dN​=2(N+2)(N+1)​**

**States (nx​,ny​,nz​)**

**0**

$\frac{3}{2}\hbar \omega$

$\mathbf{d_0 = 1}$

(0, 0, 0)

**1**

$\frac{5}{2}\hbar \omega$

$\mathbf{d_1 = 3}$

(1, 0, 0), (0, 1, 0), (0, 0, 1)

**2**

$\frac{7}{2}\hbar \omega$

$\mathbf{d_2 = 6}$

(2, 0, 0), (0, 2, 0), (0, 0, 2), (1, 1, 0), (1, 0, 1), (0, 1, 1)

**3**

$\frac{9}{2}\hbar \omega$

$\mathbf{d_3 = 10}$

(3, 0, 0) and permutations; (2, 1, 0) and permutations; (1, 1, 1)

### 🚨 Note on "Accidental" Degeneracy

This degeneracy is often called **accidental degeneracy** because it arises from the specific form of the Hamiltonian (the independence of the three dimensions and their identical frequencies $\omega$), rather than from a geometric symmetry like spherical symmetry alone (though the harmonic oscillator _does_ possess a higher, dynamic symmetry that fully explains this degeneracy). The fact that the energy depends only on $N$ is a direct result of the equal frequencies in all three directions.

Would you like to explore the **wave functions** associated with these states, such as the ground state $\psi_{0,0,0}$ and the first excited states $\psi_{1,0,0}$, etc.?