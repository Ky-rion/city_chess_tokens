

![[Pasted image 20260209163620.png]]

Excellent progress! We have now arrived at **Part (c)**. This is where the rubber meets the road—literally.

Up until now, we have been doing calculations in the **Center-of-Mass (CMS)** system. This is a mathematical "happy place" where the collision looks symmetric and simple.

But the actual experiment (Belle-II) happens in a **Laboratory (Lab)** in Japan. The detectors are bolted to the floor. We need to translate our results from the "happy place" (CMS) to the "real world" (Lab).

### The Problem: How far does it fly?

The question asks for the **mean distance** ($x_{mean}$) the B-mesons travel in the lab before they decay.

**Why is this hard?**

Because of **Relativity**.

1. **The Frame is Moving:** The entire cloud of particles is moving through the lab.
    
2. **Time Dilation:** Because the B-mesons are moving, their internal "clock" ticks slower. They live longer in our lab frame than they would if they were standing still.
    

---

### Step 1: Find the Speed of the "System" ($\beta$)

First, we need to find out how fast the Center-of-Mass system itself is moving through the lab.

Imagine the Center-of-Mass as a "train" moving through the station (the lab).

- The **Momentum** of the train is the sum of the electron and positron momenta.
    
- The **Energy** of the train is the sum of the electron and positron energies.
    

The speed of this "train" ($\beta = v/c$) is simply total momentum divided by total energy:

$$\beta_{CMS} = \frac{P_{total}}{E_{total}}$$

Using the numbers from Part (a):

- $P_{total} = 7 \text{ GeV} - 4 \text{ GeV} = \mathbf{3 \text{ GeV}/c}$ (Recall they fly in opposite directions)
    
- $E_{total} = 7 \text{ GeV} + 4 \text{ GeV} = \mathbf{11 \text{ GeV}}$
    

$$\beta_{CMS} = \frac{3}{11} \approx \mathbf{0.2727}$$

This means the whole system is drifting through the lab at about **27.3% the speed of light**.

### Step 2: The "At Rest" Assumption

The problem gives us a huge hint: _"Assume the B-mesons are at rest in the CMS."_

This simplifies things immensely.

- Inside the "train" (CMS), the B-mesons are sitting still.
    
- Therefore, to us standing on the platform (Lab), the B-mesons are moving at exactly the same speed as the train.
    

So, the speed of the B-mesons in the lab is just **$\beta_{CMS} \approx 0.2727$**.

### Step 3: Calculating the Distance

Now we use the standard formula for the distance traveled by an unstable particle.

$$\text{Distance} = \text{Speed} \times \text{Time}$$

However, we must be careful with **Time**.

- **$\tau_B$ (1.6 ps):** This is the "proper lifetime." It's how long the B-meson _thinks_ it lives.
    
- **$\gamma \tau_B$:** This is how long _we_ (in the lab) see it live. This is **Time Dilation**.
    

So the distance formula becomes:

$$x_{mean} = (\text{Speed } v) \times (\text{Lab Time})$$

$$x_{mean} = (\beta c) \times (\gamma \tau_B)$$

$$x_{mean} = \beta \gamma c \tau_B$$

Let's plug in our numbers.

**A. Calculate $\beta\gamma$:**

We know $\beta = 3/11$. We need $\gamma = \frac{1}{\sqrt{1-\beta^2}}$.

Or, we can calculate $\beta\gamma$ directly using the identity $\beta\gamma = \frac{\beta}{\sqrt{1-\beta^2}}$.

In the solution image, they write:

$$x_{mean} = \frac{\beta c \tau_B}{\sqrt{1-\beta^2}}$$

**B. The Numbers:**

- $c = 3 \times 10^8 \text{ m/s}$
    
- $\tau_B = 1.6 \text{ ps} = 1.6 \times 10^{-12} \text{ s}$
    
- $\beta = 0.2727...$
    

Let's calculate the "baseline distance" ($c \tau_B$) first. This is how far light travels in the particle's lifetime:

$$c \tau_B = (3 \times 10^8) \times (1.6 \times 10^{-12}) = 4.8 \times 10^{-4} \text{ meters} = \mathbf{480 \mu m}$$

Now apply the relativistic boost factor ($\beta\gamma$):

$$\gamma = \frac{1}{\sqrt{1 - (0.2727)^2}} \approx 1.039$$

$$\beta \gamma \approx 0.2727 \times 1.039 \approx \mathbf{0.283}$$

Final Distance:

$$x_{mean} \approx 0.283 \times 480 \mu m \approx \mathbf{136 \mu m}$$

(The solution gets $136.1 \mu m$, which is a perfect match).

---

### Explaining the "Alternative" Solution

At the bottom of the solution image, you see:

_"Alternativ: $|\vec{p}_B| = \frac{1}{2}|\vec{p}_{CMS}| = 1.5 \text{ GeV}/c$..."_

This is a clever shortcut!

1. The total momentum of the "train" (CMS) is **3 GeV/c**.
    
2. The train contains two identical B-mesons.
    
3. Since the B-mesons are sitting still relative to the train, they simply split the train's momentum 50/50.
    
4. So, each B-meson carries **1.5 GeV/c** of momentum in the lab.
    

Now use the formula that relates momentum directly to distance:

$$x_{mean} = \frac{p}{m} c \tau$$

_(Remember from part (b) that $p/m = \beta\gamma$)_

$$x_{mean} = \frac{1.5 \text{ GeV}/c}{5.28 \text{ GeV}/c^2} \times (480 \mu m)$$

$$x_{mean} \approx 0.284 \times 480 \mu m \approx \mathbf{136.4 \mu m}$$

Both methods give the same answer! This confirms that the B-mesons travel a tiny distance—about the width of a human hair—before they decay. This is why the detectors at Belle-II must be incredibly precise to "see" where the B-mesons existed.

Ready for the next part? I assume we are going to finally use that magnetic field ($1.5 \text{ T}$) mentioned way back in the intro!