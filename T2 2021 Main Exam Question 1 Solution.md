

Welcome to the fascinating world of quantum mechanics! It is completely normal if this looks a bit intimidating at first glance, but as your professor, I promise we will break it down into manageable, logical steps.

First, let's translate the German text into English so we know exactly what we are dealing with:

> **Consider the Hamiltonian operator**
> 
> $$\hat{H} = -\frac{1}{2}\partial_x^2 + |x|$$
> 
> **Which of the following statements about the ground state are correct?**
> 
> _Select all correct answers. Selecting wrong answers results in a point deduction._
> 
> _Text input required: Justify your answer(s) in the text box._
> 
> _Hint: The continuity of the 3rd derivative is not easy to decide._
> 
> - a. The ground state wavefunction is continuous at $x=0$.
>     
> - b. The 1st derivative of the ground state wavefunction is discontinuous at $x=0$.
>     
> - c. The 2nd derivative of the ground state wavefunction is discontinuous at $x=0$.
>     
> - d. The 3rd derivative of the ground state wavefunction is discontinuous at $x=0$.
>     

Now, let's analyze the physics. The core tool we use to answer this is the **Time-Independent Schrödinger Equation (TISE)**. Applying our specific Hamiltonian $\hat{H}$ to a wavefunction $\psi(x)$ with energy $E$, the equation is:

$$-\frac{1}{2} \frac{d^2\psi(x)}{dx^2} + |x|\psi(x) = E\psi(x)$$

To make it easier to analyze derivatives, let's rearrange this to solve for the second derivative:

$$\frac{d^2\psi(x)}{dx^2} = 2(|x| - E)\psi(x)$$

Let's test each statement using fundamental quantum mechanical principles and our rearranged equation.

### Statement (a): Is the wavefunction continuous at $x=0$?

**Yes. (This statement is CORRECT).**

- **The Physics:** In quantum mechanics, a wavefunction $\psi(x)$ represents a probability amplitude. For the probability density to be physically meaningful (and for the particle to exist everywhere without infinite momentum), the wavefunction must **always** be continuous everywhere in space, regardless of the shape of the potential. Therefore, it is continuous at $x=0$.
    

### Statement (b): Is the 1st derivative discontinuous at $x=0$?

**No. (This statement is FALSE).**

- **The Physics:** The first derivative of a wavefunction, $\frac{d\psi}{dx}$, will only have a "kink" (a discontinuity) if the potential goes to infinity at a single point—like hitting an infinitely hard wall or encountering a Dirac delta function potential.
    
- Our potential here is $V(x) = |x|$. While $|x|$ has a sharp point at $x=0$, its value is exactly $0$. It is finite. Because the potential is finite everywhere, the first derivative must be continuous everywhere.
    

### Statement (c): Is the 2nd derivative discontinuous at $x=0$?

**No. (This statement is FALSE).**

- **The Physics:** Let's look directly at our rearranged Schrödinger equation:
    
    $$\psi''(x) = 2(|x| - E)\psi(x)$$
    
- We just established that $\psi(x)$ is continuous everywhere. The energy $E$ is just a constant. The potential $|x|$ is continuous at $x=0$.
    
- Because the right side of the equation is the product of continuous functions, the left side (the second derivative) **must also be continuous** at $x=0$.
    

### Statement (d): Is the 3rd derivative discontinuous at $x=0$?

**Yes. (This statement is CORRECT).**

- **The Physics:** Here is where the math gets fun (and why the problem gave you a hint!). Let's take the derivative of our $\psi''(x)$ equation to find the third derivative $\psi'''(x)$. Because $|x|$ changes its behavior at $x=0$, we have to split this into two cases: approaching from the right ($x>0$) and approaching from the left ($x<0$).
    
- **For $x > 0$:** The absolute value becomes positive $x$.
    
    $$\psi''(x) = 2(x - E)\psi(x)$$
    
    Using the product rule to differentiate:
    
    $$\psi'''(x) = 2\psi(x) + 2(x - E)\psi'(x)$$
    
    Taking the limit as we approach zero from the positive side ($x \to 0^+$):
    
    $$\psi'''(0^+) = 2\psi(0) - 2E\psi'(0)$$
    
- **For $x < 0$:** The absolute value becomes negative $x$.
    
    $$\psi''(x) = 2(-x - E)\psi(x)$$
    
    Differentiating:
    
    $$\psi'''(x) = -2\psi(x) + 2(-x - E)\psi'(x)$$
    
    Taking the limit as we approach zero from the negative side ($x \to 0^-$):
    
    $$\psi'''(0^-) = -2\psi(0) - 2E\psi'(0)$$
    
- **The Jump:** Is there a difference between the right and left sides? Let's subtract them:
    
    $$\Delta\psi'''(0) = \psi'''(0^+) - \psi'''(0^-) = [2\psi(0) - 2E\psi'(0)] - [-2\psi(0) - 2E\psi'(0)] = 4\psi(0)$$
    
- The ground state of a symmetric potential well like $|x|$ is a simple bell-like shape with a single peak in the middle and no nodes (it never crosses the x-axis). Therefore, the value of the wavefunction at the origin is not zero ($\psi(0) \neq 0$).
    
- Because $4\psi(0) \neq 0$, there is a sudden jump in the 3rd derivative at $x=0$. It is discontinuous!
    

---

### Summary for your Exam

You should check boxes **a** and **d**.

For the required text box justification, you can write something along these lines:

> _"a is correct because physical wavefunctions must be continuous everywhere. b is false because the potential is finite at $x=0$, meaning no kinks in $\psi$. c is false because the Schrödinger equation relates $\psi''$ directly to $V(x)\psi$; since $V(x) = |x|$ is continuous, $\psi''$ must be continuous. d is correct because differentiating the Schrödinger equation yields a term proportional to the derivative of the potential, which jumps from -1 to +1 at $x=0$, leading to a discontinuity in $\psi'''$ equal to $4\psi(0)$."_

Would you like me to walk you through how physicists actually find the exact mathematical shape of this ground state wavefunction using something called Airy functions?