

Hello! It is wonderful to have you in my office hours. Please, pull up a chair. It is always a delight to see a student curious about the underlying mechanics of probability—after all, Statistical Physics is essentially just probability theory applied to atoms and molecules!

Let's look at this "Secret Santa" problem (or _Weihnachtswichteln_, as your German exercise calls it). It is actually a classic example of what we physicists often call the **Birthday Paradox**, just disguised with gifts instead of birthdays.

Here is how we tackle **Part (a)**.

### 1. The Setup

First, let's translate the physical situation into a mathematical model.

According to the problem text:

-   **The System:** There are **5 participants** (you plus 4 fellow students).
    
-   **The State Space:** The shop offers **50 different products**.
    
-   **The Condition:** The shop has infinite stock ("always in stock"), meaning every student chooses independently from the full set of 50.
    

The question asks for the probability of the event $E_1$: **"At least two participants receive the same gift."**

### 2. The Physicist's Trick: Complementary Probability

In statistical mechanics, we often look for the "easy path." Calculating the probability of "at least one pair" directly is messy. You would have to calculate the odds of exactly one pair matching, plus exactly two pairs matching, plus three of a kind, etc. It is a combinatorial nightmare!

Instead, we use a trick shown in your professor's notes. We calculate the probability of the **opposite event** (the complement) and subtract it from 1.

-   Let $E_1$ be the event: **At least two gifts are the same.**
    
-   Let $E_2$ (or $\bar{E_1}$) be the event: **All gifts are distinct (everyone gets something different).**
    

Since these are the only two possibilities, their probabilities must add up to 100%:

$$P(E_1) = 1 - P(E_2)$$

### 3. Calculating the "All Distinct" Event ($E_2$)

Now, let's look at the handwritten solution to see how we calculate $P(E_2)$, the probability that everyone picks a unique gift.

Imagine the 5 students walking into the shop one by one:

1.  **Student 1:** Can pick _any_ gift. They have 50 choices out of 50. The probability that they pick a "valid" gift (one that hasn't been picked yet) is $\frac{50}{50}$ (or 100%).
    
2.  **Student 2:** To avoid a collision, they must pick one of the remaining 49 "untouched" gifts. They have 49 choices out of 50. Probability: $\frac{49}{50}$.
    
3.  **Student 3:** Must pick from the remaining 48. Probability: $\frac{48}{50}$.
    
4.  **Student 4:** Must pick from the remaining 47. Probability: $\frac{47}{50}$.
    
5.  **Student 5:** Must pick from the remaining 46. Probability: $\frac{46}{50}$.
    

To get the total probability of _all_ these happening in sequence, we multiply them together:

$$P(E_2) = \frac{50}{50} \cdot \frac{49}{50} \cdot \frac{48}{50} \cdot \frac{47}{50} \cdot \frac{46}{50}$$

The handwritten note writes this out clearly in line.

### 4. The Final Result

Now we just plug this back into our first equation.

The notes show the calculation results in approximately $0.184$.

$$P(E_1) = 1 - (1 \cdot 0.98 \cdot 0.96 \cdot 0.94 \cdot 0.92)$$

$$P(E_1) \approx 1 - 0.815$$

$$P(E_1) \approx 0.185$$

Your professor's solution notes the final answer as **0.184** (or 18.4%).

### Summary

Even with 50 options to choose from, if you have just 5 people, there is nearly a **1 in 5 chance** that two of you will end up with the same present! This is why "collisions" in phase space (or hash tables in computer science) happen much more often than our intuition suggests.

---

**Would you like to move on to Part (b), where we analyze what happens as more people join the group?**