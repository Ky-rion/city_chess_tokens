

Hello there! An excellent question. This is the absolute foundation of all nuclear decay, and it's a beautiful piece of physics and calculus working together. Let's break it down step-by-step.

Our goal is to answer part (a):

1.  Find the **differential equation** for radioactive decay.
    
2.  **Derive** the radioactive decay law from it.
    

---

### 🧪 Part 1: The Differential Equation

First, let's think about the process. Radioactive decay is a **stochastic** process, which is a fancy word meaning it's **random**. We can never predict exactly when _one specific_ carbon-14 nucleus will decay.

However, if we have a huge number of them (like in our 1.2 g wood splinter), we can talk about the _average_ behavior.

Let's establish our key variable:

-   $N(t)$ = the number of radioactive nuclei (in our case, $^{14}$C atoms) that are _still present_ at a given time $t$.
    

Now, let's think about the **rate of decay**. This is the number of atoms that decay per unit of time (e.g., decays per hour). In the problem, this is given as 845 decays per hour. We call this the **Activity**, $A(t)$.

Here is the most important concept:

> The rate of decay (the Activity) is directly **proportional** to the number of radioactive nuclei currently present.

Think of it like a big container of popcorn. The more kernels you have, the more "pops" (decays) you'll hear per second. As the number of un-popped kernels ($N$) decreases, the rate of popping ($A$) also goes down.

We can write this relationship mathematically:

$A(t) \propto N(t)$

To turn this "proportional to" $(\propto)$ sign into an "equals" $(=)$ sign, we introduce a proportionality constant. In physics, we use the Greek letter **lambda ($\lambda$)**, and we call it the **decay constant**.

$A(t) = \lambda N(t)$

This $\lambda$ represents the _probability_ that any single nucleus will decay in a given unit of time.

---

So, we have one expression for Activity. But what _is_ Activity, mathematically? It's the _rate at which $N(t)$ is changing_. In calculus, "rate of change" means a **derivative**.

-   The rate of change of $N(t)$ is $\frac{dN}{dt}$.
    
-   Since the number of nuclei $N(t)$ is **decreasing** over time, its rate of change must be **negative**.
    
-   The Activity, $A(t)$, is defined as a _positive_ number (e.g., 845 decays/hour).
    

Therefore, the Activity $A(t)$ is the negative of the rate of change $\frac{dN}{dt}$:

$A(t) = -\frac{dN}{dt}$

Now we have two different expressions for the same thing, $A(t)$. Let's set them equal to each other:

$\lambda N(t) = -\frac{dN}{dt}$

Rearranging this gives us our answer. This is the **differential equation for radioactive decay**:

> $\frac{dN}{dt} = -\lambda N(t)$

This equation simply states that the rate of change of our nuclei is proportional to the number of nuclei we have, and it's negative because that number is decreasing.

---

### 🧬 Part 2: Deriving the Radioactive Decay Law

Now, we must "solve" this differential equation. Solving it means finding a function $N(t)$ that tells us the number of nuclei at _any_ time $t$, not just the _rate of change_.

We'll use a standard calculus technique called **separation of variables**. The goal is to get all the $N$ terms on one side of the equation and all the $t$ terms on the other.

1. Separate the variables:

Start with our equation:

$\frac{dN}{dt} = -\lambda N$

Divide both sides by $N$ and multiply both sides by $dt$:

$\frac{1}{N} dN = -\lambda dt$

2. Integrate both sides:

Now we take the integral of both sides. We'll integrate from our starting time, $t=0$, to some later time, $t$.

At $t=0$, we have our initial number of nuclei, which we'll call $N_0$.

At time $t$, we have the number $N(t)$.

$\int_{N_0}^{N(t)} \frac{1}{N} dN = \int_{0}^{t} -\lambda dt$

**3. Solve the integrals:**

-   Left Side: The integral of $\frac{1}{N}$ with respect to $N$ is the natural logarithm, $\ln(N)$. We evaluate this from $N_0$ to $N(t)$:
    
    $[\ln(N)]_{N_0}^{N(t)} = \ln(N(t)) - \ln(N_0)$
    
-   Right Side: $\lambda$ is a constant, so we pull it out. The integral of $dt$ is just $t$. We evaluate this from $0$ to $t$:
    
    $[-\lambda t]_{0}^{t} = (-\lambda t) - (-\lambda \cdot 0) = -\lambda t$
    

4. Set the results equal:

$\ln(N(t)) - \ln(N_0) = -\lambda t$

5. Solve for $N(t)$:

First, let's use the logarithm rule $\ln(a) - \ln(b) = \ln(\frac{a}{b})$:

$\ln(\frac{N(t)}{N_0}) = -\lambda t$

Now, to get $N(t)$ out of the logarithm, we do the inverse operation: we take $e$ (the base of the natural log) to the power of both sides:

$e^{\ln(\frac{N(t)}{N_0})} = e^{-\lambda t}$

The $e$ and the $\ln$ cancel each other out on the left side:

$\frac{N(t)}{N_0} = e^{-\lambda t}$

Finally, multiply both sides by $N_0$ to get our answer. This is the **Radioactive Decay Law**:

> $N(t) = N_0 e^{-\lambda t}$

This beautiful, fundamental equation tells us that the number of radioactive atoms we have left, $N(t)$, decreases **exponentially** from the starting amount $N_0$ over time.

This law is what we'll need to use for the rest of the problem, first by relating $\lambda$ to the half-life and then by finding $N_0$ and $N(t)$ to solve for the age $t$.

---

I hope that detailed explanation was clear! The next logical step is to use the information from the problem (like the half-life) to build on this.

Would you like me to show you how to relate the decay constant $\lambda$ to the half-life $t_{1/2}$?