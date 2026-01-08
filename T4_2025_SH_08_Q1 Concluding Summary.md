

Here is a concise summary of the key formulas and concepts from this problem, perfect for an exam cheat sheet.

### Cheat Sheet: The "Secret Santa" / Birthday Problem

1. The "At Least One" Shortcut (Complementary Probability)

Instead of calculating the messy probability of "at least one collision" (one pair, two pairs, triplets, etc.), always calculate the probability of the opposite event ("Everyone is unique") and subtract it from 1.

-   **Goal:** $P(\text{Collision})$
    
-   Method:
    
    $$P(\text{Collision}) = 1 - P(\text{All Distinct})$$
    

2. Calculating "All Distinct" (The Chain Rule)

Imagine filling the slots one by one. The numerator decreases by 1 each time (options remaining), while the denominator stays constant (total options).

-   **Variables:**
    
    -   $N$: Total options (e.g., 50 products)
        
    -   $k$: Number of trials/people (e.g., 5 students)
        
-   Formula:
    
    $$P(\text{All Distinct}) = \frac{N}{N} \cdot \frac{N-1}{N} \cdot \frac{N-2}{N} \cdot \dots \cdot \frac{N-(k-1)}{N}$$
    
-   Example ($N=50, k=5$):
    
    $$P = \frac{50}{50} \cdot \frac{49}{50} \cdot \frac{48}{50} \cdot \frac{47}{50} \cdot \frac{46}{50}$$
    

3. Conditional Evolution (Step-by-Step)

If you need to calculate the probability as the group grows (like in Part b), calculate the cumulative probability for group size $n$.

-   Recursion Concept:
    
    $$P(\text{Distinct}_{n}) = P(\text{Distinct}_{n-1}) \cdot \frac{N-(n-1)}{N}$$
    
-   Collision Probability for size $n$:
    
    $$P_{n} = 1 - \left( \frac{N}{N} \cdot \dots \cdot \frac{N-n+1}{N} \right)$$
    

4. General Approximation (For Large N)

(Optional, but good for physics exams)

For large $N$ and small $k$, the probability of "All Distinct" can be approximated using the exponential function:

$$P(\text{All Distinct}) \approx e^{-k^2 / (2N)}$$

$$P(\text{Collision}) \approx 1 - e^{-k^2 / (2N)}$$

(Note: This specific problem used exact fractions, but this is the standard statistical physics approximation for this type of problem).

---

**Would you like to continue to the next problem in the uploaded file? It looks like it involves flight failures and infinite sums!**

