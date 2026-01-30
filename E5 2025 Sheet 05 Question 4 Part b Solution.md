

![[Pasted image 20260128115124.png]]

Welcome back! I am glad you are finding the material interesting. This is where particle physics starts to feel like real detective work—we are taking general concepts and applying them to specific, real-world models like the Lithium nucleus.

In Part (a), we built our "measuring tool": the formula for the mean squared radius.

In Part (b), we are going to **use** that tool on a specific target: a nucleus shaped like a Gaussian cloud.

Let's walk through the solution step-by-step.

### 1. Recall our Tool (from Part a)

From the previous question, we derived this formula for calculating the size of a spherical nucleus:

$$\langle r^2 \rangle = 4\pi \int_0^\infty r^4 f(r) \, dr$$

We also have our specific **Shape Function** ($f(r)$) for this problem, which is a Gaussian distribution:

$$f(r) = \underbrace{\left( \frac{a^2}{2\pi} \right)^{3/2}}_{\text{Constant } C} \cdot \exp\left( -\frac{a^2 r^2}{2} \right)$$

Think of the term in the brackets as a normalization constant (let's call it $C$ for now so we don't get overwhelmed). It ensures the total probability is 1. The interesting physics is in the $\exp(...)$ term, which describes the bell-curve shape of the charge.

---

### 2. Setting up the Integral

Now, we substitute our specific $f(r)$ into our general formula.

$$\langle r^2 \rangle = 4\pi \cdot \underbrace{\left( \frac{a^2}{2\pi} \right)^{3/2}}_{\text{Constant}} \cdot \int_0^\infty r^4 \exp\left( -\frac{a^2 r^2}{2} \right) \, dr$$

This looks intimidating! But in physics, we rarely solve these integrals from scratch. We use "lookup tables" or standard integrals. That is what the **Hint** in the problem is for.

---

### 3. Using the Hint (The "Lookup Table")

The problem gives us the general solution for integrals of this type:

$$\int_0^\infty x^n \exp(-bx^2) \, dx = \frac{\Gamma\left( \frac{n+1}{2} \right)}{2 b^{\left( \frac{n+1}{2} \right)}}$$

We need to map our "messy" physics variables to the "clean" math variables in the hint.

-   **The variable:** Our $r$ corresponds to $x$.
    
-   **The power ($n$):** We have $r^4$, so **$n = 4$**.
    
-   **The exponential constant ($b$):** We have $\exp(-\frac{a^2}{2}r^2)$, so **$b = \frac{a^2}{2}$**.
    

Now we plug these into the right side of the hint equation.

First, look at the exponent term $\frac{n+1}{2}$. Since $n=4$:

$$\frac{4+1}{2} = \frac{5}{2} = 2.5$$

So the integral part becomes:

$$\text{Integral Result} = \frac{\Gamma(5/2)}{2 \cdot (a^2/2)^{5/2}}$$

---

### 4. Solving the Gamma Function ($\Gamma$)

The Gamma function, $\Gamma(z)$, is basically a factorial for non-integer numbers. The hint gives us a specific formula for half-integers:

$$\Gamma\left( z + \frac{1}{2} \right) = \frac{(2z)! \cdot \sqrt{\pi}}{z! \cdot 2^{2z}}$$

We need $\Gamma(5/2)$. We can write $5/2$ as $2 + 1/2$.

So, we set **$z = 2$**.

Now, let's plug $z=2$ into the formula:

-   **Numerator:** $(2 \cdot 2)! \cdot \sqrt{\pi} = 4! \cdot \sqrt{\pi} = 24\sqrt{\pi}$
    
-   **Denominator:** $2! \cdot 2^{2 \cdot 2} = 2 \cdot 2^4 = 2 \cdot 16 = 32$
    

So:

$$\Gamma(5/2) = \frac{24\sqrt{\pi}}{32} = \frac{3\sqrt{\pi}}{4}$$

_(Note: The solution image writes this as $\frac{24\sqrt{\pi}}{2 \cdot 16}$)_

---

### 5. Bringing it all together (The Algebra)

Now we combine _everything_.

1.  The $4\pi$ from the original formula.
    
2.  The normalization constant $\left( \frac{a^2}{2\pi} \right)^{3/2}$.
    
3.  The result of the integral we just found.
    

$$\langle r^2 \rangle = 4\pi \cdot \left( \frac{a^2}{2\pi} \right)^{3/2} \cdot \left[ \frac{\Gamma(5/2)}{2(a^2/2)^{5/2}} \right]$$

