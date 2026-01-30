

![[Pasted image 20260128115713.png]]

Welcome to your first day of Particle Physics! I am delighted to have you here. Don't be intimidated by the Greek letters or the squiggly lines; at its heart, this subject is just about tracking where energy goes when things bump into each other.

We are looking at **Elastic Electron-Nucleon Scattering**.

Let's break down the solution provided in the image for **Part (a)**. This is the foundation for everything else we will do in this problem.

---

### 1. The Big Picture: What is happening?

Imagine a game of billiards.

-   The **electron ($e^-$)** is the cue ball. It is moving very fast (high energy).
    
-   The **proton ($p$)** is the 8-ball. It is sitting completely still on the table.
    
-   **Elastic Scattering** means the cue ball hits the 8-ball and they both bounce off. The balls don't break apart, and they don't stick together. They just trade some momentum.
    

In particle physics, however, particles don't actually touch. Instead, they throw a "ball" at each other to push one another away. That "ball" is a force carrier. In this case, since the electron and proton are both electrically charged, they exchange a **photon ($\gamma$)**.

### 2. The Sketch (The Feynman Diagram)

Look at the drawing in your solution. This is a **Feynman Diagram**. We usually read these from left to right (time flows forward).

-   **The Top Line (The Electron):**
    
    -   On the left, you see an arrow pointing in. That is the incoming electron ($e^-$).
        
    -   It hits a central point (vertex), emits a squiggly line, and bounces off to the top right. That is the outgoing electron.
        
-   **The Squiggly Line (The Interaction):**
    
    -   This represents the **virtual photon ($\gamma$)**. It connects the electron to the proton. It carries the "kick" or the force from the electron to the proton.
        
-   **The Bottom Line (The Proton):**
    
    -   On the bottom left, you have the proton sitting there.
        
    -   It absorbs the squiggly photon at the bottom vertex.
        
    -   It recoils (gets kicked) to the bottom right.
        

### 3. The Math: Defining Four-Vectors

In our world, we use 3D vectors $(x, y, z)$ to describe momentum. In Special Relativity (which we must use because $25\text{ GeV}$ is very fast!), we use **Four-Vectors**. A four-vector packs **Energy** (time component) and **Momentum** (space components) into one package.

The format is always:

$$\mathbf{V} = ( \text{Energy}/c, \text{Momentum}_x, \text{Momentum}_y, \text{Momentum}_z )$$

_We divide Energy by $c$ (speed of light) so the units match momentum._

Let's translate the symbols in your solution's text:

#### A. The Incoming Electron ($p$)

$$p = \left( \frac{E}{c}, \vec{k} \right)$$

-   **What it means:** This is our bullet. It has total energy $E$ (given as $25\text{ GeV}$) and 3D momentum vector $\vec{k}$.
    
-   **Note:** The problem says "neglect electron mass." This means the electron is moving so fast it's basically light. Therefore, its energy comes entirely from its momentum ($E \approx |\vec{k}|c$).
    

#### B. The Target Proton ($P$)

$$P = (Mc, 0, 0, 0)$$

-   **What it means:** This is the sitting duck.
    
-   **Why is momentum 0?** The problem states it is a "resting proton." It isn't moving, so the vector part is $\vec{0}$.
    
-   **Why is Energy $Mc$?** Even when standing still, a particle has energy thanks to Einstein ($E=Mc^2$). If we divide that by $c$ to fit our four-vector format, we get $Mc$. This is the "Rest Mass Energy."
    

#### C. The Outgoing Electron ($p'$)

$$p' = \left( \frac{E'}{c}, \vec{p}' \right)$$

-   **What it means:** This is the electron after the collision.
    
-   **Changes:** Notice the "prime" symbol ($'$). It has a _new_ energy $E'$ (it will be lower, because it gave some energy to the proton) and a _new_ direction/momentum $\vec{p}'$.
    

#### D. The Exchanged Photon ($q$)

$$q = p - p' = \left( \frac{\nu}{c}, \vec{q} \right)$$

-   **What it means:** This is the most important variable in scattering physics! This vector represents the **difference** between what came in and what went out.
    
-   **Conservation:** Physics demands that momentum is conserved. Whatever momentum the electron _lost_ must be carried by this photon to the proton.
    
    -   Energy transfer: $\nu = E - E'$
        
    -   Momentum transfer: $\vec{q} = \vec{k} - \vec{p}'$
        

#### E. The Outgoing Proton ($P'$)

$$P' = \left( \frac{E'_p}{c}, \vec{P}' \right)$$

-   **What it means:** The proton has been hit.
    
-   **Result:** It now has kinetic energy (so total energy $E'_p > Mc^2$) and it is moving with momentum $\vec{P}'$.
    
-   **Conservation Check:** Just like the electron lost momentum to the photon, the proton gains that exact momentum. So, $P' = P + q$.
    

---

### Summary Table for your Notes

![[Pasted image 20260128142245.png]]

You have now successfully defined the kinematics of the collision!

**Would you like to move on to calculating the actual values (conservation of energy) or do you have questions about these four-vectors first?**