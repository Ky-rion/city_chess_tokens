

![[Pasted image 20260206194748.png]]

Hello! Welcome to Particle Physics 101. I am delighted to be your professor today. Don't worry if you haven't seen this before—angular momentum in quantum mechanics can be a bit counter-intuitive at first, but it follows very strict rules.

Let's break down part (a) step-by-step.

### The Big Picture: Conservation Laws

In particle physics, whenever a particle decays (breaks apart), certain properties must be conserved. This means the total amount of that property _before_ the decay must equal the total amount _after_ the decay.

For this problem, we are looking at **Angular Momentum Conservation**.

**The Equation:**

$$\text{Total Angular Momentum (Parent)} = \text{Total Angular Momentum (Daughters)}$$

### Step 1: Identify the "Spin" of the Players

First, we need to know the intrinsic "spin" ($S$) of every particle involved. Think of spin as the particle's permanent identity card; it doesn't change.

1. **The Parent ($\Delta^+$):**
    
    The problem statement tells us the Delta-plus ($\Delta^+$) has a spin of **$3/2$**.
    
    - _Prof's Note:_ We usually drop the $\hbar$ when talking casually, but physically the unit is $\hbar$.
        
2. **The Daughter 1 (Neutron, $n$):**
    
    The solution image correctly identifies the neutron spin: $S_n = 1/2$.
    
    - _Why?_ Neutrons are baryons (made of 3 quarks), and ground-state baryons like protons and neutrons always have spin $1/2$.
        
3. **The Daughter 2 (Pion, $\pi^+$):**
    
    The solution identifies the pion spin: $S_{\pi} = 0$.
    
    - _Why?_ Pions are mesons (made of a quark and antiquark). They are "scalar" particles, meaning they have no intrinsic spin.
        

### Step 2: Combine the Daughter Spins

Now, let's look at the "After" state (the right side of the decay $\Delta^+ \rightarrow n + \pi^+$). We have a neutron and a pion.

We first add their intrinsic spins together to get the total channel spin ($S_{daughters}$). In quantum mechanics, adding spins is simple if one of them is zero.

$$S_{daughters} = S_n + S_{\pi} = 1/2 + 0 = 1/2$$

So, the combined intrinsic spin of the resulting particles is **$1/2$**.

### Step 3: The Missing Ingredient (Orbital Angular Momentum)

Here is the puzzle:

- The **Parent** had a total spin of **$3/2$**.
    
- The **Daughters** have a combined intrinsic spin of only **$1/2$**.
    

The numbers don't match! $3/2 \neq 1/2$. Where did the extra angular momentum go?

It went into the **orbital motion** of the particles flying away from each other. We call this **Orbital Angular Momentum**, denoted by the letter **$l$**.

Our conservation equation now looks like this:

$$\vec{J}_{\Delta} = \vec{S}_{daughters} + \vec{l}$$

We know the magnitudes:

$$3/2 = 1/2 \oplus l$$

_(Note: I use $\oplus$ because in quantum mechanics, we are adding vectors, not just regular numbers)._

### Step 4: Solving the Vector Addition (The Solution Image Explained)

In quantum mechanics, when you add two angular momentum vectors (let's call them $A$ and $B$) to get a total $C$, the possible values for $C$ are bound by a "Triangle Inequality."

The rule is:

$$|A - B| \le C \le A + B$$

The solution image applies this rule specifically to our variables:

- $A = l$ (the unknown orbital momentum)
    
- $B = S_n = 1/2$ (the combined daughter spin)
    
- $C = 3/2$ (the total conserved momentum from the parent)
    

So, the inequality in the solution image is:

$$|l - 1/2| \le 3/2 \le l + 1/2$$

This mathematical sandwich tells us that the parent's spin ($3/2$) must be achievable by combining $l$ and $1/2$.

**Let's test integer values for $l$ (since orbital angular momentum $l$ must always be an integer: 0, 1, 2...):**

- **Try $l=0$:**
    
    Range is $|0 - 1/2|$ to $0 + 1/2$. The result is just $1/2$.
    
    _Does this match the parent's $3/2$?_ No.
    
- **Try $l=1$:**
    
    Range is $|1 - 1/2|$ to $1 + 1/2$.
    
    Range is $[1/2, 3/2]$.
    
    _Does this range include the parent's $3/2$?_ **Yes!**
    
    (This corresponds to the vector spins being aligned).
    
- **Try $l=2$:**
    
    Range is $|2 - 1/2|$ to $2 + 1/2$.
    
    Range is $[3/2, 5/2]$.
    
    _Does this range include the parent's $3/2$?_ **Yes!**
    
    (This corresponds to the vector spins being anti-aligned).
    
- **Try $l=3$:**
    
    Range starts at $|3 - 1/2| = 5/2$.
    
    _Does this include $3/2$?_ No, it's too high.
    

### Summary of the Solution Image

When the other professor wrote:

$$l = \frac{3}{2}\hbar - S_n = 1\hbar \quad \text{or} \quad l = \frac{3}{2}\hbar + S_n = 2\hbar$$

They were solving for the two specific cases that satisfy the vector addition rules:

1. **$l=1$**: The orbital momentum (1) and neutron spin (1/2) point in the **same** direction ($1 + 1/2 = 3/2$).
    
2. **$l=2$**: The orbital momentum (2) and neutron spin (1/2) point in **opposite** directions ($2 - 1/2 = 3/2$).
    

**Final Answer:**

The allowed orbital angular momenta are **$l = 1$ and $l = 2$**.

Usually, in physics, the lowest allowed $l$ dominates the decay, so $l=1$ (called p-wave decay) is the most likely scenario, but $l=2$ (d-wave) is theoretically allowed by conservation laws.

---

**Would you like to move on to part (b) to see how "Parity" eliminates one of these two options?**