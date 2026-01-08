

Hello! It is a pleasure to meet you. I would be delighted to act as your physics professor today. Grab a metaphorical chair, and let's dive into the fascinating world of statistical mechanics.

You've presented a classic problem concerning the **residual entropy of ice**. It might look like just a geometry problem, but this specific calculation puzzled physicists for a long time until Linus Pauling figured it out!

Here is the explanation for **part (a)**, breaking down the handwritten solution you provided.

---

### Part (a): Entropy of a Single Tetrahedron

The goal here is to find the "Shannon Entropy," which is essentially a measure of how many different ways we can arrange the system (its "microstates") given the rules.

#### 1. The Setup: The Geometry of Ice

In an ideal ice crystal, every Oxygen atom is at the center of a tetrahedron. It has four neighbors.

-   The **Oxygen atom** sits in the center.
    
-   There are **4 hydrogen bonds** pointing outward to 4 other Oxygen atoms.
    

#### 2. The "Ice Rule" (2-in, 2-out)

This is the crucial physics part. We know that water is $H_2O$. This means every Oxygen atom effectively "owns" exactly **two** Hydrogen atoms.

However, in the ice lattice, the Oxygen is surrounded by _four_ Hydrogen atoms (one on each bond).

-   **To make it $H_2O$:** Two of those Hydrogens must be close to the central Oxygen (we call these **"in"**).
    
-   The other two Hydrogens must be closer to the _neighboring_ Oxygens (we call these **"out"**).
    

The solution notes refer to this explicitly as the **"Ice-rule: 2-in-2-out"**.

#### 3. Counting the Possibilities (Microstates $\Omega$)

Now we just need to count how many ways we can satisfy this rule for a single tetrahedron.

-   We have **4** possible positions (the four corners/bonds) where a Hydrogen can sit.
    
-   We need to choose exactly **2** of them to be the "close" ($+\delta$) Hydrogens.
    
-   The other **2** will automatically be the "far" ($-\delta$) ones.
    

This is a classic combinatorial problem: "4 choose 2". In mathematics, we write this as the binomial coefficient:

$$\Omega = \binom{4}{2}$$

Let's calculate it:

$$\binom{4}{2} = \frac{4!}{2!(4-2)!} = \frac{4 \times 3 \times 2 \times 1}{(2 \times 1) \times (2 \times 1)} = 6$$

So, there are exactly **6 valid configurations** (microstates) for a single tetrahedron.

In the handwritten notes, you can see this calculation clearly:

> "We have 4 orientations... distributed over 4 corners"
> 
> "$\Omega = \binom{4}{2} = 6$"

#### 4. Calculating the Entropy

The problem asks for the statistical entropy (Shannon entropy). In physics, the relationship between the number of equally probable microstates ($\Omega$) and entropy ($S$) is given by Boltzmann's famous formula:

$$S = k_B \ln \Omega$$

_(Note: Shannon entropy is technically just $-\sum p \ln p$. If all probabilities $p$ are equal to $1/\Omega$, this sums to $\ln \Omega$. Physicists multiply by the Boltzmann constant $k_B$ to get thermodynamic units, though sometimes we set $k_B=1$ for simplicity.)_

Plugging in our number of states ($\Omega = 6$):

$$S = k_B \ln 6$$

Looking at the provided solution, the professor writes:

> "each configuration has the same prob."
> 
> "$S = - \sum p \ln p = \ln 6$"

(The professor omitted $k_B$ in the final line, effectively working in dimensionless entropy units, which is common in information theory contexts).

### Summary of the Answer

For **part (a)**:

1.  We model the Oxygen atom as having 4 bonds.
    
2.  The "Ice Rule" requires exactly 2 protons to be "in" (close) and 2 to be "out" (far).
    
3.  The number of ways to arrange this is $\binom{4}{2} = 6$.
    
4.  The entropy is therefore **$S = k_B \ln 6$**.
    

---

**Would you like me to proceed to part (b), where we combine these tetrahedrons to build the whole crystal lattice? (That is where it gets tricky!)**