

Excellent! Let's dive right into the next part. Moving from one dimension to three dimensions is a massive leap in quantum mechanics, but you will see that a very elegant mathematical trick makes it quite manageable. It is completely normal if this equation looks intimidating at first, but we will break it down together.

First, let's translate the text to be absolutely sure we are on the same page.

> **2. Consider now the anisotropic HO in 3 dimensions with the Hamiltonian [2 pts.]** >
> 
> $$\hat{H} = -\frac{1}{2}\Delta + \frac{\alpha x^2 + y^2 + z^2}{2}$$
> 
> **Express the eigenvectors $|n_x, n_y, n_z\rangle$ using the eigenvectors $|n_i\rangle, i = x, y, z$ of the 1-dimensional HOs in the x, y, and z-directions.**

Here is the step-by-step breakdown of how to tackle this.

---

### Step 1: Understanding the "Anisotropic" 3D Hamiltonian

Let's look at the Hamiltonian operator ($\hat{H}$) they gave us.

The triangle symbol $\Delta$ is called the **Laplace operator** (or Laplacian). In three dimensions, it is simply the sum of the second derivatives for all three spatial directions:

$$\Delta = \frac{\partial^2}{\partial x^2} + \frac{\partial^2}{\partial y^2} + \frac{\partial^2}{\partial z^2}$$

If we substitute this back into the Hamiltonian and expand the potential energy fraction, we get:

$$\hat{H} = -\frac{1}{2} \left( \frac{\partial^2}{\partial x^2} + \frac{\partial^2}{\partial y^2} + \frac{\partial^2}{\partial z^2} \right) + \frac{\alpha}{2}x^2 + \frac{1}{2}y^2 + \frac{1}{2}z^2$$

The word **anisotropic** just means "not the same in all directions." Look closely at the potential energy terms. The $y$ and $z$ directions have standard terms ($\frac{1}{2}y^2$ and $\frac{1}{2}z^2$), meaning those "springs" have a stiffness of 1. But the $x$ direction has an $\alpha$ attached to it ($\frac{\alpha}{2}x^2$). The oscillator behaves differently along the x-axis than it does along the y or z axes!

### Step 2: Separation of Variables

Here is the most beautiful trick in introductory quantum mechanics. Because there are no mixed terms in our Hamiltonian (like an $xy$ or $yz$ term), we can completely separate the variables.

We can rearrange the Hamiltonian into three totally independent 1D Hamiltonians grouped by their coordinate:

$$\hat{H} = \left( -\frac{1}{2}\frac{\partial^2}{\partial x^2} + \frac{\alpha}{2}x^2 \right) + \left( -\frac{1}{2}\frac{\partial^2}{\partial y^2} + \frac{1}{2}y^2 \right) + \left( -\frac{1}{2}\frac{\partial^2}{\partial z^2} + \frac{1}{2}z^2 \right)$$

Let's name these individual pieces $\hat{h}_x$, $\hat{h}_y$, and $\hat{h}_z$. Notice that $\hat{h}_x$ is exactly the 1D Hamiltonian you solved in the first question!

So, our 3D system is simply the sum of three independent 1D systems:

$$\hat{H} = \hat{h}_x + \hat{h}_y + \hat{h}_z$$

### Step 3: Expressing the Eigenvectors

In quantum mechanics, the state of a system is represented by a vector inside a specific kind of mathematical space called a Hilbert space. We write these vectors inside "kets," which look like this: $|\text{state}\rangle$. This is called Dirac notation.

The problem asks us to express the total 3D state $|n_x, n_y, n_z\rangle$ in terms of the individual 1D states $|n_x\rangle$, $|n_y\rangle$, and $|n_z\rangle$.

When a Hamiltonian is the exact sum of independent Hamiltonians for different dimensions, a fundamental postulate of quantum mechanics tells us that the total state vector is simply the **tensor product** of the individual state vectors.

Therefore, the answer to the question is:

$$|n_x, n_y, n_z\rangle = |n_x\rangle \otimes |n_y\rangle \otimes |n_z\rangle$$

In many physics courses, it is also perfectly acceptable to write this without the tensor product symbol $\otimes$ by just placing the kets next to each other, like this:

$$|n_x, n_y, n_z\rangle = |n_x\rangle |n_y\rangle |n_z\rangle$$

This mathematical statement physically means that a measurement in the x-direction is completely independent of the states in the y-direction or z-direction.

---

Now that we know the 3D state is just a product of the 1D states, finding the total energy is incredibly straightforward. Would you like me to show you how to calculate the total energy eigenvalues ($E$) for this complete 3D system?