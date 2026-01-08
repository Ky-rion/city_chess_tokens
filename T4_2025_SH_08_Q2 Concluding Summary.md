

That is a great idea. In theoretical physics exams, knowing _how_ to derive a result is often more valuable than the result itself.

Here is a summary cheat sheet based on Problem 2, divided into **Physics Concepts**, **Key Formulas**, and **Mathematical Tricks**.

### **Cheat Sheet: Stochastic Processes & Reliability**

#### **1. Physical Concepts**

-   **Bernoulli Trial:** A single event with two outcomes (Success/Failure).
    
    -   $p$: Probability of failure.
        
    -   $q$: Probability of success ($q = 1-p$).
        
-   **Independence:** If events are independent, you multiply their probabilities.
    
    -   $P(A \text{ and } B) = P(A) \cdot P(B)$.
        
-   **Geometric Distribution:** Used for waiting times. "How many trials until the first failure?"
    
-   **Redundancy:**
    
    -   **Series:** Fails if _any_ part fails. (Risk increases).
        
    -   **Parallel:** Fails only if _all_ parts fail. (Safety increases).
        

---

#### **2. Important Formulas (The Results)**

![[Pasted image 20260102131413.png]]

> **Rule of Thumb:** A redundant pair increases the expected lifetime by roughly **50%** (factor of $\approx 1.5$), but it reduces the instantaneous risk of failure quadratically ($p \to p^2$).

---

#### **3. Mathematical Toolbox (The Derivations)**

A. Expected Value Definition

The average outcome $\langle k \rangle$ is the sum of the value $k$ times the probability of getting $k$:

$$\langle k \rangle = \sum_{k=0}^{\infty} k \cdot P(k)$$

B. The "Derivative Trick" (Crucial for Exams!)

When summing series that look like $k \cdot x^k$, do not sum directly. Turn $k$ into a derivative:

$$k \cdot x^k = x \frac{d}{dx} (x^k)$$

This allows you to pull the operator out:

$$\sum_{k=1}^{\infty} k x^k = x \frac{d}{dx} \left( \sum_{k=1}^{\infty} x^k \right)$$

C. Geometric Series Sum

You must memorize this for statistical physics:

$$\sum_{k=0}^{\infty} q^k = \frac{1}{1-q} \quad \text{or} \quad \sum_{k=1}^{\infty} q^k = \frac{q}{1-q}$$

---

**Would you like to try applying these formulas to a specific example? For instance, we could calculate the actual numbers if the failure chance was 1% ($p=0.01$).**