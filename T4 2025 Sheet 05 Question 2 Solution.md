

Hello there! Welcome to the wonderful world of Statistical Physics. I'm delighted to be your guide. Don't worry if this looks intimidating at first glance—thermodynamics is essentially just accounting for energy and chaos (entropy), and once you learn the "rules of the game," it becomes quite intuitive.

Let's start by looking at the problem you've uploaded. It is written in German, so our first step is to translate it to make sure we are on the same page.

### **The Problem Statement**

**Original Text:**

> "Gegeben sei ein thermodynamisches System, für welches die Temperatur $T$, der Druck $P$ und die Teilchenzahl $N$ unabhängig variierbare Parameter sind. Geben Sie das thermodynamische Potential an, welches jene natürlichen Variablen besitzt und zeigen Sie, dass dieses im thermodynamischen Gleichgewicht minimal wird. Überlegen Sie sich dafür zunächst eine Realisierung, in welcher die durch $T$, $P$ und $N$ kontrollierten Zustandsänderungen dargestellt werden können."

**Translation:**

> "Consider a thermodynamic system for which the Temperature $T$, Pressure $P$, and Particle Number $N$ are independently variable parameters. State the thermodynamic potential that possesses these natural variables and show that it becomes minimal in thermodynamic equilibrium. For this purpose, first consider a realization (physical setup) in which the state changes controlled by $T$, $P$, and $N$ can be represented."

---

### **Part 1: Identifying the Thermodynamic Potential**

In thermodynamics, "Potentials" are just energy functions that tell us how a system behaves under different constraints. The key to identifying the right one is looking at the **"Natural Variables"**—the variables we control or that are fixed by the environment.

The problem states our variables are:

1.  **Temperature ($T$)**
    
2.  **Pressure ($P$)**
    
3.  **Particle Number ($N$)**
    

Let's derive the correct potential starting from the "mother" of all potentials: **Internal Energy ($U$)**.

The fundamental thermodynamic relation for Internal Energy (combining the First and Second Laws) is:

$$dU = TdS - PdV + \mu dN$$

Here, the natural variables are Entropy ($S$), Volume ($V$), and Particle Number ($N$).

We need to swap $S$ for $T$ and $V$ for $P$. We do this using a mathematical trick called the **Legendre Transform**.

1.  Swap $S \to T$: We subtract $TS$ from $U$. This gives us the Helmholtz Free Energy ($F$).
    
    $$F = U - TS$$
    
    $$dF = dU - d(TS) = (TdS - PdV + \mu dN) - (TdS + SdT) = -SdT - PdV + \mu dN$$
    
    (Now variables are $T, V, N$)
    
2.  Swap $V \to P$: We add $PV$ to the equation. This gives us our target.
    
    Let's define a new potential, let's call it $G$:
    
    $$G = F + PV = U - TS + PV$$
    
    Let's check the differential change $dG$:
    
    $$dG = d(U - TS + PV)$$
    
    $$dG = dU - (TdS + SdT) + (PdV + VdP)$$
    
    Substitute $dU = TdS - PdV + \mu dN$:
    
    $$dG = (TdS - PdV + \mu dN) - TdS - SdT + PdV + VdP$$
    
    Cancel out the terms:
    
    $$dG = -SdT + VdP + \mu dN$$
    

The Winner:

The potential depends on changes in $T$, $P$, and $N$. This is the Gibbs Free Energy (or Gibbs Potential), denoted by $G(T, P, N)$.

---

### **Part 2: The Physical Realization**

The problem asks for a "realization" or a physical setup where this applies.

To test if $G$ is minimized, we need a setup where **$T$ and $P$ are fixed by the surroundings**, and $N$ is a parameter of our system (usually fixed for a closed system, but defined as a variable characteristic).

**Imagine this setup:**

1.  **The System:** A gas inside a cylinder with a movable piston.
    
