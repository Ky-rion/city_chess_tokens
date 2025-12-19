

Great! Let's tackle part (b). This is a classic calculation in nuclear physics. We need to find two energies and explain _why_ we're allowed to use the "easy" formulas.

Here's the detailed breakdown.

---

### 1. 🎯 Determining the $\beta$ Limit Energy ($E_0$)

First, what is the "$\beta$ limit energy," or **endpoint energy ($E_0$)**?

In our decay, $³\text{H} \rightarrow ³\text{He} + e^- + \bar{\nu}_e$, the total energy released (the Q-value we found in part (a)) is shared between the kinetic energies of the three products:

$$Q = K_{³\text{He}} + K_{e^-} + K_{\bar{\nu}_e}$$

From our previous work (and the problem's solution), we know this total energy is $Q \approx 18.6 \text{ keV}$ (or $0.0186 \text{ MeV}$).

The electron ($e^-$) will have its **maximum possible kinetic energy** (which we call $E_0$) in the specific scenario where the _other_ two particles get the _minimum_ possible energy.

-   The problem tells us to assume the neutrino is massless ($m_\nu = 0$). A massless particle _can_ be created with zero energy (and zero momentum).
    
-   So, to get the maximum $K_{e^-}$, we assume the antineutrino carries away (almost) **zero energy**: $K_{\bar{\nu}_e} \approx 0$.
    

This simplifies our energy equation to:

$$Q \approx K_{³\text{He}} + K_{e^- (\text{max})}$$

$$Q \approx K_{³\text{He}} + E_0$$

This is now a two-body problem. The total energy $Q$ is split between the helium-3 nucleus and the electron. Because they must fly off in opposite directions to conserve momentum, the heavy $³\text{He}$ nucleus will get a _tiny_ fraction of the energy, and the light electron will get _almost all_ of it.

Just how tiny? The recoil energy of the nucleus is _so_ small (as we'll see in a moment) that it's negligible _compared to the 18.6 keV_.

Therefore, to an excellent approximation:

$E_0 \approx Q$

$E_0 = 18.6 \text{ keV}$

The $\beta$ limit energy is simply the total decay energy, $Q$.

---

### 2. 💥 Determining the Maximum Recoil Energy of $³\text{He}$

This part is a little subtle. The question gives $3.4 \text{ eV}$ as the solution, which isn't the _absolute_ maximum possible recoil (that happens when the _electron_ gets zero energy). The $3.4 \text{ eV}$ value is the **recoil energy of the $³\text{He}$ nucleus _at the $\beta$ limit_**—that is, _in the exact same scenario_ we just used to find $E_0$.

Let's calculate that specific recoil.

-   **Setup:** We have $Q = 18.6 \text{ keV}$ being split between the $³\text{He}$ and the $e^-$. The antineutrino is gone.
    
-   Conservation of Momentum: The initial momentum is zero. The final momenta must be equal and opposite:
    
    $$p_{³\text{He}} = p_{e^-} = p$$
    
-   Conservation of Energy: We use the non-relativistic formula for kinetic energy, $K = p^2 / (2m)$ (we'll justify this in part 3).
    
    $$Q = K_{³\text{He}} + K_{e^-}$$
    
    $$Q = \frac{p^2}{2m_{³\text{He}}} + \frac{p^2}{2m_{e^-}}$$
    

We want to find $K_{³\text{He}} = p^2 / (2m_{³\text{He}})$. The easiest way is to find a ratio. Let's look at the kinetic energies:

$$K_{³\text{He}} = \frac{p^2}{2m_{³\text{He}}}$$

$$K_{e^-} = \frac{p^2}{2m_{e^-}}$$

If we divide the first equation by the second, we get:

$$\frac{K_{³\text{He}} }{ K_{e^-} } = \frac{p^2 / (2m_{³\text{He}}) }{ p^2 / (2m_{e^-}) } = \frac{m_{e^-}}{m_{³\text{He}}}$$

This gives us a powerful, simple relationship:

$K_{³\text{He}} = K_{e^-} \cdot \left( \frac{m_{e^-}}{m_{³\text{He}}} \right)$

Now we can plug in the numbers!

-   $K_{e^-} \approx E_0 = 18.6 \text{ keV}$
    
-   $m_{e^-} c^2$ (rest mass of electron) $\approx 0.511 \text{ MeV}$
    
-   $m_{³\text{He}} c^2$ (rest mass of He-3) $\approx 2809 \text{ MeV}$ (approx. 2 protons + 1 neutron)
    

Let's run the calculation:

$K_{³\text{He}} \approx (18.6 \text{ keV}) \cdot \left( \frac{0.511 \text{ MeV}}{2809 \text{ MeV}} \right)$

$K_{³\text{He}} \approx (18.6 \text{ keV}) \cdot (0.0001819)$

$K_{³\text{He}} \approx 0.00338 \text{ keV}$

To make this number easier to read, let's convert from keV (kilo-electron-volts) to eV (electron-volts):

$0.00338 \text{ keV} \times 1000 \text{ eV/keV} = \textbf{3.38 eV}$

This rounds perfectly to the solution's **$3.4 \text{ eV}$**.

---

### 3. 🤔 Why Can We Use a Non-Relativistic Calculation?

This is a critical "check-your-assumptions" question. We used $K = p^2 / (2m)$, but the "correct" formula is the relativistic $K = \sqrt{(pc)^2 + (mc^2)^2} - mc^2$. Why was our simple version okay?

**The short answer: All the kinetic energies involved are _much, much smaller_ than the rest mass energies of the particles.**

Let's check each particle:

-   **Helium-3 Nucleus ($³\text{He}$):**
    
    -   **Kinetic Energy:** $K_{³\text{He}} \approx 3.4 \text{ eV}$
        
    -   **Rest Mass Energy:** $m_{³\text{He}} c^2 \approx 2809 \text{ MeV} = \textbf{2,809,000,000 eV}$
        
    -   **Comparison:** $3.4 \text{ eV}$ is _fantastically_ smaller than $2.8 \text{ billion eV}$. The nucleus is barely moving. Using a non-relativistic formula here is beyond safe; it's perfect.
        
-   **Electron ($e^-$):**
    
    -   **Kinetic Energy:** $K_{e^-} \approx 18.6 \text{ keV} = \textbf{18,600 eV}$
        
    -   **Rest Mass Energy:** $m_{e^-} c^2 = 0.511 \text{ MeV} = \textbf{511,000 eV}$
        
    -   **Comparison:** The electron's kinetic energy ($18.6 \text{ keV}$) is only about **3.6%** of its rest mass energy ($511 \text{ keV}$).
        

Because the kinetic energy is so small compared to the rest mass for _all_ the particles (even the "fast" electron), the system is firmly in the non-relativistic (or "classical") regime. Our approximation of $K = p^2 / (2m)$ is excellent and produces a highly accurate answer, as we've seen.

This is a great example of how conservation of energy and momentum work together to distribute the "winnings" from a nuclear decay.

Are you ready to look at the final part of this problem?