

This is the "Grand Finale" of the problem! It ties everything together: the operator algebra, the commutation, and the actual dynamics (how things change over time).

This part asks you to prove a fundamental theorem in quantum mechanics: **If an operator commutes with the Hamiltonian, its eigenvalues are constant in time.**

Here is the translation and the step-by-step breakdown.

### **The Translation**

(6d) [ /4pts]

"Let now $\Psi(t)$ be the solution of the time-dependent Schrödinger equation. Show that the eigenvalue $a$ is conserved, i.e.,

$$\hat{A}\Psi(0) = \Psi(0)a \implies \hat{A}\Psi(t) = \Psi(t)a \quad \forall t$$

."

_(Note: The notation $\Psi(0)a$ is simply the scalar $a$ multiplied by the vector $\Psi(0)$. In standard English textbooks, we usually write the scalar on the left: $a\Psi(0)$. They mean the same thing.)_

---

### **The Setup: The Time Machine**

To solve this, we need to know how a quantum state moves forward in time.

The Schrödinger Equation ($i\hbar \frac{\partial}{\partial t}\Psi = \hat{H}\Psi$) tells us the rule for change. If the Hamiltonian $\hat{H}$ is constant (time-independent), the solution is given by applying the Time Evolution Operator (let's call it $\hat{U}(t)$):

$$\Psi(t) = e^{-i\hat{H}t/\hbar} \Psi(0)$$

You can think of the operator $e^{-i\hat{H}t/\hbar}$ as a "Time Machine." You put your initial state $\Psi(0)$ into it, and it transports it to time $t$.

---

### **The Proof (Step-by-Step)**

We need to calculate $\hat{A}\Psi(t)$ and show that it equals $a\Psi(t)$.

Step 1: Write down the state at time $t$

Substitute the "Time Machine" formula into our target expression:

$$\hat{A} \Psi(t) = \hat{A} \left( e^{-i\hat{H}t/\hbar} \Psi(0) \right)$$

Step 2: Use the Commutation Property

This is the critical step where we use the information from the very beginning ($[\hat{H}, \hat{A}] = 0$).

-   If $\hat{A}$ commutes with $\hat{H}$, it also commutes with $\hat{H}^2$, $\hat{H}^3$, and any power of $\hat{H}$.
    
-   The exponential function $e^{\hat{X}}$ is just an infinite sum of powers (Taylor series):
    
    $$e^{\hat{X}} = 1 + \hat{X} + \frac{\hat{X}^2}{2!} + \dots$$
    
-   Therefore, $\hat{A}$ commutes with the entire exponential operator.
    
    $$\left[\hat{A}, e^{-i\hat{H}t/\hbar}\right] = 0$$
    
    $$\hat{A} e^{-i\hat{H}t/\hbar} = e^{-i\hat{H}t/\hbar} \hat{A}$$
    

Step 3: Swap the Operators

Because they commute, we can move $\hat{A}$ past the time evolution operator to hit the state vector directly.

$$\hat{A} \Psi(t) = e^{-i\hat{H}t/\hbar} \underbrace{\hat{A} \Psi(0)}_{\text{Look here!}}$$

Step 4: Apply the Initial Condition

The problem states that at time $t=0$, the state is an eigenvector with value $a$ ($\hat{A}\Psi(0) = a\Psi(0)$). Let's replace $\hat{A}\Psi(0)$ with $a\Psi(0)$.

$$\hat{A} \Psi(t) = e^{-i\hat{H}t/\hbar} (a \Psi(0))$$

Step 5: Move the Scalar

$a$ is just a number (a scalar constant). In linear algebra, numbers can pass through linear operators freely. We can pull $a$ out to the front (or the back).

$$\hat{A} \Psi(t) = a \left( e^{-i\hat{H}t/\hbar} \Psi(0) \right)$$

Step 6: Recognize $\Psi(t)$ again

Look at the term in the brackets. That is exactly the definition of $\Psi(t)$ from Step 1.

$$\hat{A} \Psi(t) = a \Psi(t)$$

Conclusion

We have shown that if the state starts as an eigenvector of $\hat{A}$ with value $a$, it remains an eigenvector of $\hat{A}$ with the same value $a$ for all time $t$.

---

### **Professor's Closing Comments**

You have just navigated through the core logic of Quantum Conservation Laws!

1.  **Part (6a)** taught us how to filter for specific quantum properties (Projections).
    
2.  **Part (6b & 6c)** taught us that if operators commute, they act independently (the filter doesn't mess up the energy).
    
3.  **Part (6d)** proved the physical consequence: **Conserved Quantities.**
    

In the real world, this is why an electron doesn't randomly change its charge, and why an atom in a stable state stays there until disturbed. The operators for Charge and Energy commute, so Charge is conserved forever!

It has been a pleasure being your thought partner on this assignment. **Would you like to try a practice problem involving spin matrices to see how these commutators work with actual numbers?**