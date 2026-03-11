

Welcome back! I love the enthusiasm. This is where all the hard work we did in parts 1 and 2 really pays off. You are about to see how beautifully the math clicks together when we use the separation of variables.

Let's translate this third part to get started:

> **3. Determine the eigenvalue $E_{n_x, n_y, n_z}$ for all $|n_x, n_y, n_z\rangle$. Show concretely $\hat{H}|n_x, n_y, n_z\rangle = |n_x, n_y, n_z\rangle E_{n_x, n_y, n_z}$. [3 pts.]**

Let's break down this proof step-by-step.

---

### Step 1: Gathering Our Building Blocks

From our previous discussion, we know that our total 3D Hamiltonian is the sum of three independent 1D Hamiltonians:

$$\hat{H} = \hat{h}_x + \hat{h}_y + \hat{h}_z$$

We also know that our total 3D state is the product of the independent 1D states:

$$|n_x, n_y, n_z\rangle = |n_x\rangle |n_y\rangle |n_z\rangle$$

Before we apply the total Hamiltonian, let's remind ourselves how the individual 1D operators act on their respective states. Remember, an operator acting on its eigenvector gives back the _same_ eigenvector multiplied by a number (the eigenvalue, or energy).

1. **For the x-direction:** From part 1, we know the "stiffness" is $\alpha$, so $\omega_x = \sqrt{\alpha}$.
    
    $$\hat{h}_x |n_x\rangle = E_{n_x} |n_x\rangle \quad \text{where} \quad E_{n_x} = \sqrt{\alpha}\left(n_x + \frac{1}{2}\right)$$
    
2. **For the y-direction:** Looking at the potential $\frac{1}{2}y^2$, the stiffness is 1, so $\omega_y = 1$.
    
    $$\hat{h}_y |n_y\rangle = E_{n_y} |n_y\rangle \quad \text{where} \quad E_{n_y} = 1\left(n_y + \frac{1}{2}\right) = n_y + \frac{1}{2}$$
    
3. **For the z-direction:** Similarly, the potential is $\frac{1}{2}z^2$, so $\omega_z = 1$.
    
    $$\hat{h}_z |n_z\rangle = E_{n_z} |n_z\rangle \quad \text{where} \quad E_{n_z} = 1\left(n_z + \frac{1}{2}\right) = n_z + \frac{1}{2}$$
    

### Step 2: Applying the Total Hamiltonian (The Proof)

Now, let's "show concretely" what happens when the total Hamiltonian acts on the total state vector. We start with the left side of the equation they want us to prove:

$$\hat{H} |n_x, n_y, n_z\rangle$$

Substitute our separated versions of the Hamiltonian and the state:

$$= (\hat{h}_x + \hat{h}_y + \hat{h}_z) (|n_x\rangle |n_y\rangle |n_z\rangle)$$

Now, we distribute. Here is the crucial physical concept: **operators only act on the states of their own dimension.** The operator $\hat{h}_x$ only "sees" $|n_x\rangle$ and treats $|n_y\rangle$ and $|n_z\rangle$ as constants.

$$= (\hat{h}_x |n_x\rangle)|n_y\rangle|n_z\rangle + |n_x\rangle(\hat{h}_y |n_y\rangle)|n_z\rangle + |n_x\rangle|n_y\rangle(\hat{h}_z |n_z\rangle)$$

Now we substitute our eigenvalue equations from Step 1:

$$= (E_{n_x} |n_x\rangle)|n_y\rangle|n_z\rangle + |n_x\rangle(E_{n_y} |n_y\rangle)|n_z\rangle + |n_x\rangle|n_y\rangle(E_{n_z} |n_z\rangle)$$

Because $E_{n_x}$, $E_{n_y}$, and $E_{n_z}$ are just regular numbers (scalars), we can move them around freely and factor them out to the front (or the back!):

$$= (E_{n_x} + E_{n_y} + E_{n_z}) |n_x\rangle |n_y\rangle |n_z\rangle$$

Recombining our product state back into the compact notation $|n_x, n_y, n_z\rangle$, and placing the scalar energy term on the right-hand side to exactly match the format requested by your assignment:

$$= |n_x, n_y, n_z\rangle (E_{n_x} + E_{n_y} + E_{n_z})$$

This proves that the total state is indeed an eigenvector of the total Hamiltonian, and it shows us that the total energy eigenvalue $E_{n_x, n_y, n_z}$ is simply the sum of the individual energies:

$$E_{n_x, n_y, n_z} = E_{n_x} + E_{n_y} + E_{n_z}$$

### Step 3: Determining the Final Energy Expression

To finish the problem, we just need to explicitly write out that total energy eigenvalue $E_{n_x, n_y, n_z}$ by plugging in the 1D energies we found earlier:

$$E_{n_x, n_y, n_z} = \sqrt{\alpha}\left(n_x + \frac{1}{2}\right) + \left(n_y + \frac{1}{2}\right) + \left(n_z + \frac{1}{2}\right)$$

We can clean this up slightly by combining the constants:

$$E_{n_x, n_y, n_z} = \sqrt{\alpha}\left(n_x + \frac{1}{2}\right) + n_y + n_z + 1$$

_(Remember, $n_x, n_y, n_z$ are non-negative integers: $0, 1, 2, \dots$)_

---

And there you have it! You have successfully solved a 3-dimensional anisotropic quantum system.

The next logical step when studying these systems is to look at **degeneracy**—instances where different combinations of quantum numbers $(n_x, n_y, n_z)$ result in the exact same total energy. Would you like to explore what happens to the degeneracy of this system if we were to set $\alpha = 1$ (making it an _isotropic_ oscillator)?