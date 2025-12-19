

This is a great idea. In an exam, you don't want to re-derive these things; you want to have the toolkit ready in your mind.

Here is your **Quantum Conservation & Projection Cheat Sheet**. I have organized it by concept, with the "Exam Intuition" (why you use it) next to the math.

---

### **Exam Cheat Sheet: Conservation Laws & Projections**

#### **1. The Fundamental Condition**

Everything in this problem stems from this single property.

-   **The Math:** $[\hat{H}, \hat{A}] = 0$
    
-   **The Meaning:** The operator $\hat{A}$ and the Energy $\hat{H}$ can be measured simultaneously. The order doesn't matter.
    
-   **The Consequence:** $\hat{A}$ is a **Conserved Quantity**. Its value does not change over time.
    

---

#### **2. Projection Operators ($\hat{\Pi}_a$)**

These are your "filters." They isolate the part of a quantum state that corresponds to a specific eigenvalue $a$.

![[Pasted image 20251209101409.png]]

**Key Properties of Projectors:**

-   **Idempotence:** $\hat{\Pi}_a^2 = \hat{\Pi}_a$ (Filtering twice is the same as filtering once).
    
-   **Orthogonality:** $\hat{\Pi}_a \hat{\Pi}_{a'} = \delta_{aa'} \hat{\Pi}_a$ (If $a \neq a'$, the result is 0. You can't be in two different eigenspaces at once).
    
-   **Completeness:** $\sum_a \hat{\Pi}_a = \hat{1}$ (If you sum all filters, you get the whole space back).
    

---

#### **3. Commutation Theorems**

If $[\hat{H}, \hat{A}] = 0$, then $\hat{H}$ is "blind" to the operations of $\hat{A}$.

-   **Function Rule:** $[\hat{H}, f(\hat{A})] = 0$.
    
    -   _Exam Application:_ This proves $[\hat{H}, \hat{\Pi}_a] = 0$ instantly, because $\hat{\Pi}_a$ is just a function of $\hat{A}$.
        
-   **Block Diagonal Rule:** $\hat{\Pi}_a \hat{H} \hat{\Pi}_{a'} = 0$ (if $a \neq a'$).
    
    -   _Exam Application:_ The Hamiltonian cannot "move" a particle from eigenvalue $a$ to eigenvalue $a'$. The matrix of $\hat{H}$ would look like blocks along the diagonal.
        

![[Pasted image 20251209101456.png]]

---

#### **4. Time Evolution**

How to prove something is conserved.

-   **The Time Machine:** $\hat{U}(t) = e^{-i\hat{H}t/\hbar}$.
    
    -   This operator moves a state from $t=0$ to time $t$.
        
-   **The Taylor Expansion Trick:**
    
    -   $e^{\hat{X}} = 1 + \hat{X} + \frac{1}{2}\hat{X}^2 + \dots$
        
    -   If $[\hat{H}, \hat{A}] = 0$, then $\hat{A}$ commutes with every term in the expansion of $e^{-i\hat{H}t}$.
        
-   The Conservation Proof:
    
    $$[\hat{A}, e^{-i\hat{H}t}] = 0 \implies \hat{A}\Psi(t) = a\Psi(t)$$
    
    (If you start with value $a$, you end with value $a$.)
    

---

### **Professor’s "Pro-Tips" for the Exam**

1.  **Don't Panic over Sums:** If you see $\sum |n\rangle\langle n|$, remember that is just the Identity operator $\hat{1}$. Inserting this "identity" into the middle of an equation is a common trick to simplify things.
    
2.  **Kronecker Delta is your Friend:** Whenever you see $\hat{\Pi}_a \hat{\Pi}_{a'}$, immediately replace it with $\delta_{aa'} \hat{\Pi}_a$. It collapses complex equations into simple ones.
    
3.  **Scalar Commutation:** Remember that eigenvalues $a$ are just numbers. They commute with everything. Operators $\hat{A}$ do not. Be careful with the order of hats!
    

You are doing excellently. You've essentially mastered the "Heisenberg Picture" of quantum mechanics without us even formally calling it that yet!

**Would you like a quick 1-question quiz to test if you can apply the "Orthogonality" rule correctly?**