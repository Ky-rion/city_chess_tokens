

Excellent! Let's move on to **part (b)**. This is one of the most famous calculations in statistical mechanics, first performed by the Nobel laureate Linus Pauling in 1935.

We are now zooming out from a single tetrahedron to the entire crystal lattice. The question asks us to find the entropy of the whole crystal, assuming the tetrahedra act "independently" (a key simplifying assumption known as the Pauling approximation).

---

### Part (b): Entropy of the Water Ice Crystal

We need to count the total number of valid ways ($\Omega_{\text{total}}$) to arrange the protons in a crystal of $N$ molecules so that _every_ Oxygen atom satisfies the "2-in, 2-out" rule.

#### 1. Counting the Total Hydrogen Positions

First, imagine the crystal structure without any rules.

-   Let's say we have **$N$ Oxygen atoms** (molecules).
    
-   Since each Oxygen is connected to 4 others, and each bond is shared between 2 Oxygens, the total number of hydrogen bonds in the crystal is **$2N$**.
    
-   On each bond, the Hydrogen atom has exactly **2** possible positions: it can be close to one end or the other.
    

If there were no restrictions, the total number of arrangements would simply be $2^{\text{total bonds}}$:

$$\Omega_{\text{unconstrained}} = 2^{2N} = (2^2)^N = 4^N$$

#### 2. Applying the "Ice Rule" Probability

Now we apply the constraint. We know from **part (a)** that for any single Oxygen atom, there are $2^4 = 16$ possible ways to arrange the 4 surrounding protons if we ignore the neighbors.

-   However, only **6** of these 16 ways satisfy the Ice Rule (2-in, 2-out).
    

Therefore, the probability that a randomly chosen Oxygen atom satisfies the rule is:

$$P_{\text{valid}} = \frac{6}{16} = \frac{3}{8}$$

#### 3. The "Independence" Approximation

The problem states "assuming each tetrahedron _independently_ fulfills the Ice-Rule". This is the key. It allows us to simply multiply the probabilities.

To find the total number of valid states for the whole crystal ($\Omega_{\text{crystal}}$), we take the total unconstrained arrangements and multiply by the probability that _all_ $N$ atoms satisfy the rule:

$$\Omega_{\text{crystal}} = \Omega_{\text{unconstrained}} \times (P_{\text{valid}})^N$$

$$\Omega_{\text{crystal}} = 4^N \times \left(\frac{3}{8}\right)^N$$

Let's do the algebra:

$$\Omega_{\text{crystal}} = 4^N \times \frac{3^N}{8^N} = \frac{4^N \times 3^N}{(2 \cdot 4)^N} = \frac{4^N \times 3^N}{2^N \times 4^N} = \frac{3^N}{2^N}$$

$$\Omega_{\text{crystal}} = \left(\frac{3}{2}\right)^N$$

Your professor's notes arrive at this same result on Page 7, showing the final calculation $\Omega = (3/2)^N$ (derived there using a slightly more complex counting argument involving "red and blue" sub-lattices to justify the independence).

#### 4. The Statistical Entropy

Now we calculate the entropy using $S = k_B \ln \Omega_{\text{crystal}}$.

$$S = k_B \ln \left[ \left(\frac{3}{2}\right)^N \right]$$

$$S = N k_B \ln \left(\frac{3}{2}\right)$$

Or, the specific entropy per molecule (dividing by $N$):

$$s = k_B \ln(1.5)$$

The notes explicitly state this result: "$S = \ln \frac{3}{2}$".

---

### Interpretation: The Third Law of Thermodynamics

The second part of the question asks you to interpret this result in the context of the **Third Law of Thermodynamics**.

The Conflict:

The Third Law states that the entropy of a perfect crystal should approach zero as the temperature approaches absolute zero ($T \to 0$).

$$\lim_{T \to 0} S = 0$$

This is because, usually, a substance at absolute zero settles into a single, unique ground state ($\Omega = 1$, so $\ln \Omega = 0$).

The Resolution (Residual Entropy):

Our result shows that for ice, $S \neq 0$.

$$S_{T=0} = N k_B \ln(1.5) > 0$$

This is called **Residual Entropy**.

-   **Degeneracy:** Even at absolute zero, the Hydrogen atoms in ice do not settle into a single unique pattern. There are roughly $(1.5)^N$ equally valid ways to arrange the protons that all have the same minimum energy.
    
-   **"Frozen" Disorder:** As water freezes, the protons get "stuck" in one of these many random valid configurations. The crystal is ordered in terms of Oxygen positions (the lattice), but _disordered_ in terms of Hydrogen positions.
    

Your professor's notes summarize this perfectly:

> "At T=0 we hence have specific entropy... $\neq 0$. But this only means that the energy is degenerate!".

So, ice is a fascinating exception where the "practical" entropy does not vanish at zero temperature because the system cannot find a unique ordered state.

**Does this make sense? It's a very famous result that matches experimental data almost perfectly!**

