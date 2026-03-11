

Welcome to theoretical physics! It is wonderful to have a curious student here. Do not worry at all that this is your first time seeing this material. Quantum mechanics can look like an entirely foreign language at first, but once you learn the "alphabet" of quantum numbers, it becomes incredibly elegant and logical.

Let's break this down step-by-step.

First, let's translate the German text into English so we are exactly on the same page:

> **4 Hydrogen Atom (17 points)**
> 
> 1. How many (orthogonal) bound states with energy $E_n \le -1/8$ are there in the hydrogen atom? List the quantum numbers m, l, n of all states with $E_n \le -1/8$. [2 pts.]
>     

To solve this, we need to understand two key concepts: how energy works in a hydrogen atom, and what these "quantum numbers" are.

---

### Part 1: Decoding the Energy $E_n$

In quantum mechanics, an electron in a hydrogen atom cannot just have _any_ energy. It is "quantized," meaning it can only exist in specific, discrete energy levels—like standing on the steps of a ladder rather than a ramp.

The energy of these states is given by a surprisingly simple formula. In theoretical physics, we often use **Atomic Units (Hartree)** to make our math cleaner (we essentially set fundamental constants like the mass of the electron to 1). In these units, the energy of a hydrogen atom at level $n$ is:

$$E_n = -\frac{1}{2n^2}$$

_Note: The energy is negative because the electron is "bound" to the proton. An energy of $0$ would mean the electron has completely escaped the atom. A more negative number means the electron is bound more tightly!_

The problem asks for states where the energy $E_n$ is **less than or equal to $-1/8$**. Let's plug in the first few levels ($n = 1, 2, 3, \dots$) to see which ones fit this rule:

- **For $n = 1$:** $E_1 = -\frac{1}{2(1)^2} = -\frac{1}{2} = -0.5$
    
    _Is $-0.5 \le -0.125$?_ **Yes.** * **For $n = 2$:** $E_2 = -\frac{1}{2(2)^2} = -\frac{1}{8} = -0.125$
    
    _Is $-0.125 \le -0.125$?_ **Yes.**
    
- **For $n = 3$:** $E_3 = -\frac{1}{2(3)^2} = -\frac{1}{18} \approx -0.055$
    
    _Is $-0.055 \le -0.125$?_ **No.** (Remember, $-0.055$ is closer to zero, so it is mathematically _greater_ than $-0.125$).
    

**Conclusion for Part 1:** The only allowed principal energy levels for this problem are **$n = 1$** and **$n = 2$**.

---

### Part 2: The Quantum Numbers ($n, l, m$)

Now we need to find all the specific "states" (which you can think of as unique 3D shapes the electron takes, called orbitals) that exist within $n=1$ and $n=2$. We describe these states using three specific quantum numbers:

1. **$n$ (Principal Quantum Number):** Think of this as the "shell" or the size of the orbital. As we found above, $n$ can be $1, 2, 3, \dots$
    
2. **$l$ (Azimuthal/Orbital Quantum Number):** This dictates the _shape_ of the orbital (spherical, dumbbell-shaped, etc.).
    
    - **Rule:** $l$ can be any integer from $0$ up to $n - 1$.
        
3. **$m$ (Magnetic Quantum Number):** This dictates the _orientation_ of that shape in 3D space.
    
    - **Rule:** $m$ can be any integer from $-l$ to $+l$, including $0$.
        

Let's map them all out for our allowed energy levels!

#### States for $n = 1$

- Since $n=1$, $l$ must be $0$ (because $1-1=0$).
    
- If $l=0$, $m$ must also be $0$.
    
- **Result:** This gives us exactly **1 state**: $(n=1, l=0, m=0)$. _In chemistry, this is known as the 1s orbital!_
    

#### States for $n = 2$

- Since $n=2$, $l$ can be $0$ OR $1$. We have to look at both!
    
    - **If $l = 0$:** $m$ must be $0$.
        
        - **Result:** This gives us **1 state**: $(n=2, l=0, m=0)$. _(The 2s orbital)._
            
    - **If $l = 1$:** $m$ can be $-1, 0,$ or $+1$.
        
        - **Result:** This gives us **3 states**:
            
            $(n=2, l=1, m=-1)$
            
            $(n=2, l=1, m=0)$
            
            $(n=2, l=1, m=1)$
            
            _(These are the three 2p orbitals)._
            

---

### Final Answer

If we count them all up, we have $1 + 1 + 3 = 5$ total states.

Here is the final, beautifully organized answer you would write on your exam paper:

**Total number of states:** 5

**List of quantum numbers $(n, l, m)$:**

|**n (Principal)**|**l (Orbital)**|**m (Magnetic)**|**Common Name**|
|---|---|---|---|
|1|0|0|1s|
|2|0|0|2s|
|2|1|-1|2p|
|2|1|0|2p|
|2|1|1|2p|

> **Professor's Bonus Note:** The problem strictly asked for $m, l, n$, yielding 5 states. However, later in the course, we will learn about a fourth quantum number: _Spin_ ($m_s$). Because an electron can spin "up" or "down", each of these 5 spatial states can actually hold 2 electrons. If the problem had asked for the total number of _electron_ states, the answer would be 10! But for now, 5 is exactly what the grader is looking for.

Would you like me to explain what these different states actually physically look like in 3D space, or shall we move on to another quantum mechanics problem?