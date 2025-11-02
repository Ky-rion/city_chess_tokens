

Excellent! Let's tackle part (b). This will be very similar to part (a), but with a crucial difference.

## 🧠 The Goal: What Are We Trying to Do?

This time, the problem asks us to show that the state $\hat{a}|n\rangle$ is _also_ an eigenstate of $\hat{H}$ and to find its eigenvalue.

Just like before, this means we need to apply the Hamiltonian $\hat{H}$ to this new state and see if we get a _number_ times the _same state_ back:

$\hat{H} \left( \hat{a}|n\rangle \right) = (\text{some new number}) \times \left( \hat{a}|n\rangle \right)$

Let's begin the calculation.

---

## 🔬 The Calculation: Step-by-Step

We need to "swap" the $\hat{H}$ and $\hat{a}$ operators. To do that, we must first find their commutation relation, $[\hat{H}, \hat{a}]$.

### Step 1: Find the "Swapping Rule" (the Commutator)

-   Start with the definition:
    
    $[\hat{H}, \hat{a}] = \left[ \left(\hat{a}^\dagger \hat{a} + \frac{1}{2}\right), \hat{a} \right]$ (using Equation 6)
    
-   Again, the number $\frac{1}{2}$ commutes with everything, so its commutator is zero:
    
    $[\hat{H}, \hat{a}] = [\hat{a}^\dagger \hat{a}, \hat{a}] + [\frac{1}{2}, \hat{a}] = [\hat{a}^\dagger \hat{a}, \hat{a}]$
    
-   Use the same identity as last time, $[\hat{A}\hat{B}, \hat{C}] = \hat{A}[\hat{B}, \hat{C}] + [\hat{A}, \hat{C}]\hat{B}$:
    
    $[\hat{a}^\dagger \hat{a}, \hat{a}] = \hat{a}^\dagger [\hat{a}, \hat{a}] + [\hat{a}^\dagger, \hat{a}] \hat{a}$
    
-   Now, let's look at the two commutators we have:
    
    1.  $[\hat{a}, \hat{a}] = 0$, because any operator commutes with itself.
        
    2.  $[\hat{a}^\dagger, \hat{a}]$: From Equation (7), we know $[\hat{a}, \hat{a}^\dagger] = 1$. The commutator $[\hat{B}, \hat{A}]$ is just $-[\hat{A}, \hat{B}]$. Therefore, **$[\hat{a}^\dagger, \hat{a}] = -1$**. This minus sign is the crucial difference!
        
-   Substitute these back in:
    
    $[\hat{a}^\dagger \hat{a}, \hat{a}] = \hat{a}^\dagger (0) + (-1) \hat{a} = -\hat{a}$
    
-   So, we've found our new rule:
    
    $[\hat{H}, \hat{a}] = -\hat{a}$
    
-   Let's expand this to get our swapping relation:
    
    $\hat{H}\hat{a} - \hat{a}\hat{H} = -\hat{a}$
    
-   Rearranging gives:
    
    $\hat{H}\hat{a} = \hat{a}\hat{H} - \hat{a}$
    

### Step 2: Apply the Rule to Our State

Now we're ready to solve the main problem.

$\hat{H} \left( \hat{a}|n\rangle \right)$

-   Use the swapping rule we just found:
    
    $= \left( \hat{a}\hat{H} - \hat{a} \right) |n\rangle$
    
-   Distribute the state $|n\rangle$ to both terms:
    
    $= \hat{a}\hat{H}|n\rangle - \hat{a}|n\rangle$
    
-   Now, just like before, use Equation (8) on the term $\hat{H}|n\rangle$:
    
    $= \hat{a} \left( (n + \frac{1}{2})|n\rangle \right) - \hat{a}|n\rangle$
    
-   Pull the number $\left(n + \frac{1}{2}\right)$ out to the front (it commutes past the $\hat{a}$ operator):
    
    $= \left(n + \frac{1}{2}\right) \hat{a}|n\rangle - \hat{a}|n\rangle$
    
-   We can now factor out the state $\hat{a}|n\rangle$:
    
    $= \left( \left(n + \frac{1}{2}\right) - 1 \right) \hat{a}|n\rangle$
    
-   And simplify the number:
    
    $= \left( n - 1 + \frac{1}{2} \right) \hat{a}|n\rangle$
    

---

## ✅ Conclusion and Meaning

Let's write down our final result:

$\hat{H} \left( \hat{a}|n\rangle \right) = \left( n - 1 + \frac{1}{2} \right) \left( \hat{a}|n\rangle \right)$

This again perfectly matches the eigenstate equation.

1.  Is $\hat{a}|n\rangle$ an eigenstate of $\hat{H}$?
    
    Yes, it is. (Or it's the zero vector, which we'll discuss in a second). When $\hat{H}$ acts on it, we get the same state $\hat{a}|n\rangle$ back, multiplied by a number.
    
2.  What is the new eigenvalue?
    
    The new eigenvalue (the energy) is $\left(n - 1 + \frac{1}{2}\right)$.
    

### 💡 The Physical Meaning (The "Other Half" of the Ladder)

In part (a), we saw that $\hat{a}^\dagger$ (the **creation operator**) _raises_ the energy of the state by one quantum.

Now, we see that $\hat{a}$ does the exact opposite: it _lowers_ the energy of the state by one quantum. For this reason, $\hat{a}$ is called the **"annihilation operator"** or **"lowering operator"**.

Together, $\hat{a}$ and $\hat{a}^\dagger$ form the "ladder operators," allowing us to move up and down the ladder of energy eigenstates.

> A quick note on that "or vanishes" part:
> 
> The problem text mentions that the state $\hat{a}|n\rangle$ could "vanish" (become zero). What does this mean?
> 
> Imagine we are in the lowest possible energy state, the "ground state," which is $|0\rangle$ (where $n=0$). Its energy is $E_0 = (0 + \frac{1}{2}) = \frac{1}{2}$.
> 
> What happens if we try to lower this state? Our formula would give:
> 
> $E_{new} = (0 - 1 + \frac{1}{2}) = -\frac{1}{2}$.
> 
> But we know $E_0 = \frac{1}{2}$ is the lowest energy. The system can't have negative energy. The only way for the math to be consistent is if the new state itself doesn't exist. That is, the state vector "vanishes":
> 
> $\hat{a}|0\rangle = 0$
> 
> The annihilation operator "annihilates" the ground state, which is precisely why the energy ladder has a bottom rung!

This completes the algebraic part of the problem. We've successfully used the commutation relations to find the eigenvalues of the "raised" and "lowered" states.

Would you like to discuss what happens when we apply $\hat{a}^\dagger \hat{a}$ to an eigenstate $|n\rangle$?