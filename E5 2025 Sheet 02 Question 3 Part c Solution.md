

Hello again! This is a fantastic question and a classic exercise. It's where we move from just _describing_ the nucleus to _predicting_ its properties.

Let's derive this, step-by-step.

### 🎯 Our Goal

The question asks for the **"stable isobar"**.

-   **Isobar:** This is a family of nuclei that all have the same **total mass number $A$**, but different numbers of protons ($Z$) and neutrons ($N$). For example, Carbon-14 ($A=14, Z=6$) and Nitrogen-14 ($A=14, Z=7$) are isobars.
    
-   **Stable:** In this context, "stable" means the nucleus that is the most tightly bound, which means it has the **highest binding energy $B$**.
    

The prompt tells us exactly how to find this:

1.  Get the formula for the binding energy per nucleon, $B/A$.
    
2.  Find the $Z$ value that _maximizes_ this function (which is what "defining the extrema" means).
    
3.  In calculus, we find a maximum by taking the derivative with respect to our variable ($Z$) and setting that derivative equal to zero.
    

So, our mathematical goal is to solve this equation:

$$\frac{\partial}{\partial Z} \left( \frac{B}{A} \right) = 0$$

---

### Step 1: Write Down the Formula for $B(A,Z)$

First, let's get the binding energy, $B$. In your first image, the formula is for the _mass_ $M(A,Z)$. The binding energy $B$ is the energy _released_ when the nucleus is formed, which means it's the _negative_ of those five terms in the parenthesis (since they are _added_ to the mass of the parts).

So, the binding energy $B$ is:

$$B(A,Z) = a_V A - a_O A^{2/3} - a_C \frac{Z^2}{A^{1/3}} - a_A \frac{(N-Z)^2}{A} - a_P \frac{\delta}{A^{1/2}}$$

(Note the sign change: the attractive Volume term is positive, while the repulsive Surface, Coulomb, etc. terms are negative, reducing the binding).

The prompt asks for binding energy per nucleon, $B/A$. So, we just divide the whole expression by $A$:

$$\frac{B(A,Z)}{A} = a_V - a_O A^{-1/3} - a_C \frac{Z^2}{A^{4/3}} - a_A \frac{(N-Z)^2}{A^2} - a_P \frac{\delta}{A^{3/2}}$$

### Step 2: Prepare the Equation for Differentiation

Our derivative is with respect to $Z$. We need to replace the $N$ in the asymmetry term with an expression involving $Z$ and our constant, $A$.

We know: $N = A - Z$

Let's substitute this into the asymmetry term: $(N-Z)^2$

$$(N-Z)^2 = ((A-Z) - Z)^2 = (A - 2Z)^2$$

Now, let's put this back into our $B/A$ equation:

$$\frac{B(A,Z)}{A} = a_V - a_O A^{-1/3} - a_C \frac{Z^2}{A^{4/3}} - a_A \frac{(A-2Z)^2}{A^2} - a_P \frac{\delta}{A^{3/2}}$$

### Step 3: Take the Derivative with Respect to $Z$

We are now ready to calculate $\frac{\partial}{\partial Z} \left( \frac{B}{A} \right)$. Remember, we are treating $A$ as a **constant** and $Z$ as our **variable**.

$$\frac{\partial}{\partial Z} \left[ a_V - a_O A^{-1/3} - a_C \frac{Z^2}{A^{4/3}} - a_A \frac{(A-2Z)^2}{A^2} - a_P \frac{\delta}{A^{3/2}} \right] = 0$$

Let's go term by term:

