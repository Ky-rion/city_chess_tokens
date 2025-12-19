

Hello! It is wonderful to meet you. I would be absolutely delighted to be your guide through this problem. Particle physics is a fascinating field because it allows us to understand how the smallest building blocks of the universe interact with the matter we see around us every day.

This problem is a classic "passage of particles through matter" exercise. It asks us to calculate how much energy a cosmic muon loses when it crashes through a plate of iron. To solve this, we will use one of the most famous equations in experimental particle physics: the **Bethe-Bloch formula**.

Here is the step-by-step breakdown.

### Part 1: The Calculation

#### 1. The Physics Tool: The Bethe-Bloch Formula

The energy loss per unit distance (stopping power) for a heavy charged particle (like a muon) is given by:

$$-\left\langle \frac{dE}{dx} \right\rangle = K z^2 \frac{Z}{A} \frac{1}{\beta^2} \left[ \frac{1}{2} \ln \left( \frac{2 m_e c^2 \beta^2 \gamma^2 T_{\text{max}}}{I^2} \right) - \beta^2 \right]$$

Don't let the scary symbols intimidate you! We will break them down one by one.

**The Variables from your problem:**

-   **Target Material:** Iron (Fe)
    
    -   $Z = 26$ (Atomic number, number of protons)
        
    -   $A = 55.85$ g/mol (Molar mass)
        
    -   $\rho = 7.874$ g/cm$^3$ (Density)
        
    -   $x = 5$ cm (Thickness of the plate)
        
-   **The Particle:** Cosmic Muon ($\mu$)
    
    -   $E = 3$ GeV (Total Energy)
        
    -   $z = 1$ (Charge of a muon, same as an electron)
        
-   **Constants:**
    
    -   $K \approx 0.307$ MeV mol$^{-1}$ cm$^2$ (Standard constant in this formula)
        
    -   $m_e c^2 = 0.511$ MeV (Rest mass energy of an electron)
        
    -   $m_\mu c^2 = 105.7$ MeV (Rest mass energy of a muon)
        
    -   $I \approx Z \cdot 10 \text{ eV} = 260 \text{ eV} = 2.6 \times 10^{-4}$ MeV (Mean excitation potential, using the hint provided).
        

#### 2. The Kinematics (Getting $\beta$ and $\gamma$)

First, we need to know how fast the muon is going. In particle physics, we describe speed using $\beta$ (fraction of light speed) and $\gamma$ (Lorentz factor).

We know the total energy $E = 3$ GeV $= 3000$ MeV.

The rest mass $m_\mu = 105.7$ MeV.

$$\gamma = \frac{E}{m_\mu c^2} = \frac{3000}{105.7} \approx 28.38$$

Now we find $\beta$:

$$\beta = \sqrt{1 - \frac{1}{\gamma^2}} = \sqrt{1 - \frac{1}{(28.38)^2}} \approx 0.9994$$

_Professor's Note:_ As you can see, this muon is relativistic (traveling at $99.94\%$ the speed of light)!

#### 3. Calculating $T_{\text{max}}$

$T_{\text{max}}$ is the maximum kinetic energy the muon can transfer to a free electron in a single collision.

$$T_{\text{max}} \approx 2 m_e c^2 \beta^2 \gamma^2$$

(Note: There is a more precise formula, but for $\gamma \approx 28$, this approximation is excellent).

$$T_{\text{max}} = 2 \cdot (0.511 \text{ MeV}) \cdot (0.9994)^2 \cdot (28.38)^2$$

$$T_{\text{max}} \approx 1.022 \cdot 1 \cdot 805.4 \approx 823 \text{ MeV}$$

#### 4. Putting it all together

Now, we plug our numbers into the Bethe-Bloch formula.

A. The Pre-factor ($K z^2 \frac{Z}{A} \frac{1}{\beta^2}$):

$$\text{Prefactor} = 0.307 \cdot (1)^2 \cdot \frac{26}{55.85} \cdot \frac{1}{(0.9994)^2}$$

$$\text{Prefactor} \approx 0.307 \cdot 0.4655 \cdot 1.001$$

$$\text{Prefactor} \approx 0.143 \text{ MeV cm}^2/\text{g}$$

