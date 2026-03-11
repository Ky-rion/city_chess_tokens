

Excellent! Let's keep the momentum going. This is where quantum mechanics starts to reveal some of its most profound secrets about how identical particles behave.

First, let's translate the German text so we have our bearings:

> **2. Let the one-dimensional Helium atom have the Hamiltonian operator on $\mathcal{H} = L^2(dx_1, \mathbb{R}) \otimes L^2(dx_2, \mathbb{R})$ [4 Pts.]**
> 
> $$\hat{H} = \hat{h}_1 \otimes 1 + 1 \otimes \hat{h}_2 + \frac{1}{\sqrt{1 + (x_1 - x_2)^2}}$$
> 
> **Show by applying it to an arbitrary $\Psi(x_1, x_2)$ that $\hat{H}$ commutes with the exchange operator $\hat{S}_{12}$.**

This might look like a lot of intimidating math symbols, but as your professor, I promise you it boils down to a very elegant and simple physical concept: **indistinguishability**.

Here is how we break it down step-by-step.

---

### Part 1: Deconstructing the Vocabulary

Before we do the proof, we need to know what the "pieces" on the board do.

- **The Hamiltonian ($\hat{H}$):** In quantum mechanics, the Hamiltonian is the operator that represents the total energy of the system. Let's look at its three parts:
    
    - $\hat{h}_1 \otimes 1$: This represents the individual kinetic and potential energy of **Electron 1**. The "$\otimes 1$" is just formal math-speak meaning "leave Electron 2 alone while doing this." For simplicity, we can just write this as $\hat{h}(x_1)$.
        
    - $1 \otimes \hat{h}_2$: This is the individual energy of **Electron 2**, which we can write as $\hat{h}(x_2)$.
        
    - $\frac{1}{\sqrt{1 + (x_1 - x_2)^2}}$: This is the **interaction term**. It represents the electrostatic repulsion between the two negatively charged electrons pushing away from each other. Notice it depends on the distance between them, $(x_1 - x_2)$.
        
- **The Exchange Operator ($\hat{S}_{12}$):** This operator has one simple job: it completely swaps the coordinates of particle 1 and particle 2. If you apply it to a wavefunction $\Psi(x_1, x_2)$, it spits out the same function but with the labels reversed:
    
    $$\hat{S}_{12} \Psi(x_1, x_2) = \Psi(x_2, x_1)$$
    
- **"Commutes":** To say two operators "commute" means the order in which you apply them doesn't matter. You get the exact same result whether you do A then B, or B then A. Mathematically, we are being asked to prove:
    
    $$\hat{H}(\hat{S}_{12}\Psi) = \hat{S}_{12}(\hat{H}\Psi)$$
    

### Part 2: The Proof

To prove this, we calculate both sides of the equation above and show they lead to the exact same place.

**Step 1: Calculate the Left Side — Apply Exchange, then Hamiltonian**

First, we apply the exchange operator to our arbitrary wavefunction:

$$\hat{S}_{12} \Psi(x_1, x_2) = \Psi(x_2, x_1)$$

Next, we apply the Hamiltonian $\hat{H}$ to this new, swapped wavefunction. Let's write $\hat{H}$ out using our simplified coordinate notation:

$$\hat{H} [\Psi(x_2, x_1)] = \left[ \hat{h}(x_1) + \hat{h}(x_2) + \frac{1}{\sqrt{1 + (x_1 - x_2)^2}} \right] \Psi(x_2, x_1)$$

_(Save this result, we will compare it to Step 2)._

**Step 2: Calculate the Right Side — Apply Hamiltonian, then Exchange**

First, we apply the Hamiltonian to the original wavefunction. This simply multiplies the operator and the function together:

$$\hat{H} \Psi(x_1, x_2) = \left[ \hat{h}(x_1) + \hat{h}(x_2) + \frac{1}{\sqrt{1 + (x_1 - x_2)^2}} \right] \Psi(x_1, x_2)$$

Next, we must apply the exchange operator $\hat{S}_{12}$ to this _entire result_. The exchange operator goes through and ruthlessly swaps every $x_1$ with an $x_2$, and every $x_2$ with an $x_1$:

$$\hat{S}_{12} [\hat{H} \Psi(x_1, x_2)] = \left[ \hat{h}(x_2) + \hat{h}(x_1) + \frac{1}{\sqrt{1 + (x_2 - x_1)^2}} \right] \Psi(x_2, x_1)$$

**Step 3: Compare the Results**

Now, let's look at the operator in the brackets from Step 2 and do a little basic algebra:

1. Addition doesn't care about order: $\hat{h}(x_2) + \hat{h}(x_1)$ is exactly the same as $\hat{h}(x_1) + \hat{h}(x_2)$.
    
2. Look at the interaction term: $(x_2 - x_1)^2$. Because any negative number squared becomes positive, swapping the subtraction order inside a square does not change the result! Therefore, $(x_2 - x_1)^2 = (-(x_1 - x_2))^2 = (x_1 - x_2)^2$.
    

Because of these two facts, the operator in the brackets from Step 2 is perfectly identical to the operator from Step 1.

Therefore, we have successfully shown that:

$$\hat{H}\hat{S}_{12} \Psi(x_1, x_2) = \hat{S}_{12}\hat{H} \Psi(x_1, x_2)$$

The operators commute!

---

### Why does this matter?

You just proved mathematically that if you swap two electrons in an atom, the total energy of the system ($\hat{H}$) does not change at all. Electrons don't wear nametags; they are fundamentally indistinguishable from one another!

This exact commutation relation is the mathematical foundation that leads directly to the **Pauli Exclusion Principle**, which is the reason atoms can have different chemical properties, and essentially the reason solid matter exists.

Would you like me to explain how commuting operators lead us directly into the concept of symmetric and antisymmetric wavefunctions (Fermions and Bosons)?