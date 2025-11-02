

Of course! This calculation is a perfect application of the rules we just derived in part (c). Let's do this step-by-step.

The quantity $\langle n | \hat{O} | n \rangle$ is called the **expectation value** of the operator $\hat{O}$ in the state $|n\rangle$. Physically, it represents the _average_ value you would get if you measured the observable $O$ many times on identical systems all in the state $|n\rangle$.

We need to calculate two of these: $\langle n | \hat{x} | n \rangle$ and $\langle n | \hat{p} | n \rangle$.

---

### 1. 📏 Calculation of $\langle n | \hat{x} | n \rangle$ (Expectation Value of Position)

1.  Substitute the definition of $\hat{x}$:
    
    We start with our expression and replace $\hat{x}$ with its definition in terms of $\hat{a}$ and $\hat{a}^\dagger$:
    
    $\langle n | \hat{x} | n \rangle = \left\langle n \left| \left( \frac{1}{\sqrt{2}}(\hat{a}^\dagger + \hat{a}) \right) \right| n \right\rangle$
    
2.  Pull out the constant:
    
    The number $\frac{1}{\sqrt{2}}$ can be pulled out of the entire expression:
    
    $= \frac{1}{\sqrt{2}} \langle n | (\hat{a}^\dagger + \hat{a}) | n \rangle$
    
3.  Distribute the expression:
    
    We can split this into two separate expectation values:
    
    $= \frac{1}{\sqrt{2}} \left( \langle n | \hat{a}^\dagger | n \rangle + \langle n | \hat{a} | n \rangle \right)$
    
4.  Use the rules from part (c):
    
    Now, let's look at each part inside the main parentheses. We'll use the rules $\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$ and $\hat{a}|n\rangle = \sqrt{n}|n-1\rangle$.
    
    -   **First term:** $\langle n | \hat{a}^\dagger | n \rangle = \langle n | \left( \sqrt{n+1}|n+1\rangle \right) = \sqrt{n+1} \langle n | n+1 \rangle$
        
    -   **Second term:** $\langle n | \hat{a} | n \rangle = \langle n | \left( \sqrt{n}|n-1\rangle \right) = \sqrt{n} \langle n | n-1 \rangle$
        
5.  Use Orthonormality:
    
    This is the key step! The states are orthonormal, which means $\langle m | n \rangle = 0$ if $m \neq n$.
    
    -   In the first term, $\langle n | n+1 \rangle = 0$ (because $n \neq n+1$).
        
    -   In the second term, $\langle n | n-1 \rangle = 0$ (because $n \neq n-1$).
        
6.  Find the result:
    
    Let's substitute these zeros back in:
    
    $= \frac{1}{\sqrt{2}} \left( \sqrt{n+1} \cdot (0) + \sqrt{n} \cdot (0) \right)$
    
    $= \frac{1}{\sqrt{2}} (0 + 0) = 0$
    

So, **$\langle n | \hat{x} | n \rangle = 0$**.

---

### 2. 💨 Calculation of $\langle n | \hat{p} | n \rangle$ (Expectation Value of Momentum)

The process is almost identical.

1.  Substitute the definition of $\hat{p}$:
    
    $\langle n | \hat{p} | n \rangle = \left\langle n \left| \left( \frac{i}{\sqrt{2}}(\hat{a}^\dagger - \hat{a}) \right) \right| n \right\rangle$
    
2.  Pull out the constant:
    
    $= \frac{i}{\sqrt{2}} \langle n | (\hat{a}^\dagger - \hat{a}) | n \rangle$
    
3.  Distribute the expression:
    
    $= \frac{i}{\sqrt{2}} \left( \langle n | \hat{a}^\dagger | n \rangle - \langle n | \hat{a} | n \rangle \right)$
    
4.  Use the rules and Orthonormality (same as before):
    
    We already found that $\langle n | \hat{a}^\dagger | n \rangle = 0$ and $\langle n | \hat{a} | n \rangle = 0$.
    
5.  Find the result:
    
    Let's substitute these zeros:
    
    $= \frac{i}{\sqrt{2}} ( 0 - 0 ) = 0$
    

So, **$\langle n | \hat{p} | n \rangle = 0$**.

---

## 💡 The Physical Meaning

This result makes perfect physical sense. The states $|n\rangle$ are **stationary states**, meaning their properties don't change in time. For a particle in a symmetric potential like the harmonic oscillator (which is centered at $x=0$), the particle is, on average, exactly at the center. It's equally likely to be found on the left side as on the right side, so its average position $\langle \hat{x} \rangle$ is $0$.

Similarly, it's equally likely to be moving to the left as it is to the right, so its average momentum $\langle \hat{p} \rangle$ is also $0$.

Here is the next question in the series:

{

type: uploaded file

fileName: image_52077e.png