

Welcome to the wonderful world of quantum mechanics! It is completely normal if this looks like an alien language at first glance. We all start from zero, and I am thrilled to guide you through this.

First, let's translate the German text in the image so we are on the exact same page:

> **6. One-dimensional Helium atom (17 Points)**
> 
> 1. How many nodes do the ground state $\Phi_1(x)$ and the first excited state $\Phi_2(x)$ of $h$ have? Make a qualitative sketch of the two states. [2 Pts.]
>     

This is a beautiful, fundamental question. Even though the overarching problem is about a Helium atom, this specific part asks about a single-particle Hamiltonian, denoted here as $h$. The wavefunctions $\Phi_1(x)$ and $\Phi_2(x)$ are the mathematical descriptions of the particle's quantum states.

Let's break down the concepts to answer this step-by-step.

---

### Part 1: What is a Node?

In quantum mechanics, a **node** is a point where the wavefunction crosses the horizontal axis (where $\Phi(x) = 0$). Physically, the square of the wavefunction, $|\Phi(x)|^2$, tells us the probability of finding the particle at a specific location $x$. Therefore, a node is a place where there is exactly zero probability of finding the particle.

_(Note: We do not count the boundaries at infinity, or the absolute edges of an inescapable box, as nodes. We only count the zero-crossings strictly inside the allowed region)._

### Part 2: The Ground State $\Phi_1(x)$

The ground state is the state with the absolute lowest possible energy.

In quantum mechanics, the kinetic energy of a particle is intimately tied to how much its wavefunction "wiggles" or curves (mathematically, this is the second derivative). Every time a wavefunction goes from a positive peak, crosses zero (a node), and goes to a negative valley, it has to bend. More bending means higher kinetic energy.

To minimize the energy, the ground state wavefunction must be as smooth and "un-wiggled" as possible. Therefore, it is just a single, smooth bump.

- **Answer:** The ground state $\Phi_1(x)$ has **0 nodes**.
    

### Part 3: The First Excited State $\Phi_2(x)$

The first excited state is the next level up; it has the second-lowest energy.

Because it is a distinct quantum state, a fundamental rule called _orthogonality_ requires that it must not overlap entirely with the ground state. If the ground state is entirely positive (a single bump up), the first excited state must have a positive part and a negative part so that they cancel each other out when multiplied together.

To achieve this with the _least_ amount of added kinetic energy (bending), the wavefunction will cross the zero axis exactly once.

- **Answer:** The first excited state $\Phi_2(x)$ has **1 node**.
    

> **The Golden Rule of 1D Quantum Mechanics (Oscillation Theorem):** > If you order the energy states from lowest to highest ($n = 1, 2, 3, \dots$), the $n$-th state will always have exactly $n - 1$ nodes!

---

### Part 4: Qualitative Sketch

If you were drawing this on your exam paper, you wouldn't need an exact mathematical plot—just a "qualitative" sketch that captures the physics (the nodes and the general shape).

Here is how you should draw it:

1. **Draw an x-axis and a y-axis** for your wavefunctions.
    
2. **Sketch $\Phi_1(x)$:** Draw a single, symmetric "hill" or bell curve that starts near zero, peaks in the middle, and goes back down to zero. It should never dip below the x-axis.
    
3. **Sketch $\Phi_2(x)$:** Draw a wave that starts near zero, goes up to a positive peak, crosses exactly through the center of the x-axis (this is your 1 node!), dips down to a negative valley, and comes back up to zero.
    

---

You did a great job tackling your first bit of quantum theory! This concept of nodes will be crucial when you start putting _two_ electrons into these states to build your 1D Helium atom in the later parts of this problem.

Would you like me to explain how we use these single-particle states to construct the actual wavefunction for the two electrons in the Helium atom, or should we look at the math behind why kinetic energy causes these wiggles?