

Hello! This is a fantastic question. The Rutherford-Geiger-Marsden experiment is one of the most important in history. It completely changed our understanding of the atom, moving us from the old "plum pudding" model to the nuclear model we recognize today.

Let's break down your questions step-by-step.

### The Setup: A Quick Picture

First, let's visualize what's happening.

-   **The Bullet:** We are firing **alpha ($\alpha$) particles**. An alpha particle is just a helium nucleus—it contains 2 protons and 2 neutrons. This gives it a positive charge of $+2e$.
    
-   **The Target:** The target is a thin foil of gold. Specifically, we're interested in the gold **nucleus**. The problem gives us $^{197}_{79}\text{Au}$. The important number here is '79', the atomic number ($Z$). This means the gold nucleus has 79 protons, giving it a large positive charge of $+79e$.
    

## The entire experiment is based on the **electrostatic force** (also called the Coulomb force). Since both the alpha particle (our "bullet") and the gold nucleus (our "target") are **positively charged**, they will repel each other.

## (a) The Turning Point and Smallest Distance

### 1. At what scattering angle is the smallest distance?

Imagine the gold nucleus as a very heavy bowling ball, sitting still. The alpha particle is like a small, fast-moving marble. Both are "magnetic" and repel each other.

-   If you roll the marble so it passes _far away_ from the bowling ball, it will be deflected only slightly. This is a **small scattering angle**.
    
-   If you aim the marble to pass _closer_ to the bowling ball, the repulsive force is stronger, and it will be deflected more sharply. This is a **larger scattering angle**.
    
-   Now, what if you aim the marble **directly at the center** of the bowling ball? This is a "head-on collision." The marble will travel straight towards the bowling ball, slowing down as the repulsion gets stronger and stronger. It will momentarily **stop** at some closest distance, and then the repulsion will push it straight back the way it came.
    

This head-on collision is where the two nuclei get the closest they can possibly get. The alpha particle comes in, stops, and is repelled straight back.

**Answer:** The smallest possible distance is achieved in a head-on collision, which corresponds to a **scattering angle of $180^\circ$**.

### 2. What is the kinetic energy at the turning point?

The "turning point" is that exact moment of closest approach we just described. It's the instant the alpha particle **stops** moving forward and is about to start moving backward.

**Kinetic energy** is the energy of motion ($E_{\text{kin}} = \frac{1}{2}mv^2$). If the particle is momentarily at a complete stop, its velocity ($v$) is zero.

**Answer:** At the turning point, the alpha particle's velocity is zero, so its **kinetic energy is $0 \text{ MeV}$**.

---

## (b) Calculating the Smallest Possible Distance ($d_{\text{min}}$)

This part is all about one of the most important concepts in physics: **Conservation of Energy**.

The total energy of the alpha particle is a combination of its kinetic energy (energy of motion) and its potential energy (energy stored by the repulsive force). This total energy cannot be created or destroyed.

$E_{\text{total}} = E_{\text{kinetic}} + E_{\text{potential}}$

Let's look at the energy at two key moments:

1.  **Initial State (Far Away):** The alpha particle is fired from the source, very far from the gold nucleus.
    
    -   **$E_{\text{kinetic}}$:** It has its full initial kinetic energy. The problem states this is $E_{\text{kin}} = 5 \text{ MeV}$.
        
    -   **$E_{\text{potential}}$:** Because it's "very far" away, the repulsive force is essentially zero. We can define its potential energy here as $0$.
        
    -   **Total Energy:** $E_{\text{total}} = 5 \text{ MeV} + 0 = 5 \text{ MeV}$.
        
2.  **Final State (At the Turning Point, $d_{\text{min}}$):** This is the head-on collision at the moment of closest approach.
    
    -   **$E_{\text{kinetic}}$:** As we said in part (a), the particle stops. Its kinetic energy is $0 \text{ MeV}$.
        
    -   **$E_{\text{potential}}$:** All of that initial kinetic energy has been converted into electrostatic potential energy, stored in the repulsive field between the two positive nuclei.
        
    -   **Total Energy:** $E_{\text{total}} = 0 + E_{\text{potential (final)}}$.
        

By the law of conservation of energy, the total energy must be the same in both states:

$E_{\text{Total (Initial)}} = E_{\text{Total (Final)}}$

$E_{\text{kinetic (initial)}} = E_{\text{potential (final)}}$

This gives us our starting equation:

$5 \text{ MeV} = E_{\text{potential (final)}}$

### The Calculation

Now, we just need the formula for electrostatic potential energy ($E_{\text{pot}}$) between two charges ($q_1$ and $q_2$) separated by a distance ($r$):

$$E_{\text{pot}} = k \frac{q_1 q_2}{r}$$

In our problem:

-   $q_1$ is the charge of the alpha particle ($\alpha$) = $+2e$ (where $e$ is the elementary charge)
    
-   $q_2$ is the charge of the gold nucleus ($\text{Au}$) = $+79e$
    
-   $r$ is our smallest possible distance, $d_{\text{min}}$.
    

Let's plug these in:

$E_{\text{kinetic (initial)}} = k \frac{(2e)(79e)}{d_{\text{min}}}$

$E_{\text{kinetic (initial)}} = k \frac{158e^2}{d_{\text{min}}}$

Now we can rearrange the formula to solve for $d_{\text{min}}$:

$d_{\text{min}} = \frac{k \cdot 158e^2}{E_{\text{kinetic (initial)}}}$

We can do this calculation in two ways. I'll show you the "particle physics" way, which is much simpler as it avoids using big SI units like Joules and Coulombs.

We can use a very handy combined constant: $k \cdot e^2 \approx 1.44 \text{ MeV}\cdot\text{fm}$ (Mega-electron-Volt femtometers). A femtometer (fm) is $10^{-15}$ meters.

Let's rewrite our formula slightly differently. The charges are $q_1 = Z_1 e$ and $q_2 = Z_2 e$.

-   $Z_1$ (for alpha) = 2
    
-   $Z_2$ (for gold) = 79
    

$d_{\text{min}} = \frac{k \cdot (Z_1 e) \cdot (Z_2 e)}{E_{\text{kin}}} = \frac{Z_1 Z_2 \cdot (k \cdot e^2)}{E_{\text{kin}}}$

Now, let's plug in our values:

-   $Z_1 Z_2 = (2)(79) = 158$
    
-   $k \cdot e^2 = 1.44 \text{ MeV}\cdot\text{fm}$
    
-   $E_{\text{kin}} = 5 \text{ MeV}$
    

$d_{\text{min}} = \frac{158 \cdot (1.44 \text{ MeV}\cdot\text{fm})}{5 \text{ MeV}}$

Notice how the "MeV" units cancel out, leaving us with "fm," which is a unit of distance. This is exactly what we want!

$d_{\text{min}} = \frac{227.52}{5} \text{ fm}$

**$d_{\text{min}} = 45.5 \text{ fm}$**

(Or, if you prefer standard SI units: $45.5 \times 10^{-15} \text{ m}$, which is $4.55 \times 10^{-14} \text{ m}$).

This calculation was revolutionary! It showed that the "positive stuff" in the atom must be packed into a space _smaller_ than this distance. This was the first real estimate of the size of an atomic nucleus.

I hope that detailed explanation was helpful!

Would you like to discuss what this result _means_ for the atomic model, or perhaps calculate the distance for a different scattering angle?