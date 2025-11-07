

This is a fantastic question! It's the logical reverse of the problem we just solved.

In part (1.a), we proved:

Ideal Gas Law $\implies$ Energy depends only on T

Now, in part (1.b), we're asked to prove the reverse:

Energy depends only on T $\implies$ What is the (most general) equation of state?

Let's use the exact same toolkit we developed in the last problem.

### 🎯 The Goal

First, let's translate the problem:

> Given:
> 
> The assumption that the internal energy $E$ depends only on temperature $T$. (In other words, $E = E(T)$).
> 
> To Find:
> 
> The most general equation of state, $P(V, T)$, that is consistent with this assumption.

### Derivation: Finding the General Form

We will start from the exact same "test equation" (the thermodynamic equation of state) that we derived in the last problem. This equation is _always_ true and connects $E$, $P$, $T$, and $V$.

$$\left(\frac{\partial E}{\partial V}\right)_T = T \left(\frac{\partial P}{\partial T}\right)_V - P$$

---

#### Step 1: Apply the New Assumption

Our new assumption is that **$E$ depends only on $T$**.

Let's look at the left-hand side (LHS) of our test equation: $\left(\frac{\partial E}{\partial V}\right)_T$.

-   This mathematical expression asks: "How does the internal energy $E$ change when the volume $V$ changes, _while the temperature $T$ is held constant_?"
    
-   According to our new assumption, $E$ _only_ depends on $T$. If $T$ is held constant, then $E$ _cannot change_ at all, no matter what happens to $V$.
    
-   Therefore, the assumption $E = E(T)$ mathematically _forces_ the following to be true:
    
    $$ \left(\frac{\partial E}{\partial V}\right)_T = 0$$
    

---

#### Step 2: Solve the Resulting Equation

Now we can substitute this `0` into our "test equation":

$$0 = T \left(\frac{\partial P}{\partial T}\right)_V - P$$

This is the central relationship. Any gas whose energy depends only on $T$ _must_ obey this equation. Our goal is to solve this equation for $P$.

Let's rearrange it to isolate the derivative:

$$T \left(\frac{\partial P}{\partial T}\right)_V = P$$

$$\left(\frac{\partial P}{\partial T}\right)_V = \frac{P}{T}$$

---

#### Step 3: Solve the Partial Differential Equation

This is a **partial differential equation** (PDE). It looks a bit scary, but we can solve it using a method called "separation of variables."

We are looking at the change in $P$ with respect to $T$, while holding $V$ constant. Since $V$ is constant, we can treat this like a simpler ordinary differential equation.

Let's rearrange the equation so all the $P$ terms are on one side and all the $T$ terms are on the other:

$$\frac{1}{P} \left(\frac{\partial P}{\partial T}\right)_V = \frac{1}{T}$$

Since $V$ is constant, we can write $\frac{\partial P}{P} = \frac{\partial T}{T}$. Let's integrate both sides:

$$\int \frac{1}{P} dP = \int \frac{1}{T} dT$$

This integration gives us:

$$\ln(P) = \ln(T) + C$$

where $C$ is the "constant of integration."

Here is the most important part:

Because our original derivative $\left(\frac{\partial}{\partial T}\right)_V$ was taken while holding $V$ constant, our "constant" of integration $C$ isn't necessarily a simple number. It can be any function of the variable we held constant.

Therefore, the constant of integration $C$ is actually an arbitrary function of $V$. Let's write $C = f(V)$ to make this clear.

$$\ln(P) = \ln(T) + f(V)$$

(where $f(V)$ is _some unknown function_ that depends only on $V$).

Now, let's solve for $P$ by exponentiating both sides:

$$e^{\ln(P)} = e^{(\ln(T) + f(V))}$$

$$P = e^{\ln(T)} \cdot e^{f(V)}$$

$$P = T \cdot e^{f(V)}$$

Since $f(V)$ is an arbitrary function of $V$, $e^{f(V)}$ is also just _some other_ arbitrary function of $V$. Let's call this new function $g(V)$:

$$g(V) = e^{f(V)}$$

Substituting this in gives our final, most general answer:

$$P(V, T) = T \cdot g(V)$$

---

### 💡 The "Big Picture" Conclusion

The most general equation of state consistent with the assumption that $E = E(T)$ is:

$P(V, T) = T \cdot g(V)$

This means that for _any_ gas whose internal energy depends only on its temperature, its equation of state **must** be separable into a product of $T$ and some function $g(V)$ that depends _only_ on volume.

**Let's check this against the Ideal Gas Law (part 1.a):**

-   The Ideal Gas Law is $PV = N k_B T$.
    
-   Let's solve for $P$: $P = \frac{N k_B T}{V}$
    
-   We can rewrite this as: $P = T \cdot \left( \frac{N k_B}{V} \right)$
    
-   This perfectly matches our general form $P = T \cdot g(V)$, where the specific function for an ideal gas is $g(V) = \frac{N k_B}{V}$.
    

So, the ideal gas is just **one specific example** of this more general family of equations!

Does this "reverse" derivation make sense, and do you see how the "constant" of integration $C$ was the key to finding the "most general" form?