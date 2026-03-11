

This is indeed the grand finale, and it has a reputation for being tricky! But don't worry—since we have laid all the groundwork in the previous six parts, you actually have all the puzzle pieces you need to solve it beautifully.

First, let's translate the final prompt:

> **7. Determine the sign of the integral of the exchange term using mathematical arguments. The numerical value of the integral does not need to be calculated, only the sign needs to be determined. [5 Pts.]**

This is asking us to mathematically prove what we just argued physically in Part 6. We want to show that the exchange integral (which we called $K$) is mathematically a **positive number**. _(Because remember, it was subtracted in our energy equation: $\langle V_{12} \rangle = J - K$. If $K$ is mathematically positive, then subtracting it lowers the total energy!)_

Here is how a theoretical physicist constructs this proof step-by-step.

---

### Step 1: Rearranging the Integral

Let's start by looking at our exchange integral $K$ from Part 5. Let's group the terms so that all the $x_1$ functions are together and all the $x_2$ functions are together:

$$K = \iint [\Phi_1(x_1)\Phi_2(x_1)] \left( \frac{1}{\sqrt{1+(x_1-x_2)^2}} \right) [\Phi_1(x_2)\Phi_2(x_2)] dx_1 dx_2$$

To make this easier to read, let's define a new "overlap function", $f(x) = \Phi_1(x)\Phi_2(x)$. Let's also just call our potential $V(x_1, x_2)$. Now our integral looks much cleaner:

$$K = \iint f(x_1) V(x_1, x_2) f(x_2) dx_1 dx_2$$

### Step 2: Analyzing the Overlap Function $f(x)$

Now we need to recall the very first thing we did in this exam: our qualitative sketches from Part 1!

- **The Ground State $\Phi_1(x)$:** This was a smooth bump with 0 nodes. We can assume it is strictly positive everywhere.
    
- **The Excited State $\Phi_2(x)$:** This had exactly 1 node right in the middle (at $x=0$). It was positive on the right side ($x > 0$) and negative on the left side ($x < 0$).
    

When we multiply a strictly positive function by a function that crosses zero, the result $f(x)$ adopts the sign of the crossing function. Therefore:

- When $x$ is positive, $f(x)$ is **positive**.
    
- When $x$ is negative, $f(x)$ is **negative**.
    

### Step 3: Dividing Space into Four Quadrants

We are integrating over all possible positions for both electron 1 ($x_1$) and electron 2 ($x_2$). We can divide this infinite 2D space into four logical regions based on where the electrons are:

1. **Both on the right ($x_1 > 0, x_2 > 0$):** Here, $f(x_1)$ is positive and $f(x_2)$ is positive. Their product is **positive**.
    
2. **Both on the left ($x_1 < 0, x_2 < 0$):** Here, $f(x_1)$ is negative and $f(x_2)$ is negative. A negative times a negative means their product is also **positive**!
    
3. **Opposite sides (One left, one right):** In these two remaining regions, one $f(x)$ is positive and the other is negative. Their product will be **negative**.
    

### Step 4: The Core Mathematical Argument (Distance)

Now we must look at the middle part of our integral: the repulsive potential $V(x_1, x_2) = \frac{1}{\sqrt{1+(x_1-x_2)^2}}$.

This potential strictly depends on the **distance** between the two electrons. The closer they are, the larger the value of $V$. The further apart they are, the smaller the value of $V$.

Let's compare our regions:

- **Same Side (Regions 1 & 2):** When both electrons are on the same side of the origin, the distance between them is relatively small. Therefore, the potential $V$ is evaluated at a **large** positive number.
    
- **Opposite Sides (Region 3):** When one electron is on the far left and the other is on the far right, the distance between them is relatively large. Therefore, the potential $V$ is evaluated at a **small** positive number.
    

### Step 5: The Grand Conclusion

Let's add up the whole integral conceptually:

$$K \approx (\text{Positive Product} \times \text{Large } V) + (\text{Negative Product} \times \text{Small } V)$$

The positive contributions to the integral (when the electrons are on the same side of the atom and close together) are multiplied by a large number. The negative contributions (when the electrons are on opposite sides and far apart) are multiplied by a small number.

Because the positive terms heavily outweigh the negative terms, the total sum must be strictly greater than zero.

- **Final Answer:** Through mathematical analysis of the symmetries and the distance dependence of the potential, we have determined that the sign of the exchange integral $K$ is strictly **positive ($+$)**.
    

---

And there you have it! Because $K$ is positive, the term $-K$ in our total energy equation strictly lowers the energy of the state, mathematically proving the "Fermi hole" effect we described physically in part 6.

You have successfully navigated a complete, multi-part, university-level theoretical quantum mechanics problem from start to finish! How are you feeling about all of this? Would you like me to summarize the main "story" of this entire problem so you have a clean overview for your notes?