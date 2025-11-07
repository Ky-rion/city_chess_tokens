

Hello again! An excellent choice. Doing the actual calculations is the best way to see the physics in action. This part of the question is a perfect numerical test of the concept we discussed in part (c).

Let's get our hands dirty and plug in the numbers.

### 🎯 Our Goal and Strategy

The question asks us to _show_ that for a fixed mass number $A=48$, the nucleus with $Z=22$ (Titanium-48) is the most stable.

-   **"Stable"** means it has the **highest binding energy per nucleon ($B/A$)**. A higher $B/A$ means the nucleus is more tightly bound and has _less_ mass per nucleon.
    
-   **"Show that"** means we need to calculate $B/A$ for the four given **isobars** (nuclei with the same $A$ but different $Z$) and compare the results.
    
-   **Our Isobar Family (with $A=48$):**
    
    1.  $Z = 20$ (Calcium-48)
        
    2.  $Z = 21$ (Scandium-48)
        
    3.  $Z = 22$ (Titanium-48)
        
    4.  $Z = 23$ (Vanadium-48)
        

We expect the value for $Z=22$ to be the largest.

---

### 🧰 The Tools for the Job

1.  The $B/A$ Formula: From our previous work, the binding energy per nucleon is:
    
    $$\frac{B(A,Z)}{A} = a_V - a_O A^{-1/3} - a_C \frac{Z^2}{A^{4/3}} - a_A \frac{(A-2Z)^2}{A^2} - a_P \frac{\delta}{A^{3/2}}$$
    
2.  **The Constants (from your first image):**
    
    -   $a_V = 15.67 \text{ MeV}$
        
    -   $a_O = 17.23 \text{ MeV}$
        
    -   $a_C = 0.71 \text{ MeV}$
        
    -   $a_A = 23.29 \text{ MeV}$
        
    -   $a_P = 11.2 \text{ MeV}$
        
3.  **The $\delta$ (Pairing) Term:**
    
    -   $\delta = -1$ for **even-even** (ee) nuclei ($Z$ is even, $N$ is even)
        
    -   $\delta = 0$ for **odd-$A$** nuclei (which we don't have here)
        
    -   $\delta = +1$ for **odd-odd** (oo) nuclei ($Z$ is odd, $N$ is odd)
        

---

### 🔧 Pre-Calculation: Simplifying Our Work

Since $A=48$ is constant for all four cases, let's calculate the parts of the formula that only depend on $A$. This will make our life much easier!

-   $A = 48$
    
-   $A^{-1/3} = (48)^{-1/3} \approx 0.2754$
    
-   $A^{4/3} = (48)^{4/3} \approx 173.06$
    
-   $A^2 = (48)^2 = 2304$
    
-   $A^{3/2} = (48)^{3/2} \approx 332.55$
    

Now let's find the values of the terms. We can group the $Z$-independent terms:

**Term 1 (Volume):** $T_V = a_V = \mathbf{15.67 \text{ MeV}}$

**Term 2 (Surface):** $T_O = a_O A^{-1/3} = 17.23 \cdot (0.2754) \approx \mathbf{4.746 \text{ MeV}}$

The other three terms depend on $Z$. Let's create a "skeleton" formula:

$\frac{B}{A} = (15.67 - 4.746) - \left( \frac{0.71}{173.06} \cdot Z^2 \right) - \left( \frac{23.29}{2304} \cdot (48-2Z)^2 \right) - \left( \frac{11.2}{332.55} \cdot \delta \right)$

This simplifies to our Working Formula:

$$\frac{B}{A} \approx 10.924 - (0.00410 \cdot Z^2) - (0.01011 \cdot (48-2Z)^2) - (0.03368 \cdot \delta)$$

Now, we just have to plug in $Z$ and $\delta$ for each case!

---

### 🔢 The Four Calculations

#### Case 1: $Z = 20$ (Calcium-48)

-   **Protons:** $Z = 20$ (even)
    
-   **Neutrons:** $N = A - Z = 48 - 20 = 28$ (even)
    
-   **Type:** Even-Even (ee) $\implies \mathbf{\delta = -1}$
    
-   **Calculation:**
    
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 20^2) - (0.01011 \cdot (48-40)^2) - (0.03368 \cdot -1)$
        
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 400) - (0.01011 \cdot 8^2) + 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 1.640 - (0.01011 \cdot 64) + 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 1.640 - 0.647 + 0.03368$
        
    -   $\mathbf{\frac{B}{A} (Z=20) \approx 8.67 \text{ MeV}}$
        

