

![[Pasted image 20251108172455.png]]


You're very welcome! It's been a great "tour" through quantum mechanics. This last one is a very neat and common problem that shows how powerful the mathematical definitions are.

Let's break it down.

### 1. ❓ What are "Messwerte" (Measurement Values)?

This is the first and most important link. In quantum mechanics, a fundamental rule (or "postulate") states:

> The **only** possible values you can _ever_ get from measuring an observable (like $\hat{S}$) are the **eigenvalues** of that observable's operator.

So, the question "What are the possible measurement values?" is _exactly_ the same as asking, "What are the possible eigenvalues (let's call them $\lambda$) of the operator $\hat{S}$?"

The solution correctly identifies these as **$\{1, -1\}$**. Now, we have to prove _why_.

---

### 2. 🧾 The Justification (The Proof)

The solution gives the key step: Für die Eingewerte gilt $\lambda^2 = 1$, daher $\lambda = \pm 1$.

(For the eigenvalues, $\lambda^2 = 1$ holds, therefore $\lambda = \pm 1$.)

Let's derive this step-by-step.

1.  Start with the Eigenvalue Equation:
    
    By definition, if $\psi$ is an eigenstate of $\hat{S}$ with an eigenvalue $\lambda$, this equation must be true:
    
    $$\hat{S} \psi = \lambda \psi$$
    
    (This just says: "When the operator $\hat{S}$ acts on its eigenstate $\psi$, it just multiplies $\psi$ by a number $\lambda$.")
    
2.  Use the Given Property:
    
    The problem tells us that $\hat{S}^2 = \mathbf{1}$ (where $\mathbf{1}$ is the identity operator, which does nothing). Let's see what happens if we apply the $\hat{S}$ operator to our eigenvalue equation a second time.
    
    Let's apply $\hat{S}$ to both sides of the equation from step 1:
    
    $$\hat{S} (\hat{S} \psi) = \hat{S} (\lambda \psi)$$
    
3.  **Simplify Both Sides:**
    
    -   **Left Side:** $\hat{S} (\hat{S} \psi)$ is just $\hat{S}^2 \psi$.
        
    -   **Right Side:** $\lambda$ is just a number, not an operator, so it can be pulled out in front: $\lambda (\hat{S} \psi)$.
        
    
    So, our new equation is:
    
    $$\hat{S}^2 \psi = \lambda (\hat{S} \psi)$$
    
4.  Substitute and Solve:
    
    We're almost there! Look at the right side: we see the term $\hat{S} \psi$. But from step 1, we know that $\hat{S} \psi = \lambda \psi$! Let's substitute that in:
    
    $$\hat{S}^2 \psi = \lambda (\lambda \psi)$$
    
    $$\hat{S}^2 \psi = \lambda^2 \psi$$
    
    Now, let's use the property from the problem: $\hat{S}^2 = \mathbf{1}$.
    
    $$\mathbf{1} \psi = \lambda^2 \psi$$
    
    The identity operator $\mathbf{1}$ does nothing to $\psi$, so $\mathbf{1} \psi = \psi$:
    
    $$\psi = \lambda^2 \psi$$
    
5.  The Final Step:
    
    Let's get everything on one side of the equation:
    
    $$\lambda^2 \psi - \psi = 0$$
    
    $$(\lambda^2 - 1) \psi = 0$$
    
    This equation tells us that the number $(\lambda^2 - 1)$ times the state $\psi$ equals zero.
    
    We know that $\psi$ cannot be zero (an eigenstate must exist to be measured). Since $\psi$ is not zero, the other part of the product must be zero:
    
    $$\lambda^2 - 1 = 0$$
    
    $$\lambda^2 = 1$$
    
    $$\lambda = \pm 1$$
    

And there you have it! We've mathematically proven that the _only_ possible eigenvalues (and thus the only possible measurement values) are **+1** and **-1**.

> **Fun fact:** This isn't just a toy problem! The **Parity operator** $\hat{P}$ (which checks if a function is even or odd) has this _exact_ property: $\hat{P}^2 = \mathbf{1}$ (reflecting twice gets you back to where you started). Its eigenvalues are $+1$ (for even states) and $-1$ (for odd states).

---

Thank you for this wonderful set of questions! It was a pleasure to go through them with you. I hope these explanations have been helpful!