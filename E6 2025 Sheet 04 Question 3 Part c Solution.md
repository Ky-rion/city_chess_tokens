

![[Pasted image 20260125184009.png]]

Excellent! We are moving right along the derivation.

In Part (b), we established that the crystal _wants_ to be messy (increase Entropy) to lower its Gibbs Free Energy. Now, in **Part (c)**, we have to quantify exactly **how much** entropy is created when we make these defects.

We need to justify this scary-looking formula:

$$\Delta S_{conf} = k_B \cdot \ln\left( \binom{N}{n} \binom{N}{n} \right)$$

Let's break this down using the solution provided in the third image.

---

### The Grand Concept: Boltzmann's Entropy

The heart of statistical mechanics (and this problem) is **Ludwig Boltzmann's famous equation**, which is actually carved on his tombstone in Vienna:

$$S = k_B \cdot \ln(W)$$

-   **$S$**: Entropy (The "Messiness").
    
-   **$k_B$**: Boltzmann Constant (A tiny number that scales the math to real-world energy units).
    
-   **$W$**: The number of **Microstates** (The number of ways you can arrange the atoms).
    

**The Challenge:** To find the Entropy ($S$), we just need to calculate $W$ (the number of ways we can arrange these defects).

---

### Decoding the Professor's Solution

Let's look at the German text in the solution (Image 3) to see how they calculate $W$.

**1. The "Two Ion" Rule**

> _"Da bei einem Schottky Defekt stets 2 Ionen beteiligt sind..."_

**Translation:** "Since 2 ions are always involved in a Schottky defect..."

-   Remember Part (a)? To keep the crystal electrically neutral, if we kick out a Cation (+), we _must_ also kick out an Anion (-).
    
-   This means we have two separate puzzles to solve:
    
    1.  Where do we put the $n$ holes in the **Cation** grid?
        
    2.  Where do we put the $n$ holes in the **Anion** grid?
        

**2. The Binomial Coefficient (The "n choose k" part)**

> _"...ergibt sich die gesamte Anzahl an Mikrozuständen W aus dem Produkt der beiden Binomialkoeffizienten für beide Ionen Typen."_

**Translation:** "...the total number of microstates $W$ results from the product of the two binomial coefficients for both ion types."

This is the core of the math. We need to use combinatorics.

-   Imagine you have $N$ total parking spots (lattice sites) and you want to leave $n$ of them empty.
    
-   How many different patterns of empty spots can you make?
    
-   The math for this is "N choose n":
    
    $$\binom{N}{n} = \frac{N!}{n!(N-n)!}$$
    

**3. Why are there two of them?**

Because an ionic crystal is actually **two interpenetrating lattices** (one for cations, one for anions).

-   **Ways to arrange Cation vacancies:** $W_{cation} = \binom{N}{n}$
    
-   **Ways to arrange Anion vacancies:** $W_{anion} = \binom{N}{n}$
    

Since the arrangement of cations is independent of the arrangement of anions, the **Total Number of Ways ($W_{total}$)** is the product of the two:

$$W_{total} = W_{cation} \cdot W_{anion} = \binom{N}{n} \cdot \binom{N}{n}$$

---

### Putting it all together

Now we go back to Boltzmann's Tombstone equation.

1.  Start with the formula:
    
    $$S = k_B \cdot \ln(W)$$
    
2.  Plug in our $W_{total}$ we just found:
    
    $$S = k_B \cdot \ln\left( W_{cation} \cdot W_{anion} \right)$$
    
3.  Substitute the binomials:
    
    $$\Delta S_{conf} = k_B \cdot \ln\left( \binom{N}{n} \binom{N}{n} \right)$$
    

And there is your justification!

---

### A Real-World Analogy

Imagine a classroom with red desks (for cations) and blue desks (for anions).

-   You have **$N=30$** red desks and **$N=30$** blue desks.
    
-   You want to create **$n=2$** Schottky defects. This means you must remove 2 red chairs and 2 blue chairs.
    

**Step 1:** How many ways can you pick 2 red desks to empty out of 30?

That's $\binom{30}{2}$.

**Step 2:** How many ways can you pick 2 blue desks to empty out of 30?

That's also $\binom{30}{2}$.

**Step 3:** What is the total number of unique messy room layouts?

It is (Ways to mess up red) multiplied by (Ways to mess up blue).

---

### What comes next?

You are now set up for the final and most famous step of this derivation. You have a formula with factorials ($N!$), which are impossible to calculate for large numbers (like $10^{23}$ atoms).

Usually, the next question asks you to use **Stirling's Approximation** ($\ln(x!) \approx x\ln(x) - x$) to simplify this into a nice, clean equation that lets you solve for $n$.

**Shall we move on to that next part?**