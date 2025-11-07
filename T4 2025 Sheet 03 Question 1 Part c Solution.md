

This is a great problem that ties all the concepts together! It looks more complicated, but the logic is just as elegant.

Let's break down what we need to do.

### 🎯 The Goal

First, the translation:

> **Given:**
> 
> 1.  The **van der Waals equation of state**: $\left[P - a \left(\frac{N}{V}\right)^2\right] (V - Nb) = N k_B T$
>     
> 2.  The definition of **heat capacity at constant volume**: $C_V = \left(\frac{\partial E}{\partial T}\right)_V$
>     
> 
> To Prove:
> 
> $C_V$ is a function only of temperature $T$. (In other words, $C_V = C_V(T)$).

Just like in problem (1.a), our mathematical goal is to prove that $C_V$ does not depend on the other variable, $V$. We must show that the change in $C_V$ with respect to $V$ (at constant $T$) is **zero**.

Our mathematical goal is to prove:

$$\left(\frac{\partial C_V}{\partial V}\right)_T = 0$$

---

### Derivation: The Step-by-Step Proof

This derivation is beautiful. We are going to find a _general_ test for $C_V$ and then apply it to the van der Waals gas.

#### Step 1: Find a General "Test Equation" for $C_V$

We want to calculate $\left(\frac{\partial C_V}{\partial V}\right)_T$. Let's start by substituting the definition of $C_V$:

$$\left(\frac{\partial C_V}{\partial V}\right)_T = \left( \frac{\partial}{\partial V} \left[ \left(\frac{\partial E}{\partial T}\right)_V \right] \right)_T$$

This is a mixed second derivative: $\frac{\partial^2 E}{\partial V \partial T}$.

Since $E$ is a "state function" (it doesn't matter which path you take, its value only depends on the state $T, V$), the order of differentiation does not matter (this is Schwarz's theorem).

$$\frac{\partial^2 E}{\partial V \partial T} = \frac{\partial^2 E}{\partial T \partial V}$$

So, we can swap the order of our derivatives:

$$\left(\frac{\partial C_V}{\partial V}\right)_T = \left( \frac{\partial}{\partial T} \left[ \left(\frac{\partial E}{\partial V}\right)_T \right] \right)_V$$

This might look just as complicated, but we have a _fantastic_ expression for that inner term $\left(\frac{\partial E}{\partial V}\right)_T$! We derived it in part (1.a):

$$\left(\frac{\partial E}{\partial V}\right)_T = T \left(\frac{\partial P}{\partial T}\right)_V - P$$

Let's substitute this "thermodynamic equation of state" into our expression for $\left(\frac{\partial C_V}{\partial V}\right)_T$:

$$\left(\frac{\partial C_V}{\partial V}\right)_T = \left( \frac{\partial}{\partial T} \left[ T \left(\frac{\partial P}{\partial T}\right)_V - P \right] \right)_V$$

Now, let's evaluate the derivative with respect to $T$. We'll use the **product rule** on the first term:

$$\left(\frac{\partial C_V}{\partial V}\right)_T = \left[ \left(\frac{\partial T}{\partial T}\right)_V \cdot \left(\frac{\partial P}{\partial T}\right)_V + T \cdot \left( \frac{\partial}{\partial T} \left[ \left(\frac{\partial P}{\partial T}\right)_V \right] \right)_V \right] - \left(\frac{\partial P}{\partial T}\right)_V$$

Let's simplify.

-   $\left(\frac{\partial T}{\partial T}\right)_V = 1$
    
-   $\frac{\partial}{\partial T} \left[ \left(\frac{\partial P}{\partial T}\right)_V \right]$ is just the second derivative, $\left(\frac{\partial^2 P}{\partial T^2}\right)_V$
    

So our equation becomes:

$$\left(\frac{\partial C_V}{\partial V}\right)_T = \left[ 1 \cdot \left(\frac{\partial P}{\partial T}\right)_V + T \left(\frac{\partial^2 P}{\partial T^2}\right)_V \right] - \left(\frac{\partial P}{\partial T}\right)_V$$

The first and last terms cancel out!

