

Here is your **Quantum Mechanics Hydrogen Atom Cheat Sheet**. This covers every key concept we derived from Problem 5a to 5g.

You can save this summary to review before your exam. It connects the math to the physical intuition!

---

### **1. The Ground State & Probability (Parts 5a, 5b)**

-   The Wave Function:
    
    The ground state $\psi_{1,0,0}$ depends only on the radius $r$. It is spherically symmetric.
    
    $$\psi_{1,0,0} \propto e^{-r/a_0}$$
    
    (Source: Problem 5a)
    
-   Radial Probability Density $P(r)$:
    
    The probability of finding the electron at a distance $r$ (summed over all angles).
    
    $$P(r) = \frac{4}{a_0^3} r^2 e^{-\frac{2r}{a_0}}$$
    
    -   **Key Feature:** $P(0) = 0$ because of the $r^2$ volume term. The electron is essentially never _inside_ the nucleus.
        
-   Most Likely Radius:
    
    Where does the electron hang out the most? We found this by setting $\frac{dP}{dr} = 0$.
    
    $$r_{\text{max}} = a_0$$
    
    The electron is a cloud, but its "favorite" distance is exactly the Bohr radius.
    
    (Source: Problem 5b)
    

---

### **2. Uncertainty & Commutators (Parts 5c, 5d)**

-   The Commutator:
    
    Order matters! Position $\hat{r}$ and Radial Momentum $\hat{p}_r$ do not commute.
    
    $$[\hat{r}, \hat{p}_r] = i\hbar$$
    
    Meaning: You cannot measure the exact distance from the nucleus and the exact radial speed at the same time.
    
    (Source: Problem 5c)
    
-   Heisenberg Uncertainty Principle:
    
    The math must satisfy the inequality:
    
    $$\Delta r \cdot \Delta p_r \ge \frac{\hbar}{2}$$
    
    Our Result: For the ground state, we calculated:
    
    $$\Delta r \cdot \Delta p_r = \frac{\sqrt{3}}{2}\hbar \approx 0.866\hbar$$
    
    Since $0.866 > 0.5$, the hydrogen atom obeys the laws of quantum mechanics!
    
    (Source: Problem 5d)
    

---

### **3. Scaling Laws: "What if we change the atom?" (Parts 5e - 5g)**

Physicists love to see how things change if we swap the nucleus or the particle.

-   The "Master" Scaling Length ($a_1$):
    
    This replaces $a_0$ for generic atoms.
    
    $$a_1 = \frac{4\pi\epsilon_0\hbar^2}{m e^2 Z}$$
    
    (Source: Problem 5e)
    

![[Pasted image 20251208204014.png]]

---

### **Professor’s Final Exam Tip**

If you see a Hamiltonian that looks like this:

$$\hat{H} \propto -\frac{1}{2}\partial_r^2 - \frac{1}{r}$$

Don't panic! It is just the Hydrogen atom written in Atomic Units. It means they have scaled the length by $a_1$ and the energy by the Hartree energy to make the math clean.

Good luck with your studies! You have shown great intuition for Quantum Mechanics. Is there anything else you'd like to review?