1.  $\frac{\partial}{\partial Z} (a_V) = 0$ (it's a constant)
    
2.  $\frac{\partial}{\partial Z} (-a_O A^{-1/3}) = 0$ (it's a constant)
    
3.  $\frac{\partial}{\partial Z} \left(-a_C \frac{Z^2}{A^{4/3}}\right) = -\frac{a_C}{A^{4/3}} \cdot (2Z)$ (using the power rule)
    
4.  $\frac{\partial}{\partial Z} \left(-a_A \frac{(A-2Z)^2}{A^2}\right) = -\frac{a_A}{A^2} \cdot \left[ 2(A-2Z) \cdot (-2) \right]$ (using the chain rule!)
    
    -   This simplifies to: $+\frac{4 a_A (A-2Z)}{A^2}$
        
5.  $\frac{\partial}{\partial Z} \left(-a_P \frac{\delta}{A^{3/2}}\right) = 0$ (the prompt tells us to assume $\delta$ is constant)
    

Now, let's put the non-zero terms together and set them to 0:

$$-\frac{2 a_C Z}{A^{4/3}} + \frac{4 a_A (A-2Z)}{A^2} = 0$$

### Step 4: Solve the Equation for $Z$

This is the final step! We just need to do some algebra to isolate $Z$.

1.  Move one term to the other side:
    
    $$\frac{4 a_A (A-2Z)}{A^2} = \frac{2 a_C Z}{A^{4/3}}$$
    
2.  Let's simplify. We can divide both sides by 2:
    
    $$\frac{2 a_A (A-2Z)}{A^2} = \frac{a_C Z}{A^{4/3}}$$
    
3.  Now, let's get $Z$ out of the parenthesis. Multiply both sides by $A^2$ to clear the left denominator:
    
    $$2 a_A (A-2Z) = \left( \frac{a_C Z}{A^{4/3}} \right) \cdot A^2$$
    
4.  Simplify the $A$ terms on the right side. Remember that $\frac{A^2}{A^{4/3}} = A^{(2 - 4/3)} = A^{(6/3 - 4/3)} = A^{2/3}$.
    
    $$2 a_A (A-2Z) = a_C Z A^{2/3}$$
    
5.  Expand the left side:
    
    $$2 a_A A - 4 a_A Z = a_C Z A^{2/3}$$
    
6.  Our goal is to get all terms with $Z$ on one side and all terms without $Z$ on the other.
    
    $$2 a_A A = 4 a_A Z + a_C Z A^{2/3}$$
    
7.  Factor out the $Z$ on the right side:
    
    $$2 a_A A = Z (4 a_A + a_C A^{2/3})$$
    
8.  Finally, divide to solve for $Z$:
    
    $$Z = \frac{2 a_A A}{4 a_A + a_C A^{2/3}}$$
    

---

### 🏁 Conclusion

And there we have it! This is the formula to calculate the most stable proton number $Z$ for a given mass number $A$.

This equation beautifully shows the "tug-of-war" inside the nucleus. The stable $Z$ is a balance between:

-   The **Asymmetry term** (represented by $a_A$), which wants $N=Z$ (or $Z = A/2$). You can see that if $a_C$ were zero, the formula would simplify to $Z = \frac{2 a_A A}{4 a_A} = \frac{A}{2}$.
    
-   The **Coulomb term** (represented by $a_C$), which _hates_ protons. This force pushes the stable $Z$ to be _less_ than $A/2$, favoring more neutrons (which are neutral) to space out the repelling protons. This is why the $a_C$ term is in the denominator, making $Z$ smaller.
    

This line of $Z$ vs $A$ on a chart of all nuclei is called the **"line of stability"**.

---

### 👨‍🏫 A Quick Professor's Note on the Method

The prompt _specifically_ told us to maximize $B/A$. This is a very common simplification and leads to a great result.

In a more advanced treatment, we would find the most stable nucleus by finding the one with the _minimum mass_ $M(A,Z)$. This means we would solve $\frac{\partial M}{\partial Z} = 0$.

If we do that, we get a slightly different result because the mass formula _also_ includes the $N m_n + Z m_p$ part. This adds a small constant from the neutron-proton mass difference. Your problem's method is a very standard and useful approximation that assumes the proton and neutron have the same mass (or, more precisely, that we can ignore the effect of their mass difference on the derivative). It's an excellent simplification!

Does it make sense how we used calculus to find the most stable configuration? We can move on to another part if you're ready!