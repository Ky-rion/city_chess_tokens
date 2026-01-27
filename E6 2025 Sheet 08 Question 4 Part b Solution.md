

![[Pasted image 20260125190549.png]]

Excellent, welcome back to the blackboard! Let's tackle **Part b)**.

This part of the problem is a classic exercise in "counting states." In physics, before we can calculate probabilities or thermodynamics, we have to know exactly how many different ways our system can arrange itself.

Let's break down the question and the solution you provided.

---

### The Question (Translated)

> **German:** "Bestimmen Sie $\Omega_i$, die Anzahl der Möglichkeiten $N_i$ Fermionen auf $D_i$ Zustände zu verteilen."
> 
> **English:** "Determine $\Omega_i$, the number of possibilities to distribute $N_i$ fermions into $D_i$ states."

The goal is to find a mathematical formula for $\Omega_i$.

### The Physics: Why Fermions are "Picky" Eaters

To answer this, we need to remember the two golden rules of **Fermions** (like electrons):

1.  **The Pauli Exclusion Principle:** No two fermions can occupy the exact same state at the same time. Think of the energy states $D_i$ as seats in a movie theater. You cannot have two people sitting in one seat.
    
2.  **Indistinguishability:** All electrons look exactly the same. If you have two electrons and they swap seats, the "state" of the universe hasn't changed. We cannot tell them apart.
    

### The Derivation (The "Cinema" Analogy)

Let's imagine energy level $E_i$ is a row in a cinema.

-   **$D_i$**: The number of empty seats in that row (the "degeneracy" or available slots).
    
-   **$N_i$**: The number of people (fermions) you want to seat in that row.
    

**Step 1: Placing the first person**

You have $D_i$ seats available. The first fermion can pick any of them.

-   Options: $D_i$
    

**Step 2: Placing the second person**

One seat is taken (Pauli Exclusion!). So the second fermion only has $(D_i - 1)$ seats left to choose from.

-   Options: $D_i \times (D_i - 1)$
    

**Step 3: Placing all $N_i$ people**

We keep going until everyone is seated.

-   Options: $D_i \times (D_i - 1) \times (D_i - 2) \times \dots \times (D_i - N_i + 1)$
    

Mathematically, we can write this product using factorials as:

$$\frac{D_i!}{(D_i - N_i)!}$$

**Step 4: Fixing the Overcounting (The "Clone" Problem)**

Wait! We made a mistake. The math above assumes the order matters (i.e., "Alice in seat 1, Bob in seat 2" is different from "Bob in seat 1, Alice in seat 2").

But electrons are identical clones! "Electron A in seat 1, Electron B in seat 2" looks **exactly** the same as "Electron B in seat 1, Electron A in seat 2."

Because we have $N_i$ identical fermions, there are $N_i!$ (N-factorial) ways to swap them around without changing the physical picture. We must divide our answer by this number to remove the duplicates.

$$\Omega_i = \frac{\text{Permutations}}{\text{Swaps}} = \frac{\frac{D_i!}{(D_i - N_i)!}}{N_i!}$$

### The Solution Explained

This leads us directly to the formula shown in your second image (the solution):

$$\Omega_i = \frac{D_i!}{N_i! (D_i - N_i)!}$$

This specific mathematical structure is extremely famous. It is called the **Binomial Coefficient**, often read aloud as "D choose N" (written as $\binom{D}{N}$).

As your professor's notes say:

> _"Mit dem Binomialkoeffizienten ergeben sich $\Omega_i = \binom{D_i}{N_i}$ Möglichkeiten..."_
> 
> _"Using the binomial coefficient results in $\Omega_i = \binom{D_i}{N_i}$ possibilities..."_

**In Summary:**

The formula represents the number of unique ways you can choose $N_i$ occupied spots out of $D_i$ available spots, where the order of choosing doesn't matter, and you can't double-park in a single spot.

---

**Professor's Check-in:**

Does this "Cinema Seat" analogy help you visualize why we divide by $N_i!$ and why we subtract $N_i$ from $D_i$?

**Would you like to move on to the next step, where we usually combine all these energy levels to find the total entropy?**