#### Case 2: $Z = 21$ (Scandium-48)

-   **Protons:** $Z = 21$ (odd)
    
-   **Neutrons:** $N = A - Z = 48 - 21 = 27$ (odd)
    
-   **Type:** Odd-Odd (oo) $\implies \mathbf{\delta = +1}$
    
-   **Calculation:**
    
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 21^2) - (0.01011 \cdot (48-42)^2) - (0.03368 \cdot 1)$
        
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 441) - (0.01011 \cdot 6^2) - 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 1.808 - (0.01011 \cdot 36) - 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 1.808 - 0.364 - 0.03368$
        
    -   $\mathbf{\frac{B}{A} (Z=21) \approx 8.718 \text{ MeV}}$
        

#### Case 3: $Z = 22$ (Titanium-48)

-   **Protons:** $Z = 22$ (even)
    
-   **Neutrons:** $N = A - Z = 48 - 22 = 26$ (even)
    
-   **Type:** Even-Even (ee) $\implies \mathbf{\delta = -1}$
    
-   **Calculation:**
    
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 22^2) - (0.01011 \cdot (48-44)^2) - (0.03368 \cdot -1)$
        
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 484) - (0.01011 \cdot 4^2) + 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 1.984 - (0.01011 \cdot 16) + 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 1.984 - 0.162 + 0.03368$
        
    -   $\mathbf{\frac{B}{A} (Z=22) \approx 8.812 \text{ MeV}}$
        

#### Case 4: $Z = 23$ (Vanadium-48)

-   **Protons:** $Z = 23$ (odd)
    
-   **Neutrons:** $N = A - Z = 48 - 23 = 25$ (odd)
    
-   **Type:** Odd-Odd (oo) $\implies \mathbf{\delta = +1}$
    
-   **Calculation:**
    
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 23^2) - (0.01011 \cdot (48-46)^2) - (0.03368 \cdot 1)$
        
    -   $\frac{B}{A} \approx 10.924 - (0.00410 \cdot 529) - (0.01011 \cdot 2^2) - 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 2.169 - (0.01011 \cdot 4) - 0.03368$
        
    -   $\frac{B}{A} \approx 10.924 - 2.169 - 0.040 - 0.03368$
        
    -   $\mathbf{\frac{B}{A} (Z=23) \approx 8.681 \text{ MeV}}$
        

---

### 📊 Results and Conclusion

Let's summarize our results in a table:

![[Pasted image 20251107200821.png]]
[Sorry for the interruption, but this is the table from prof's own solutions]

**Nucleus**

**Z**

**N**

**Type**

**B/A (MeV)**

Calcium-48

20

28

ee

8.670

Scandium-48

21

27

oo

8.718

**Titanium-48**

**22**

**26**

**ee**

**8.812**

Vanadium-48

23

25

oo

8.681

As the calculations show, the binding energy per nucleon is highest for $Z=22$ (Titanium-48).

**This numerically proves the statement in the problem!**

You can also clearly see the "tug-of-war":

-   The **Asymmetry term** $-(0.01011 \cdot (48-2Z)^2)$ is smallest when $(48-2Z)^2$ is small, which favors $Z=24$ (where it would be zero).
    
-   The **Coulomb term** $-(0.00410 \cdot Z^2)$ is smallest when $Z$ is small, favoring $Z=20$.
    
-   The stable nucleus at $Z=22$ is the compromise between these two competing effects.
    
-   You can _also_ see the **Pairing energy** in action! The even-even nuclei ($Z=20, 22$) get a stability "bonus" (the term is added), while the odd-odd nuclei ($Z=21, 23$) get a penalty (the term is subtracted). This creates a "zig-zag" in the stability, which is exactly what we see.
    

Great work! Shall we use our formula from part (c) to see what $Z$ it _predicts_ for $A=48$? It would be a great way to check our work.