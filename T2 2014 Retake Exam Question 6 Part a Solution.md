

Welcome to class! I am delighted to be your guide into the fascinating world of Quantum Mechanics. It is a strange and beautiful landscape, but don’t worry—we will walk through it step by step.

Today, we are looking at a problem regarding **Conserved Quantities** (the German title "Erhaltungsgrößen" means exactly that). This is a fundamental concept because it tells us which properties of a quantum system stay constant over time.

First, let me translate the problem statement into English so we are completely aligned, and then I will break down every single concept for you.

---

### **The Translation**

6: Conserved Quantities

Let $\hat{A}$ be an arbitrary Observable that commutes with the Hamiltonian operator $[\hat{H}, \hat{A}] = 0$. We assume that $\hat{A}$ has a purely discrete spectrum.

**(6a) [ /3pts]** Give the projection operator $\hat{\Pi}_a$ onto the eigenspace for the eigenvalue $a$ of $\hat{A}$ in two forms:

1.  By means of the normalized eigenvectors of $\hat{A}$ for the eigenvalue $a$.
    
2.  As a function of the operator $\hat{A}$.
    

---

### **Part 1: The Setup (The "What is happening?" Phase)**

Before we solve the math, we must understand the players on the field.

1. The Observable ($\hat{A}$)

In quantum mechanics, anything you can measure (like position, momentum, or spin) is called an Observable, and we represent it mathematically as an operator (that's why it has a little hat $\hat{A}$). You can think of an operator as a machine: you feed it a quantum state function, and it chews on it and spits out a new function.

2. The Spectrum & Eigenvalues

When we measure $\hat{A}$, we don't just get random numbers. We get specific values called eigenvalues. The list of all possible values you can measure is called the spectrum.

-   The problem states the spectrum is "discrete." This means the possible values are distinct steps (like energy levels in an atom: $1, 2, 3...$) rather than a continuous smooth slide.
    

3. The Commutator ($[\hat{H}, \hat{A}] = 0$)

This is the most important sentence in the intro. $\hat{H}$ is the Hamiltonian, the operator for total Energy. It controls how the system changes over time.

The notation $[\hat{H}, \hat{A}]$ is the commutator, defined as $\hat{H}\hat{A} - \hat{A}\hat{H}$.

-   If $[\hat{H}, \hat{A}] = 0$, it means the order doesn't matter ($\hat{H}\hat{A} = \hat{A}\hat{H}$).
    
-   **Physics meaning:** $\hat{A}$ is a **Conserved Quantity**. If you prepare a state with a specific value of $A$, it will stay that way forever. It is a "Constant of Motion."
    

---

### **Part 2: Solving Question (6a)**

We need to find the **Projection Operator** $\hat{\Pi}_a$.

What is a Projection Operator?

Imagine you have a basket of mixed fruit (apples, bananas, oranges). A "Apple Projection Operator" is a machine that, when you dump the basket in, keeps all the apples exactly as they are but destroys the bananas and oranges.

In math: If you apply $\hat{\Pi}_a$ to a state vector, it filters out everything _except_ the part that corresponds to the eigenvalue $a$.

#### **Form 1: Using Normalized Eigenvectors**

In Quantum Mechanics, we use **Dirac Notation** (Bra-ket notation).

-   A state vector is a "ket": $| \psi \rangle$
    
-   Its conjugate (like a row vector) is a "bra": $\langle \psi |$
    

Let's say the eigenvectors corresponding to the eigenvalue $a$ are written as $|a\rangle$.

If we have a simple case where there is only one eigenvector for the value $a$ (non-degenerate), the projector is simply the outer product:

$$\hat{\Pi}_a = |a\rangle \langle a|$$

Why?

Let's apply this to a general state $|\psi\rangle = c_a|a\rangle + c_b|b\rangle$ (a mix of state $a$ and state $b$):

$$\hat{\Pi}_a |\psi\rangle = (|a\rangle \langle a|) (c_a|a\rangle + c_b|b\rangle)$$

$$= c_a |a\rangle \underbrace{\langle a | a \rangle}_{1} + c_b |a\rangle \underbrace{\langle a | b \rangle}_{0}$$

$$= c_a |a\rangle$$

It kept the $a$ part and killed the $b$ part!

The General Case (Degeneracy):

Sometimes, multiple different states share the same eigenvalue $a$. We call this degeneracy. We need to sum over all of them to capture the whole "space" of $a$. Let's denote the different eigenvectors for eigenvalue $a$ as $|a, i\rangle$, where $i$ counts them ($1, 2, \dots g_a$).

The answer for Form 1 is:

$$\hat{\Pi}_a = \sum_{i=1}^{g_a} |a, i\rangle \langle a, i|$$

_(Where $g_a$ is the degree of degeneracy. If there is no degeneracy, the sum just has one term.)_

---

#### **Form 2: As a Function of Operator $\hat{A}$**

This is the clever "math trick" part. We want to write a formula using only the operator $\hat{A}$ itself, not the vectors.

We need a function $f(\hat{A})$ that acts like a **filter**:

1.  If the operator sees the value $a$, it should become **1**.
    
2.  If the operator sees any other eigenvalue $a'$ (where $a' \neq a$), it should become **0**.
    

We can build this using a mathematical structure similar to the **Lagrange Interpolating Polynomial**.

The formula is:

$$\hat{\Pi}_a = \prod_{a' \neq a} \frac{\hat{A} - a' \hat{1}}{a - a'}$$

**Let's break this scary formula down:**

-   The symbol $\prod$ means a **product** (multiply everything together).
    
-   We multiply terms for every eigenvalue $a'$ in the spectrum that is **not** our target $a$.
    
-   $\hat{1}$ is the Identity operator (a matrix with 1s on the diagonal).
    

Why does this work?

Imagine we apply this big product operator to an eigenvector $|a\rangle$ (our target):

Every instance of $\hat{A}$ in the formula gets replaced by the value $a$.

$$\text{Term} = \frac{a - a'}{a - a'} = 1$$

Since every term is 1, the product is $1 \times 1 \times 1 \dots = 1$. The state is kept!

Now, apply it to a different eigenvector $|b\rangle$ (where $b \neq a$).

Somewhere in that big product list, there will be a term where $a' = b$.

That specific term becomes:

$$\frac{\hat{A} - b\hat{1}}{a - b} \rightarrow \frac{b - b}{a - b} = \frac{0}{a - b} = 0$$

Since one term in the product is 0, the whole thing becomes 0. The state is destroyed!

---

### **Professor's Summary**

So, the answer the question is looking for is:

1. Using Eigenvectors:

$$\hat{\Pi}_a = \sum_{i} |a, i\rangle \langle a, i|$$

2. As a function of $\hat{A}$:

$$\hat{\Pi}_a = \prod_{a' \in \sigma(\hat{A}), a' \neq a} \frac{\hat{A} - a'\hat{1}}{a - a'}$$

(Where $\sigma(\hat{A})$ denotes the spectrum, or the set of all eigenvalues of $\hat{A}$.)

You have just defined a quantum filter! This tool is incredibly useful in quantum information theory and measurement definitions.

**Would you like me to show you a concrete example using a $2 \times 2$ matrix (like electron spin) to see these numbers in action?**