2.  **Temperature Control:** The cylinder is submerged in a gigantic swimming pool (a **Heat Reservoir**) maintained at a constant temperature $T_{bath}$. This ensures that no matter what happens in the cylinder, its final temperature will be $T$.
    
3.  **Pressure Control:** The piston is not locked. Instead, it is weighted down by a constant mass or exposed to the atmosphere. This acts as a **Pressure Reservoir**, ensuring the system is always under constant external pressure $P_{ext}$.
    

In this setup, our system can exchange **Heat** (with the bath) and **Volume work** (with the weight on the piston), but the Universe (System + Bath + Weight) is isolated.

---

### **Part 3: Proving $G$ is Minimal at Equilibrium**

Now for the physics proof! We need to show that under these conditions (constant $T, P, N$), the system will evolve until $G$ hits a minimum.

Step 1: The Second Law of Thermodynamics

The golden rule of the universe is that for any spontaneous process in an isolated system (the "Universe"), the total entropy must increase (or stay constant at equilibrium).

$$dS_{total} \ge 0$$

Our "Universe" consists of the System and the Surroundings (Reservoir).

$$dS_{total} = dS_{sys} + dS_{surr} \ge 0$$

Step 2: Analyzing the Surroundings

The surroundings are a massive reservoir. When the system exchanges a small amount of heat $dQ$ with the surroundings, the entropy change of the surroundings is defined simply as:

$$dS_{surr} = \frac{dQ_{surr}}{T}$$

Since energy is conserved, any heat entering the system ($dQ_{sys}$) must come from the surroundings ($dQ_{surr} = -dQ_{sys}$).

$$dS_{surr} = \frac{-dQ_{sys}}{T}$$

Step 3: Analyzing the Heat Exchange (First Law)

For our system, the First Law of Thermodynamics says:

$$dU_{sys} = dQ_{sys} - dW_{sys}$$

Where $dW_{sys}$ is the work done by the system. Since pressure is constant ($P$), the work is simply $P dV_{sys}$.

$$dQ_{sys} = dU_{sys} + P dV_{sys}$$

Step 4: Putting it all together

Now, substitute the expression for $dQ_{sys}$ (Step 3) into the expression for $dS_{surr}$ (Step 2), and then put that into the Second Law inequality (Step 1).

$$dS_{sys} + \left( \frac{-(dU_{sys} + P dV_{sys})}{T} \right) \ge 0$$

Let's clean this up by multiplying the whole inequality by $T$ (since $T > 0$, the sign doesn't flip):

$$T dS_{sys} - dU_{sys} - P dV_{sys} \ge 0$$

Rearrange to group terms on one side:

$$dU_{sys} + P dV_{sys} - T dS_{sys} \le 0$$

Step 5: Identifying the Gibbs Free Energy

Look at the definition of Gibbs Free Energy: $G = U + PV - TS$.

If we take the differential of $G$ assuming $T$, $P$, and $N$ are constant (because they are properties of the reservoir/setup):

$$dG_{T,P,N} = dU + P dV - T dS$$

Compare this to our inequality above:

$$dG \le 0$$

Conclusion:

This inequality tells us that for any spontaneous change occurring at constant temperature and pressure, the change in Gibbs Free Energy ($dG$) must be negative. The system will keep changing, lowering its $G$, until it can't go any lower.

Therefore, **at equilibrium, $G$ is at a minimum.**

---

### **Summary for your Professor**

If you were to write this out for your exam, you would say:

1.  **The Potential:** The Gibbs Free Energy $G(T, P, N) = U - TS + PV$.
    
2.  **The Realization:** A system in contact with a heat bath (fixing $T$) and a pressure reservoir (fixing $P$).
    
3.  **The Proof:** By applying the Second Law ($dS_{total} \ge 0$) to the combined system + reservoir, we derive that $dG \le 0$ for the system. This implies that the stable equilibrium state corresponds to the minimum of $G$.
    

**Would you like me to clarify the Legendre Transform math, or move on to the next problem?**