$$\left(\frac{\partial P}{\partial T}\right)_V - \left(\frac{\partial P}{\partial T}\right)_V = 0$$

This leaves us with an incredibly powerful and general result:

$$\left(\frac{\partial C_V}{\partial V}\right)_T = T \left(\frac{\partial^2 P}{\partial T^2}\right)_V$$

This is our **general test equation**. To prove $\left(\frac{\partial C_V}{\partial V}\right)_T = 0$, we just need to prove that $\left(\frac{\partial^2 P}{\partial T^2}\right)_V = 0$.

#### Step 2: Test the Van der Waals Equation

Our task is now much simpler: just calculate $\left(\frac{\partial^2 P}{\partial T^2}\right)_V$ for the van der Waals gas.

First, let's take the VdW equation from the problem and solve it for $P$:

$$\left[P - a \left(\frac{N}{V}\right)^2\right] (V - Nb) = N k_B T$$

$$P - a \left(\frac{N}{V}\right)^2 = \frac{N k_B T}{V - Nb}$$

$$P(T, V) = \frac{N k_B T}{V - Nb} + a \left(\frac{N}{V}\right)^2$$

_(Note: This is the equation given in the problem. The standard VdW equation usually has a `+a` in the first bracket, which would result in a `-a` term here. However, the mathematical logic is identical, so we will proceed with the equation as written in your image!)_

Now, let's take the derivatives. We can write the equation as:

$P(T, V) = T \cdot \underbrace{\left( \frac{N k_B}{V - Nb} \right)}_{\text{function of V}} + \underbrace{\left( a \left(\frac{N}{V}\right)^2 \right)}_{\text{function of V}}$

Let's find the first derivative $\left(\frac{\partial P}{\partial T}\right)_V$:

$$\left(\frac{\partial P}{\partial T}\right)_V = \frac{\partial}{\partial T} \left[ T \left( \frac{N k_B}{V - Nb} \right) + a \left(\frac{N}{V}\right)^2 \right]$$

The second term, $a(N/V)^2$, has no $T$ dependence, so its derivative is 0.

The first term is just $T$ times a constant (since $V$ is held constant).

$$\left(\frac{\partial P}{\partial T}\right)_V = \frac{N k_B}{V - Nb}$$

Now, let's find the second derivative $\left(\frac{\partial^2 P}{\partial T^2}\right)_V$:

$$\left(\frac{\partial^2 P}{\partial T^2}\right)_V = \frac{\partial}{\partial T} \left[ \left(\frac{\partial P}{\partial T}\right)_V \right] = \frac{\partial}{\partial T} \left[ \frac{N k_B}{V - Nb} \right]$$

Look at the term we are differentiating: $\frac{N k_B}{V - Nb}$. This expression contains $N$, $k_B$, $V$, and $b$. It has no $T$ dependence at all.

Therefore, its derivative with respect to $T$ is zero.

$$\left(\frac{\partial^2 P}{\partial T^2}\right)_V = 0$$

---

### 💡 The "Big Picture" Conclusion

We can now go back to our general "test equation" from Step 1 and plug in our result.

$$\left(\frac{\partial C_V}{\partial V}\right)_T = T \left(\frac{\partial^2 P}{\partial T^2}\right)_V$$

$$\left(\frac{\partial C_V}{\partial V}\right)_T = T \cdot (0)$$

$$\left(\frac{\partial C_V}{\partial V}\right)_T = 0$$

We have successfully proven that for a van der Waals gas, the change in $C_V$ with respect to $V$ is zero. This means $C_V$ does not depend on volume.

Therefore, **$C_V$ must be a function only of temperature, $T$**.

The reason this works is that the van der Waals equation's pressure $P$ is "linear in $T$". That is, $P(T,V) = T \cdot f(V) + g(V)$. Any equation of state of this form will always have $\left(\frac{\partial^2 P}{\partial T^2}\right)_V = 0$, and therefore will always have a $C_V$ that depends only on temperature.

Congratulations on working through this entire problem! These three steps are a classic and fundamental part of thermodynamics.

Is there another topic in statistical physics you'd like to explore?