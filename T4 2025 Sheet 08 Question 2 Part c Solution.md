

This is a fantastic follow-up question. It deals with **redundancy**, a core concept in engineering safety and reliability theory.

The problem (Aufgabe 2c) asks us to analyze a system with **two** independent components. The aircraft only crashes (critical failure) if **both** components fail on the same flight.

Here is the step-by-step breakdown based on your professor's notes.

### 1. The Setup: A Redundant System

-   **Single Component:** Fails with probability $p$, survives with $q = 1-p$.
    
-   **Dual System:** We have two components.
    
-   **Critical Failure:** Occurs _only_ if Component 1 fails **AND** Component 2 fails simultaneously.
    
-   **Safety Net:** If Component 1 breaks but Component 2 keeps working, the plane is still safe (and vice versa).
    

We need to find the **Maintenance Interval**, which is defined as the **Expected Value** ($\langle k \rangle$) of successful flights before a critical failure occurs.

### 2. Deriving the Expected Lifetime ($\langle k \rangle$)

This derivation is more complex than part (b) because the system has "partial failure" states (one working, one broken). The notes use a rigorous summation method.

Step A: The Probability of "Survival"

The notes calculate the probability that the system survives $k$ flights. For the system to survive $k$ flights, we need to avoid the case where both fail within those $k$ flights.

-   The notes derive the probability distribution $P_k$ (probability that the critical failure happens exactly at flight $k$).
    
-   However, a simpler way to understand the result derived in the notes is to view the system lifetime as the **maximum** lifetime of the two components. The system works as long as _at least one_ component works.
    

Step B: The Summation (The "Professor's Trick" Returns)

Your professor calculates the expected value $\langle k \rangle$ by summing the probabilities using the derivative trick again.

$$\langle k \rangle = \sum_{k=1}^{\infty} k \cdot P_k$$

Through algebraic manipulation (using $r = q^2$ and derivatives), the notes arrive at this specific formula for the expected number of flights:

$$\langle k \rangle = \frac{q}{1-q} \left( 2 - \frac{q}{1+q} \right)$$

Step C: Interpreting the Formula

Let's translate this back into $p$ (since $q = 1-p$) to make it readable:

$$\langle k \rangle = \frac{1-p}{p} \left( 2 - \frac{1-p}{2-p} \right)$$

-   **Recall Part (a):** A single component lasts $\approx 1/p$ flights.
    
-   **This Result:** The term in the brackets is roughly $2 - 0.5 = 1.5$.
    
-   So, adding a second component increases the expected lifetime to roughly **1.5 times** that of a single component. It doesn't double it, because once the first one breaks (which happens relatively "soon"), you are back to relying on a single component.
    

### 3. The "Smallest Possible Failure Probability"

The second part of the question asks: _What is the smallest possible failure probability and how can it be achieved?_

The notes provide a very clear answer.

The Problem with Long Intervals:

If you wait a long time to check the plane (the interval calculated above), there is a high risk that one component fails early, and you fly for a long time with no backup, essentially waiting for the second one to fail.

The Solution:

To achieve the absolute safest operation, you must check the components after every single flight.

-   **Why?** If you check after every flight, you ensure that you always start with two working components.
    
-   The Probability: For a crash to occur, both must fail on that specific single flight. Since they are independent, you multiply their probabilities:
    
    $$P_{\text{min}} = p \cdot p = p^2$$
    

> **From the notes:** "Smallest possible prob. for failure is achieved, if after each flight devices are checked, then we have $P_n = p^2$".

### Summary of Answers for 2c

1.  **Maintenance Interval:** You should set the interval to $N = \frac{q}{p} \left( 2 - \frac{q}{1+q} \right)$ flights.
    
2.  **Smallest Probability:** The smallest risk is $p^2$.
    
3.  **How to Achieve It:** Inspect and replace/repair components **after every flight** (Maintenance Interval = 1).
    

---

**Would you like to move on to Problem 3 (Aufgabe 3)? It shifts gears completely to "Entropy" and counting states on a tetrahedron (a pyramid shape).**