B. The Logarithmic Term (The Bracket):

$$\text{Bracket} = \frac{1}{2} \ln \left( \frac{2 m_e c^2 \beta^2 \gamma^2 T_{\text{max}}}{I^2} \right) - \beta^2$$

Let's simplify the inside of the natural log ($\ln$):

Numerator $= (2 m_e c^2 \beta^2 \gamma^2) \cdot T_{\text{max}} = (823 \text{ MeV}) \cdot (823 \text{ MeV})$.

Wait, looking closely at the standard formula forms, sometimes the numerator is written as $2 m_e c^2 \beta^2 \gamma^2 T_{max}$. Let's calculate that ratio:

$$\text{Ratio} = \frac{823 \text{ MeV} \cdot 823 \text{ MeV}}{(2.6 \times 10^{-4} \text{ MeV})^2}$$

$$\text{Ratio} \approx \frac{677329}{6.76 \times 10^{-8}} \approx 1.0 \times 10^{13}$$

Now take the natural log:

$$\ln(1.0 \times 10^{13}) \approx 29.93$$

Now compute the full bracket:

$$\text{Bracket} = \frac{1}{2}(29.93) - (0.9994)^2$$

$$\text{Bracket} \approx 14.96 - 1 \approx 13.96$$

C. Calculate Stopping Power ($-\frac{dE}{dx}$):

$$-\frac{dE}{dx} = (\text{Prefactor}) \times (\text{Bracket})$$

$$-\frac{dE}{dx} = 0.143 \times 13.96 \approx 2.0 \text{ MeV} \cdot \text{cm}^2/\text{g}$$

_Professor's Check:_ This is a very reassuring number! For most materials and relativistic particles, the energy loss is roughly **1.5 to 2 MeV cm$^2$/g**. Being close to 2 tells us we are on the right track.

#### 5. Total Energy Loss

The formula gave us the "mass stopping power" (energy loss per density-distance). To get the linear energy loss per centimeter, we multiply by the density $\rho$.

$$\frac{dE}{dx}_{\text{linear}} = 2.0 \frac{\text{MeV cm}^2}{\text{g}} \times 7.874 \frac{\text{g}}{\text{cm}^3} \approx 15.75 \text{ MeV/cm}$$

Finally, multiply by the thickness of the iron ($x = 5$ cm):

$$\Delta E \approx 15.75 \text{ MeV/cm} \times 5 \text{ cm} \approx 78.75 \text{ MeV}$$

**Answer for Part 1:** The muon loses approximately **79 MeV** of energy.

---

### Part 2: The Conceptual Question

**Question:** _"Why can you consider the energy loss as a constant instead of integrating it over the distance covered by the muon?"_

Explanation:

To calculate energy loss strictly accurately, you would normally have to integrate because as the particle travels, it loses energy ($E$ decreases). As $E$ decreases, its velocity ($\beta$) and Lorentz factor ($\gamma$) change. Since the Bethe-Bloch formula depends on $\beta$ and $\gamma$, the rate of energy loss $dE/dx$ should change as the particle goes deeper into the iron.

**However, we can assume it is constant here because:**

1.  The loss is tiny compared to the total:
    
    The muon started with $3000$ MeV ($3$ GeV).
    
    It lost roughly $79$ MeV.
    
    $$\text{Percentage Loss} = \frac{79}{3000} \approx 2.6\%$$
    
    Since the muon retains $>97\%$ of its energy, its velocity $\beta$ hardly changes at all. It stays extremely close to the speed of light.
    
2.  The "MIP" Plateau:
    
    At energies around 3 GeV, muons are what we call Minimum Ionizing Particles (MIPs). In this energy range, the curve of energy loss vs. energy is very flat (it's a broad minimum). Even if the energy changed a little bit, the $dE/dx$ value stays almost exactly the same.
    

Because the velocity doesn't change significantly, and the stopping power function is flat in this region, treating $dE/dx$ as a constant is a perfectly safe approximation!

---

Professor's Next Step:

Would you like me to show you a graph of the Bethe-Bloch curve so you can visually see where this "Minimum Ionizing" region sits compared to lower energies?