This is the "messy" middle step in the solution image. Let's simplify it by grouping similar terms.

**Group the $\pi$ terms:**

-   Numerator: $\pi$ (from $4\pi$) and $\sqrt{\pi}$ (from Gamma). Total: $\pi^{3/2}$.
    
-   Denominator: $\pi^{3/2}$ (from the normalization constant).
    
-   **Result:** The $\pi$ terms cancel out perfectly!
    

**Group the number constants:**

-   Numerator: $4$ (from $4\pi$) $\times$ $3/4$ (from Gamma factor).
    
-   Denominator: There are various factors of 2.
    
    -   Let's look at the solution image's second-to-last line. They expand everything out to be safe:
        
        $$\frac{4 \cdot 24 \cdot \dots}{32 \cdot 2 \dots}$$
        
    -   Let's do it a simpler way. Look at the variable $a$.
        

**Group the $a$ terms:**

-   Numerator: $(a^2)^{3/2} = a^3$.
    
-   Denominator: The integral result has $b^{5/2} = (a^2/2)^{5/2}$. The $a$ part is $(a^2)^{5/2} = a^5$.
    
-   Total $a$ dependence: $\frac{a^3}{a^5} = \frac{1}{a^2}$.
    

**Group the remaining numbers:**

If you carefully cancel the $2$'s and other numbers as shown in the solution image (lines 4 and 5), you are left with just a $3$ on top and a $2$ on the bottom.

$$\text{Final Answer: } \langle r^2 \rangle = \frac{3}{2 a^2}$$

_(Note: The solution image writes this as $\frac{3}{a^2}$ but has a distinct "$2$" in the denominator in the final line. Wait, looking closely at the image, the final line is just $\frac{3}{a^2}$. Let me double-check the math for you to ensure the professor's notes are right!)_

**Double Check:**

$$\langle r^2 \rangle = 4\pi \left(\frac{a^3}{(2\pi)^{3/2}}\right) \frac{1}{2(a^2/2)^{5/2}} \frac{3\sqrt{\pi}}{4}$$

$$= \pi \frac{a^3}{(2\pi)^{3/2}} \frac{2^{5/2}}{a^5} \frac{3\sqrt{\pi}}{2}$$

$$= \pi \cdot \frac{a^3}{2^{3/2}\pi^{3/2}} \cdot \frac{2^{5/2}}{a^5} \cdot \frac{3\pi^{1/2}}{2}$$

Combine powers of 2: $\frac{2^{5/2}}{2^{3/2} \cdot 2^1} = \frac{2^{2.5}}{2^{2.5}} = 1$. (The 2s cancel perfectly!)

Combine powers of $\pi$: $\frac{\pi^1 \cdot \pi^{1/2}}{\pi^{3/2}} = 1$. (The $\pi$s cancel perfectly!)

Combine powers of $a$: $\frac{a^3}{a^5} = \frac{1}{a^2}$.

Remaining numbers: Just the **3**.

**Correction:**

My manual calculation suggests the answer is $\frac{3}{a^2}$.

Let's look at the professor's image again. The final line is $\frac{3}{a^2}$. However, the line before that shows $\frac{32 \cdot a^2}{...}$.

Actually, looking at the very last line of the solution image:

$$= \frac{3}{a^2}$$

But wait, standard Gaussian variance is usually related to $1/a$. Let's look at the distribution definition. The exponent is $-a^2 r^2 / 2$. This is equivalent to $-r^2 / (2\sigma^2)$ where $\sigma = 1/a$.

For a 3D Gaussian, $\langle r^2 \rangle = \langle x^2 + y^2 + z^2 \rangle = 3\sigma^2$.

Since $\sigma = 1/a$, then $\langle r^2 \rangle = 3/a^2$.

**Conclusion:** The professor's final line is correct! The answer is indeed:

$$\langle r^2 \rangle = \frac{3}{a^2}$$

### What does this mean?

The parameter $a$ determines how "tight" the nucleus is.

-   If $a$ is **large**, $1/a^2$ is small, meaning the radius is small (tightly packed nucleus).
    
-   If $a$ is **small**, the radius is large (fluffy nucleus).
    

This result gives us a direct link between the mathematical parameter $a$ and the physical size of the nucleus!

Would you like to try calculating the radius for a specific value of $a$, or should we move on to the next part of the problem?