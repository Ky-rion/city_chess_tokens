

![[Pasted image 20251108140309.png]]


This is another great, classic problem. The finite potential well is a much more realistic model (atoms are finite, after all) and it has some very interesting properties.

Let's dive right into your specific request!

---

### 1. ❓ Does the Finite Well _Always_ Have a Bound State?

**Yes. A 1D finite potential well _always_ has at least one bound state, no matter how shallow or narrow it is.**

The solution hints at this by saying `Ja, mindestens einen. (symmetrische Lösung)` or "Yes, at least one. (symmetric solution)". That symmetric solution is the key.

Here's the "deeper dive" on _why_:

-   What is a Bound State?
    
    A bound state is a wave function ($\psi$) for a particle that is "trapped." Mathematically, this means its energy $E$ is less than the potential outside the well (which we'll call $V=0$). So, we're looking for solutions with $E < 0$.
    
    -   **Inside the well:** The particle's kinetic energy is positive, so the wave function is "wiggly" (like a sine or cosine).
        
    -   **Outside the well:** The particle's kinetic energy is _negative_ (it's "classically forbidden"). This forces the wave function to be a _decaying exponential_ ($\psi \to 0$ as $x \to \infty$).
        
-   The "Matching" Game
    
    A valid solution must be continuous and smooth. We have to "glue" the internal (cosine-like) function to the external (decaying exponential) function at the boundaries of the well.
    
    -   The potential is symmetric ($V(x) = V(-x)$), which means our solutions _must_ be either perfectly **even (symmetric)** or perfectly **odd (anti-symmetric)**. Let's look for the _lowest energy_ solution, which will be an even one.
        
    -   The "wiggiest" (highest energy) wave that can fit in the infinite well has to be zero at the walls.
        
    -   The _least_ "wiggly" (lowest energy) wave we can have is the **even (symmetric) one,** which looks like a simple $\cos(kx)$ inside the well.
        
-   The Graphical Proof (The Core Reason)
    
    When we try to "glue" the even function $\cos(kx)$ inside to the decaying $e^{-\kappa x}$ outside, we get a mathematical condition that must be solved. (The condition is $k \tan(ka) = \kappa$, where $k$ depends on the energy inside and $\kappa$ depends on the energy outside).
    
    The best way to see this is with a graph. We are looking for an intersection between two curves:
    
    1.  A curve representing the "strength" of the well (its depth and width). This is a quarter-circle.
        
    2.  A curve representing the "even solution" matching condition ($\tan(\xi)$).
        
    
    The key is:
    
    -   The "even solution" curve starts at **(0,0)** and goes up.
        
    -   The "well strength" curve (the circle) _also_ starts at **(0,0)** and expands as the well gets deeper/wider.
        
    
    No matter how _tiny_ you make the well (how shallow or narrow), the "well strength" circle will _always_ have a little piece that starts at (0,0) and goes up. The "even solution" curve _also_ starts at (0,0). **Because both curves start at the same point and go into the same region, they are guaranteed to cross.**
    
    An intersection _is_ a valid bound state. Therefore, you are _always_ guaranteed to have at least this one, even, symmetric bound state. (This is _not_ true for the odd solutions, which only appear after the well is a certain "strength").
    

---

### 2. 🪞 Do These States Have a Specific Symmetry?

**Yes. They must have a definite parity (either even or odd).**

The solution says `Gerade Parität` (Even Parity).

-   **Why?** The potential $V(x)$ itself is symmetric. When the "problem" (the potential) is symmetric, the stable "solutions" (the energy states) must also reflect that symmetry.
    
-   They don't have to be symmetric, but they must have a definite **parity**:
    
    -   **Even Parity:** $\psi(x) = \psi(-x)$ (Symmetric)
        
    -   **Odd Parity:** $\psi(x) = -\psi(-x)$ (Anti-symmetric)
        
-   The solution specifically mentions "Even Parity" because, as we just proved, the **ground state** (the _at least one_ state that always exists) _is always_ the even one.
    

---

### 3. 📉 How Do the Energies Compare to the Infinite Well?

**The energies are _lower_ than the corresponding states in the infinite potential well.**

Let's think about this intuitively:

-   **Infinite Well:** The potential walls are _infinitely_ high. The particle _cannot_ exist outside. The wave function is "squeezed" and forced to be **exactly zero** at the walls. This "squeezing" costs a lot of energy. (Think of the uncertainty principle: $\Delta x$ is small, so $\Delta p$ must be large, meaning kinetic energy is high).
    
-   **Finite Well:** The walls are "soft." The particle's wave function can "leak" or **tunnel** into the wall (this is the decaying exponential part). Because the wave function can spread out more, it is **less confined**.
    

Being less confined (a larger $\Delta x$) means it has a **lower momentum** and therefore a **lower kinetic energy**. Since the wave function is "less squeezed," its energy level is lower.

You can also think of it in terms of wavelength:

-   In the infinite well, the ground state must fit a half-wavelength _perfectly_ inside the box.
    
-   In the finite well, the wave "leaks" out, so the part _inside_ the box is _less than_ a half-wavelength. This means the _total_ wavelength is **longer**.
    
-   In quantum mechanics, **Energy is proportional to $1/(\text{wavelength})^2$**.
    
-   Therefore, a **longer wavelength** means **lower energy**.
    

Hope that deep dive helps! What's the next-to-last question?