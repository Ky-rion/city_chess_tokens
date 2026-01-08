

Welcome back! I am so glad you asked for the details on this one. This part of the problem (Problem 2b) is an absolute classic. It introduces a mathematical "trick" that we use constantly in statistical mechanics and thermodynamics.

Let's put on our theoretical physics hats. We are looking for the **Expected Value** (or mean) of the number of successful flights.

### 1. Setting up the "Ensemble"

To find an average (expected value), we need two things:

1.  **The value:** $k$ (the number of successful flights).
    
2.  **The probability of that value:** $P(k)$.
    

We established in part (a) that surviving $k$ flights has probability $q^k$. But for the **expectation**, we need the probability that the streak ends _exactly_ after $k$ flights. This means you survived $k$ times ($q^k$) AND then failed on the next one ($p$).

So, our probability distribution is:

$$P(k) = q^k \cdot p$$

_(Note: In probability theory, this is known as the **Geometric Distribution**.)_

### 2. The Definition of Expected Value

The symbol for expected value in physics is often written with angle brackets: $\langle k \rangle$. The definition is simply the sum of every possible outcome multiplied by its probability.

$$\langle k \rangle = \sum_{k=0}^{\infty} k \cdot P(k) = \sum_{k=1}^{\infty} k \cdot q^k \cdot p$$

_(Note: We can start the sum at $k=1$ because if $k=0$, the term is $0 \cdot P(0) = 0$, so it doesn't add anything)._

### 3. The "Professor's Trick" (The Derivative Method)

Now, look at how your professor solves this summation in the notes. You _could_ try to solve this sum brute-force, but physicists love shortcuts.

We need to sum terms that look like $k \cdot q^k$. The trick is to realize that $k \cdot q^k$ looks suspiciously like a derivative.

$$k \cdot q^k = q \cdot \frac{d}{dq} (q^k)$$

Why? Because $\frac{d}{dq}(q^k) = k \cdot q^{k-1}$. Multiply that by $q$, and you get $k \cdot q^k$.

This allows us to pull the derivative outside the summation!

$$\langle k \rangle = p \sum_{k=1}^{\infty} k q^k = p \cdot q \frac{d}{dq} \left( \sum_{k=1}^{\infty} q^k \right)$$

Do you see the beauty of this? Instead of summing a complicated $k \cdot q^k$, we just have to sum a simple geometric series $q^k$, and then take a derivative at the end.

### 4. Solving the Geometric Series

Now we focus on the inner part: $\sum_{k=1}^{\infty} q^k$.

This is an infinite geometric series. Since $q < 1$ (it's a probability), the formula is:

$$\sum_{k=1}^{\infty} q^k = \frac{q}{1-q}$$

### 5. Bringing it all together

Now we substitute this back into our equation with the derivative:

Step A: Differentiate

We need $\frac{d}{dq} \left( \frac{q}{1-q} \right)$. Using the quotient rule (or just chain rule):

$$\frac{d}{dq} \left( \frac{q}{1-q} \right) = \frac{1}{(1-q)^2}$$

(The notes skip a tiny step here, but if you work it out, the result is $1/(1-q)^2$).

Step B: Multiply by the constants

Remember we had a $p \cdot q$ sitting outside the derivative.

$$\langle k \rangle = p \cdot q \cdot \left[ \frac{1}{(1-q)^2} \right]$$

Step C: Simplify using $q = 1-p$

Since $1-q = p$, the denominator becomes $p^2$.

$$\langle k \rangle = \frac{p \cdot q}{p^2} = \frac{q}{p}$$

### 6. The Final Answer

Substituting $q = 1-p$ back in, we get the final result shown in the notes:

$$\langle k \rangle = \frac{1-p}{p}$$

### Professor's Interpretation

This result makes intuitive sense!

-   If the probability of failure $p$ is tiny (e.g., $0.01$ or 1%), then $1/p$ is large (100).
    
-   The expected number of safe flights is roughly $1/p$.
    
-   Strictly speaking, it is $(1/p) - 1$, because we are counting _successful_ flights, not the flight number of the crash.
    

**Would you like me to tackle the next part (Problem 2c), which gets much more involved with "entropy" and finding the safest configuration?**