

We are now looking at **Part (b)**, where the rules of the game change slightly to add a bit of suspense!

In this scenario, you are the **last person** to open your gift. You watch your four friends open their packages one by one, and remarkably, **every single one of them reveals a different, unique gift**.

The question asks: **How does the probability that "at least one product has been gifted twice" change as this process unfolds?**

Let's break this down step-by-step, just like in the handwritten solution.

### 1. The New Perspective

In Part (a), we calculated the probability _before_ anyone opened anything. Now, we are updating our prediction _live_ as information becomes available. This is a classic example of **conditional probability**.

We are still looking for the probability of the event $E_1$ ("At least two gifts are the same"), but the condition changes after each friend opens a unique gift.

Let $n$ be the number of people who have opened their gifts so far.

-   The total number of available product types remains $N = 50$.
    
-   We are interested in the probability $P_{n}$ that a collision (a match) occurs among the group of size $n$.
    

However, the problem statement says "While your fellow students open their packages and **always find different content**...". This implies we are looking at the probability of a collision happening _specifically for the next person or the total group_ given the previous ones were distinct.

The solution sheet actually calculates the probability of a collision _within a group of size $n$_, given the previous $(n-1)$ people didn't collide. Let's trace that logic.

### 2. Step-by-Step Evolution

The handwritten notes provide a formula for the probability of a collision for a group of size $n$, denoted as $P_{n}$.

The formula used is the same complementary logic as Part (a):

$$P_{n} = 1 - P(\text{all } n \text{ gifts are distinct})$$

Let's calculate this for each stage as the group grows:

**Stage 1: The First Student ($n=1$)**

-   The first student opens a gift.
    
-   Can they collide with anyone? No, they are the only one!
    
-   Probability of collision: $P_{n=1} = 0$.
    

**Stage 2: The Second Student ($n=2$)**

-   Student 1 has a specific gift.
    
-   Student 2 opens their gift. For them _not_ to match Student 1, they must pick one of the 49 remaining types out of 50.
    
-   $P(\text{distinct}) = \frac{49}{50} = 0.98$
    
-   Probability of collision:
    
    $$P_{n=2} = 1 - 0.98 = 0.02$$
    
-   So, a **2%** chance of a match so far.
    

**Stage 3: The Third Student ($n=3$)**

-   Students 1 and 2 have distinct gifts.
    
-   Student 3 must pick from the remaining 48 types to avoid a match.
    
-   $P(\text{distinct}) = \frac{49}{50} \cdot \frac{48}{50}$
    
-   The notes calculate this as:
    
    $$P_{n=3} = 1 - (0.98 \cdot 0.96) \approx 1 - 0.941 = 0.059$$
    
-   Roughly **5.9%** chance. (The notes round this to **0.06**).
    

**Stage 4: The Fourth Student ($n=4$)**

-   Students 1, 2, and 3 have distinct gifts.
    
-   Student 4 must pick from the remaining 47 types.
    
-   $P(\text{distinct}) = \frac{49}{50} \cdot \frac{48}{50} \cdot \frac{47}{50}$
    
-   Calculation:
    
    $$P_{n=4} = 1 - (0.98 \cdot 0.96 \cdot 0.94) \approx 1 - 0.885 = 0.115$$
    
-   Roughly **11.5%** chance. (The notes approximate this as **0.12** or **0.14** depending on rounding in intermediate steps, but 11.5% is the precise value).
    

**Stage 5: You (The Fifth Student) ($n=5$)**

-   This brings us back to the full group size we calculated in Part (a).
    
-   If the first 4 students definitely have unique gifts (which the problem states they do), does your probability change?
    
    -   Actually, the probability for the _entire group_ is fixed at the start.
        
    -   But if we interpret the question as "What is the probability _you_ create a collision given the others didn't?", the math is simply: You have 4 people with gifts, so 4 "forbidden" items. You have a $4/50$ chance of hitting one of them.
        
    -   $4/50 = 0.08$.
        
-   However, the notes calculate $P_{n=5}$ as the cumulative probability for the whole group, which matches our answer from Part (a):
    
    $$P_{n=5} = 1 - \frac{46}{50} \dots \approx 0.18$$
    

Wait, let's look closer at the specific line in the solution notes for $n=5$ (labeled $P_{n=5}$ or similar):

The note says: $P_{n=5} = 1 - \dots \approx 0.18$.

There seems to be a slight typo in the student's handwritten note where they write $P_{n=4} = 1 - \dots = 0.14$ and then $P_{n=5} = \dots = 0.08$.

-   The value **0.08** ($8\%$) corresponds to the probability of **just the 5th person** crashing the party (colliding) given the first 4 were safe ($4/50$).
    
-   The value **0.18** ($18\%$) corresponds to the probability of **the whole group** having a collision (Part a).
    

Given the phrasing "How does the probability... change?", it implies we are tracking the cumulative risk of the group as it grows.

### 3. Summary of the Evolution

Here is how the probability of "at least one pair matches" evolves as the group size $n$ increases from 1 to 5:

![[Pasted image 20260102130031.png]]

Conclusion:

The probability starts at 0 and grows non-linearly. It essentially triples from $n=2$ to $n=3$, and doubles again by $n=4$. By the time it is your turn ($n=5$), there is an 18.5% chance that someone in the group has the same gift as someone else.

If the question implies "What is the chance _you_ specifically force a match, knowing the others didn't?", that probability is simply $\frac{4}{50} = \mathbf{8\%}$. The handwritten notes seem to calculate the cumulative probabilities first, but the final number "0.08" suggests the "conditional" interpretation for the final step.

**Would you like to analyze the next problem about the flight failures ($A2$)? That one introduces some interesting infinite sums!**