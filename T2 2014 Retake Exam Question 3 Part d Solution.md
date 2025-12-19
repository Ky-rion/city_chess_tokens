

This is where things get interesting! Now that we have the formula for energy, we get to explore the "ladder" of energy levels that the particle can inhabit.

Part **(3d)** asks us to list the **four lowest eigenenergies** and determine their **degree of degeneracy**.

### 1. The Strategy

First, let's bring back the energy formula we derived in Part (3c):

$$E_{m,n} = \frac{\hbar^2 \pi^2}{2Ma^2} (m^2 + n^2)$$

To make the math cleaner and easier to read, let's group all those constants into a single unit called $E_0$ (or sometimes just "units of energy").

$$E_0 = \frac{\hbar^2 \pi^2}{2Ma^2}$$

So, our formula is simply:

$$E_{m,n} = E_0 (m^2 + n^2)$$

Our job is to plug in integer values for the quantum numbers $m$ and $n$ (remember, they start at 1, not 0!) to find the smallest possible values for $(m^2 + n^2)$.

---

### 2. Hunting for the Lowest Energies

Let's test combinations of $m$ and $n$.

**Attempt 1: The absolute minimum**

-   Smallest possible integers: $m=1, n=1$.
    
-   Calculation: $1^2 + 1^2 = 2$.
    
-   **Energy:** $2 E_0$.
    
-   **Is there any other way to get this number?** No. $m$ and $n$ must be at least 1.
    
-   **Degeneracy:** 1 (Non-degenerate).
    

**Attempt 2: Increasing the integers slightly**

-   Let's try increasing one number: $m=1, n=2$.
    
-   Calculation: $1^2 + 2^2 = 1 + 4 = 5$.
    
-   **Energy:** $5 E_0$.
    
-   **Is there another way?** Yes! We can swap them: $m=2, n=1$.
    
-   Calculation: $2^2 + 1^2 = 4 + 1 = 5$.
    
-   **Degeneracy:** 2.
    
    -   _Physics Note:_ The state $(1,2)$ looks like one hump in x and two in y. The state $(2,1)$ looks like two humps in x and one in y. They look different (one is rotated 90 degrees), but they have the exact same energy. This is called **degeneracy**.
        

**Attempt 3: Increasing further**

-   What if we increase both to 2? $m=2, n=2$.
    
-   Calculation: $2^2 + 2^2 = 4 + 4 = 8$.
    
-   **Energy:** $8 E_0$.
    
-   **Is there another way?** No.
    
-   **Degeneracy:** 1.
    

**Attempt 4: Finding the next level**

-   We need to beat 8. Let's try $m=1, n=3$.
    
-   Calculation: $1^2 + 3^2 = 1 + 9 = 10$.
    
-   **Energy:** $10 E_0$.
    
-   **Is there another way?** Yes, swap them: $m=3, n=1$.
    
-   Calculation: $3^2 + 1^2 = 9 + 1 = 10$.
    
-   **Degeneracy:** 2.
    

_(Quick check: Are there any combinations between 8 and 10? We tried (2,2)=8. The next mix is (2,3) which is $4+9=13$. So 10 is definitely the next lowest.)_

---

### 3. The Final Answer Table

Here are the four lowest energy levels, ranked from lowest energy to highest.

**Energy Level**

**Formula (Em,n​)**

**Value (units of 2Ma2ℏ2π2​)**

**Quantum Numbers (m,n)**

**Degeneracy (Entartungsgrad)**

**1. Ground State**

$E_{1,1}$

**2**

$(1, 1)$

**1** (Non-degenerate)

**2. First Excited State**

$E_{1,2} = E_{2,1}$

**5**

$(1, 2)$ and $(2, 1)$

**2** (2-fold degenerate)

**3. Second Excited State**

$E_{2,2}$

**8**

$(2, 2)$

**1** (Non-degenerate)

**4. Third Excited State**

$E_{1,3} = E_{3,1}$

**10**

$(1, 3)$ and $(3, 1)$

**2** (2-fold degenerate)

**Summary for your solution sheet:**

1.  **Lowest Energy:** $E_1 = 2 \cdot \frac{\hbar^2 \pi^2}{2Ma^2}$, Degeneracy $g=1$.
    
2.  **Second Energy:** $E_2 = 5 \cdot \frac{\hbar^2 \pi^2}{2Ma^2}$, Degeneracy $g=2$.
    
3.  **Third Energy:** $E_3 = 8 \cdot \frac{\hbar^2 \pi^2}{2Ma^2}$, Degeneracy $g=1$.
    
4.  **Fourth Energy:** $E_4 = 10 \cdot \frac{\hbar^2 \pi^2}{2Ma^2}$, Degeneracy $g=2$.
    

You are doing great! We have classified the energy spectrum. I am ready for the next part whenever you are!