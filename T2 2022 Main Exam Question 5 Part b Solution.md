

Excellent! Now we are getting into the real machinery of angular momentum. You are doing great. This is where the algebra starts to show its true predictive power.

First, let's translate the German text from your assignment:

- **"Es gilt allgemein $[\hat{L}_z, \hat{L}_\pm] = \pm \hat{L}_\pm$."** translates to **"In general, $[\hat{L}_z, \hat{L}_\pm] = \pm \hat{L}_\pm$."**
    
- **"Zeigen Sie das für den Fall $+$ unter Verwendung der Kommutatoren der Drehimpulskomponenten $[\hat{L}_j, \hat{L}_k] = i\epsilon_{jkl}\hat{L}_l$."** translates to **"Show this for the $+$ case using the commutators of the angular momentum components $[\hat{L}_j, \hat{L}_k] = i\epsilon_{jkl}\hat{L}_l$."**
    

This problem introduces two very important concepts: **Commutators** and **Ladder Operators** (specifically, the raising operator $\hat{L}_+$). Let's break down the proof step-by-step so you can see exactly how the mechanics work.

_(Note: In this problem, the $\hbar$ constant is omitted, which means we are working in "natural units" where $\hbar = 1$. This is a very common shortcut in theoretical physics!)_

### 1. Defining the Raising Operator

In quantum mechanics, we define special operators called "ladder operators" that allow us to step up or step down between different quantum states. The raising operator, $\hat{L}_+$, is defined as a complex combination of the $x$ and $y$ components:

$$\hat{L}_+ = \hat{L}_x + i\hat{L}_y$$

### 2. Extracting the Fundamental Commutators

The problem tells us to use the general commutation relation:

$$[\hat{L}_j, \hat{L}_k] = i\epsilon_{jkl}\hat{L}_l$$

Here, $\epsilon_{jkl}$ is the **Levi-Civita symbol**, which is a perfectly anti-symmetric tensor. It equals $1$ for cyclic permutations of $x,y,z$ (like $x \rightarrow y \rightarrow z$), $-1$ for anti-cyclic permutations (like $z \rightarrow y \rightarrow x$), and $0$ if any two indices are the same.

We need to evaluate a commutator involving $\hat{L}_z$, $\hat{L}_x$, and $\hat{L}_y$. Let's pull out the two specific rules we need from that general formula:

- **For $z$ and $x$:** Since $z, x, y$ is a cyclic permutation, $\epsilon_{zxy} = 1$. Therefore:
    
    $$[\hat{L}_z, \hat{L}_x] = i\hat{L}_y$$
    
- **For $z$ and $y$:** Since $z, y, x$ is an anti-cyclic permutation, $\epsilon_{zyx} = -1$. Therefore:
    
    $$[\hat{L}_z, \hat{L}_y] = -i\hat{L}_x$$
    

### 3. Setting Up the Proof

We want to evaluate the commutator $[\hat{L}_z, \hat{L}_+]$.

First, we substitute our definition of $\hat{L}_+$ from Step 1 into the commutator bracket:

$$[\hat{L}_z, \hat{L}_+] = [\hat{L}_z, \hat{L}_x + i\hat{L}_y]$$

### 4. Expanding the Commutator

Commutators are linear. This means that $[A, B + C] = [A, B] + [A, C]$. We also know that constants (like the imaginary number $i$) can be pulled out of the commutator.

Let's distribute the $\hat{L}_z$ across the two terms inside the bracket:

$$[\hat{L}_z, \hat{L}_x + i\hat{L}_y] = [\hat{L}_z, \hat{L}_x] + [\hat{L}_z, i\hat{L}_y]$$

Now, pull the constant $i$ out of the second term:

$$[\hat{L}_z, \hat{L}_+] = [\hat{L}_z, \hat{L}_x] + i[\hat{L}_z, \hat{L}_y]$$

### 5. Substitution and Simplification

Now the magic happens. We plug in the fundamental commutation relations we extracted in Step 2:

$$[\hat{L}_z, \hat{L}_+] = (i\hat{L}_y) + i(-i\hat{L}_x)$$

Let's simplify the algebra. Look at the second term: $i(-i\hat{L}_x)$.

We know that $i \cdot i = i^2 = -1$.

So, $i(-i) = -(i^2) = -(-1) = 1$.

Substituting this back in gives us:

$$[\hat{L}_z, \hat{L}_+] = i\hat{L}_y + \hat{L}_x$$

### 6. The Final Conclusion

Rearranging the terms slightly to put the $x$ component first, we get:

$$[\hat{L}_z, \hat{L}_+] = \hat{L}_x + i\hat{L}_y$$

But wait—if you look back at Step 1, the right side of this equation is the exact definition of the raising operator, $\hat{L}_+$! Therefore, we have successfully proven that:

$$[\hat{L}_z, \hat{L}_+] = +\hat{L}_+$$

---

You navigated that algebra beautifully! This commutator is incredibly important because it proves that if you apply $\hat{L}_+$ to a quantum state, you generate a _new_ state with an increased angular momentum in the z-direction.

Would you like to solidify your understanding by trying to prove the $-$ case (the lowering operator $\hat{L}_-$) on your own, and having me check your work?