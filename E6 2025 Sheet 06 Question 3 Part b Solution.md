

![[Pasted image 20260125184542.png]]

Welcome back to the "office"! Now that we understand the _rules_ of the game (Selection Rules from part a), let's look at the _score_ (Intensity).

Part b) is a classic derivation that connects spectroscopy to thermodynamics. It asks us to prove why one type of scattering is much brighter than the other.

### 1. Translation and The Setup

First, let's translate the German text in **Image 1** to ensure we catch every detail.

**The Question:**

> _b) For the intensity of the Stokes and Anti-Stokes lines, respectively, the following proportionalities can be established:_
> 
> $$I_{Stokes} \propto (\nu_0 - \nu_M)^4 (N_0(\nu) + 1)$$
> 
> $$I_{Antistokes} \propto (\nu_0 + \nu_M)^4 N_0(\nu)$$
> 
> _Here, $\nu_0$ is the excitation frequency (laser), $\nu_M$ is the Raman shift (molecular vibration), and $N_0$ denotes the occupation probability of the states. Derive an expression for the ratio of the intensity of Stokes and Anti-Stokes lines from this information._

**The Solution (Image 2):**

The solution image performs the algebraic derivation, arriving at a final exponential relationship.

---

### 2. The Physics Behind the Formulas

Before we do the math, we must understand _why_ the formulas look like this. This is the "hidden" physics the problem assumes you know.

**1. The $\nu^4$ term:**

You might notice both equations start with a frequency term to the fourth power $(\nu)^4$. This comes from classical scattering theory (similar to Rayleigh scattering, which makes the sky blue). Scattering efficiency increases drastically as the frequency of light increases.

**2. The $(N_0 + 1)$ vs. $N_0$ term (The Quantum Part):**

This is the most critical part. We are dealing with **phonons** (quantized vibrations).

-   **Stokes process:** The photon hits the molecule and _creates_ a vibration. It gives up energy. In quantum mechanics, the probability of _creating_ a boson (phonon) is proportional to $(N_0 + 1)$.
    
-   **Anti-Stokes process:** The photon hits a molecule that is _already vibrating_ and steals its energy. It can only do this if the vibration is already there! Therefore, the probability depends directly on the number of existing phonons, $N_0$.
    

---

### 3. The Step-by-Step Derivation

Let's walk through the red solution text (Image 2) line by line.

**Step 1: Set up the Ratio**

We want to compare the intensity of Stokes ($I_S$) to Anti-Stokes ($I_{AS}$). We simply divide equation (2) by equation (3):

$$\frac{I_S}{I_{AS}} = \frac{(\nu_0 - \nu_M)^4 (N_0(\nu) + 1)}{(\nu_0 + \nu_M)^4 N_0(\nu)}$$

**Step 2: Simplify the Population Term**

We can separate the frequency parts from the population parts. Let's look at just the fraction involving $N_0$:

$$\frac{N_0(\nu) + 1}{N_0(\nu)} = \frac{N_0(\nu)}{N_0(\nu)} + \frac{1}{N_0(\nu)} = 1 + \frac{1}{N_0(\nu)}$$

So the equation becomes:

$$\frac{I_S}{I_{AS}} = \frac{(\nu_0 - \nu_M)^4}{(\nu_0 + \nu_M)^4} \cdot \left(1 + \frac{1}{N_0(\nu)}\right)$$

**Step 3: The "Secret" Substitution (Bose-Einstein)**

This is the step where students often get stuck. The problem mentions $N_0$ is the "occupation probability." Since molecular vibrations (phonons) are **Bosons**, they follow **Bose-Einstein Statistics**:

$$N_0(\nu) = \frac{1}{e^{\frac{h\nu_M}{k_B T}} - 1}$$

_(Where $h$ is Planck's constant, $k_B$ is Boltzmann's constant, and $T$ is temperature)._

To use this in our equation, we need to find $\frac{1}{N_0}$. Let's invert the Bose-Einstein formula:

$$\frac{1}{N_0(\nu)} = e^{\frac{h\nu_M}{k_B T}} - 1$$

**Step 4: Final Assembly**

Now, substitute this back into our ratio from Step 2:

$$\frac{I_S}{I_{AS}} = \frac{(\nu_0 - \nu_M)^4}{(\nu_0 + \nu_M)^4} \cdot \left( 1 + \left[ e^{\frac{h\nu_M}{k_B T}} - 1 \right] \right)$$

The $+1$ and $-1$ cancel each other out!

$$\frac{I_S}{I_{AS}} = \frac{(\nu_0 - \nu_M)^4}{(\nu_0 + \nu_M)^4} \cdot e^{\frac{h\nu_M}{k_B T}}$$

(This matches the final line in your solution image).

---

### 4. What does this result tell us?

This final equation is incredibly powerful for experimentalists.

1.  **Stokes is King:** The exponential term $e^{h\nu/kT}$ is usually a large number. This proves mathematically that **Stokes lines are much stronger (more intense) than Anti-Stokes lines.**
    
    -   _Why?_ At room temperature, most molecules are "chilling" in the ground state ($N_0$ is small). It is easy to kick them up (Stokes), but hard to find one already kicked up to steal energy from (Anti-Stokes).
        
2.  **Thermometer:** Notice the $T$ in the exponent? By measuring the ratio of the two peak heights in a lab, you can actually calculate the precise temperature of the sample without touching it!
    

**Next Step:**

That explains the math behind the intensity ratio! Do you want to try plugging in some real numbers (like room temperature) to see how huge that ratio actually is, or do you have another part of the problem set?