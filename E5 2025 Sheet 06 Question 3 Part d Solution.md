

![[Pasted image 20260128120049.png]]
![[Pasted image 20260128120107.png]]
![[Pasted image 20260128120120.png]]

This part of our journey takes us from the theoretical limits of physics to the practical realities of the laboratory. We are going to look at the **ZEUS detector**, which lived at HERA, and figure out what it could actually "see" based on its physical design.

In experimental physics, we are limited by our hardware. A detector is like a camera lens: it can only see within a certain field of view (angles) and above a certain brightness (energy).

---

### 1. Finding the $Q^2$ Range

To find the range of $Q^2$ (the "momentum transfer squared") that the ZEUS detector can measure, we use the formula we've been working with:

$$Q^2 \approx \frac{2 E_e E'_e}{c^2} (1 - \cos \theta)$$

Where $E_e$ is our starting electron energy (**27.6 GeV** from the first part of the problem). The detector has two main constraints:

-   **Energy Threshold:** It can only detect electrons with an energy $E'_e \geq 5 \text{ GeV}$.
    
-   **Angular Coverage:** It only "sees" between $\theta = 7^\circ$ and $\theta = 178^\circ$.
    

#### The Minimum $Q^2$ ($Q^2_{\text{min}}$)

To get the smallest possible $Q^2$, we need the smallest energy and the smallest angle:

-   Plug in $E'_e = 5 \text{ GeV}$ and $\theta = 7^\circ$.
    
-   $Q^2_{\text{min}} \approx \frac{2 \cdot 27.6 \cdot 5}{1} (1 - \cos 7^\circ) \approx \mathbf{2.1 \text{ (GeV/c)}^2}$.
    

#### The Maximum $Q^2$ ($Q^2_{\text{max}}$)

To reach the highest $Q^2$, we need the highest possible energy ($E'_e$ can theoretically reach the proton beam energy of **920 GeV** in a total recoil) and the widest angle ($178^\circ$):

-   $Q^2_{\text{max}} \approx \frac{2 \cdot 27.6 \cdot 920}{1} (1 - \cos 178^\circ) \approx \mathbf{10^5 \text{ (GeV/c)}^2}$.
    

---

### 2. The Bjorken Scaling Variable ($x$)

Now for the "Extra Task." We need to find the range of $x$. In particle physics, $x$ represents the **fraction of the proton's momentum** carried by the quark that got hit. It ranges from $0$ to $1$.

Using the conservation of four-momentum (the messy looking matrices in your solution image), your professor derived a formula for $x$ in the laboratory frame:

$$x = \frac{E_e E'_e (1 - \cos \theta)}{2 E_p E_e - E_p E'_e (1 + \cos \theta)}$$

#### The $x$ Range

-   **$x_{\text{min}}$:** By plugging in the minimum detection values ($E'_e = 5 \text{ GeV}$, $\theta = 7^\circ$), we find that ZEUS can probe quarks carrying as little as **$0.0025\%$** of the proton's momentum ($x \approx 2.5 \cdot 10^{-5}$).
    
-   **$x_{\text{max}}$:** At the other extreme ($E'_e = 920 \text{ GeV}$, $\theta = 178^\circ$), $x$ approaches **$1$**, meaning we are hitting a quark that carries essentially the entire momentum of the proton.
    

---

### Professor's Summary: Why does this matter?

The last image you provided (the plot with many black triangles) is one of the most famous plots in history! It shows the **Proton Structure Function** ($F_2$).

-   **Fixed-target experiments** (the little circles and squares at the bottom right) could only see high $x$ and low $Q^2$.
    
-   **HERA** (the triangles) blew the doors open by reaching tiny values of $x$ and huge values of $Q^2$.
    

This revealed that when you look really closely at a proton (high $Q^2$), it isn't just three quarks; it's a "sea" of thousands of gluons and transient quarks constantly popping in and out of existence.

**We've covered a lot of ground! Is there any specific part of that $x$ derivation or the structure function plot you'd like to dive deeper into?**