

![[Pasted image 20260126135210.png]]

This is the most critical conceptual jump in understanding electrical transport! You have spotted a massive contradiction that puzzled physicists for a long time.

Let's look at part **b)**.

### 1. The Paradox (The Question)

**The Question (Image 1):**

> "Why is an equilibrium with **constant current flow** established after switching on the electric field, even though the solution in a) suggests an **accelerated motion** of the electrons?"

**Why this is confusing:**

In part **a)**, we found that $\frac{d\vec{k}}{dt}$ is proportional to the Electric Field $\vec{E}$.

Since momentum $\vec{p} = \hbar\vec{k}$ and velocity $\vec{v} = \vec{p}/m$, this implies:

$$\frac{d\vec{v}}{dt} \propto \vec{E}$$

This is simple acceleration ($a = F/m$). If you push a car in a friction-less vacuum, it goes faster and faster forever. It never settles at a "constant speed."

But in a wire, current is constant (Ohm's Law). The electrons don't accelerate to the speed of light! **Something must be stopping them.**

---

### 2. The Solution: Scattering (The Missing Piece)

**The Answer (Image 2):**

> "Entgegen der Beschleunigung durch das elektrische Feld sorgen Streuprozesse für eine Verschiebung der Fermikugel in den Ausgangszustand."

**Translation:**

"Counteracting the acceleration by the electric field, **scattering processes** ensure a displacement of the Fermi sphere [back] into the initial state."

### 3. Deep Dive: What is actually happening?

To understand this, we need a mental model. Let's use the **"Skydiver Analogy."**

#### The Acceleration (Part A)

Imagine a skydiver jumping out of a plane. Gravity pulls them down.

-   **Gravity** = The Electric Field ($\vec{E}$).
    
-   **The Skydiver** = The Electron.
    
    If there were no air, the skydiver would accelerate forever until they hit the ground. This is what part **a)** described—pure acceleration.
    

#### The "Friction" (Part B)

But there _is_ air. The skydiver hits air molecules. These collisions slow them down.

-   **Air Resistance** = **Scattering**.
    

In a metal, electrons don't fly through empty space. They fly through a crystal lattice of atoms. They constantly crash into things:

1.  **Impurities:** Foreign atoms or defects in the metal structure.
    
2.  **Phonons:** The atoms of the metal are vibrating (heat). Electrons crash into these vibrating atoms.
    

#### The Equilibrium (Terminal Velocity)

Eventually, the skydiver reaches a speed where the **pull of gravity** exactly equals the **push of air resistance**. They stop accelerating and fall at a constant speed ("Terminal Velocity").

In the metal:

-   The Electric Field pushes the Fermi Sphere to the **right** (increasing $\vec{k}$).
    
-   Scattering events knock electrons out of their path, effectively relaxing the Fermi Sphere back toward the **center** (decreasing average $\vec{k}$).
    

**Equilibrium happens when:**

$$\text{Rate of Acceleration (from Field)} = \text{Rate of Relaxation (from Scattering)}$$

This results in a constant average drift velocity, which we measure as a **constant current**.

---

### 4. Visualizing the Fermi Sphere

Here is how a solid-state physicist pictures this balance:

1.  **Step 1 (Field On):** The Electric Field applies a force, shifting the _entire_ Fermi sphere of electrons slightly to the right (in k-space).
    
2.  **Step 2 (Scattering):** An electron on the far right (high energy) hits an impurity. It loses that extra momentum and "scatters" back to an empty spot on the left side of the sphere.
    
3.  **The Result:** The sphere looks like it is stationary, but slightly shifted off-center. It isn't moving further right because for every tiny push to the right, scattering knocks an electron back.
    

This steady, shifted position represents a constant non-zero average momentum $\langle \vec{k} \rangle$, and therefore a constant current!

Ready for the next part? We usually have to combine these two ideas mathematically next!