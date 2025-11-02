

This is an excellent problem that highlights the extreme relativistic nature of particles in modern accelerators like the Large Hadron Collider (LHC) and demonstrates the necessity of using approximations (like the Taylor expansion) for calculations involving such high precision.

The goal is to find the **speed difference ($\Delta v$)** between an LHC proton (moving at velocity $v$) and a beam of light (moving at $c$), and express this difference in $\text{km/h}$.

$$\Delta v = c - v$$

---

## 1. Relativistic Velocity and Energy

The relationship between a particle's total energy ($E$) and its velocity ($v$) in special relativity is:

$$E = \frac{E_0}{\sqrt{1 - (v/c)^2}} = \gamma E_0$$

where $E_0$ is the rest energy and $\gamma$ is the Lorentz factor.

From this, we can solve for the velocity $v$:

$$\frac{E_0}{E} = \sqrt{1 - (v/c)^2}$$

$$\left(\frac{E_0}{E}\right)^2 = 1 - \frac{v^2}{c^2}$$

$$\frac{v^2}{c^2} = 1 - \left(\frac{E_0}{E}\right)^2$$

$$v = c \sqrt{1 - \left(\frac{E_0}{E}\right)^2}$$

The difference we want is $\Delta v = c - v$:

$$\Delta v = c - c \sqrt{1 - \left(\frac{E_0}{E}\right)^2} = c \left(1 - \sqrt{1 - \left(\frac{E_0}{E}\right)^2}\right)$$

---

## 2. Setting Up the Calculation

We need the proton's rest energy ($E_0$) and its total energy ($E$).

-   Proton Total Energy ($E$): $6.5 \text{ TeV}$
    
    $$E = 6.5 \times 10^{12} \text{ eV} = 6500 \text{ GeV}$$
    
-   Proton Rest Energy ($E_0$): This is a known fundamental constant.
    
    $$E_0 = m_p c^2 \approx 938.272 \text{ MeV} \approx 0.938 \text{ GeV}$$
    

The ratio of rest energy to total energy, which we'll call $\epsilon$, is extremely small:

$$\epsilon = \frac{E_0}{E} = \frac{0.938 \text{ GeV}}{6500 \text{ GeV}} \approx 1.443 \times 10^{-4}$$

Since $\epsilon$ is very small, $\epsilon^2$ is even smaller:

$$\epsilon^2 \approx (1.443 \times 10^{-4})^2 \approx 2.083 \times 10^{-8}$$

---

## 3. Applying the Taylor Expansion

The term inside the square root in our $\Delta v$ equation is $1 - \epsilon^2$. The direct calculation of $v$ from $v = c \sqrt{1 - \epsilon^2}$ would require retaining many significant digits to find the tiny difference $c-v$, which is prone to numerical error (known as "catastrophic cancellation").

We'll use the binomial approximation (Taylor expansion) for the square root:

$$\sqrt{1 - x} \approx 1 - \frac{1}{2}x - \frac{1}{8}x^2 - \dots \quad \text{for } |x| \ll 1$$

In our case, $x = \epsilon^2 = (E_0/E)^2$. Since $\epsilon^2 \approx 2 \times 10^{-8}$ is very small, we can safely stop at the first-order term ($x/2$):

$$\sqrt{1 - \epsilon^2} \approx 1 - \frac{1}{2}\epsilon^2$$

Now substitute this approximation back into the $\Delta v$ equation:

$$\Delta v = c \left(1 - \sqrt{1 - \epsilon^2}\right)$$

$$\Delta v \approx c \left(1 - \left(1 - \frac{1}{2}\epsilon^2\right)\right)$$

$$\Delta v \approx c \left(1 - 1 + \frac{1}{2}\epsilon^2\right)$$

$$\Delta v \approx \frac{1}{2} c \epsilon^2 = \frac{1}{2} c \left(\frac{E_0}{E}\right)^2$$

This approximated formula gives a much more stable and accurate result for the small speed difference.

---

## 4. Final Calculation and Unit Conversion

### A. Calculate $\Delta v$

$$c \approx 299,792,458 \text{ m/s}$$

$$\epsilon^2 \approx 2.083 \times 10^{-8}$$

$$\Delta v \approx \frac{1}{2} c \epsilon^2 = \frac{1}{2} (299,792,458 \text{ m/s}) (2.083 \times 10^{-8})$$

$$\Delta v \approx 0.5 \times 299,792,458 \times 2.083 \times 10^{-8} \text{ m/s}$$

$$\Delta v \approx 3.123 \text{ m/s}$$

The protons are $3.123 \text{ m/s}$ slower than light.

### B. Unit Conversion to $\text{km/h}$

The final answer must be in $\text{km/h}$. We use the conversion factor:

$$1 \text{ m/s} = \frac{1 \text{ m}}{1 \text{ s}} \times \frac{1 \text{ km}}{1000 \text{ m}} \times \frac{3600 \text{ s}}{1 \text{ h}} = 3.6 \text{ km/h}$$

$$\Delta v (\text{km/h}) = \Delta v (\text{m/s}) \times 3.6$$

$$\Delta v \approx 3.123 \text{ m/s} \times 3.6 \frac{\text{km/h}}{\text{m/s}}$$

$$\Delta v \approx 11.24 \text{ km/h}$$

The LHC protons, accelerated to $6.5 \text{ TeV}$, are slower than a beam of light by about **$11.24 \text{ km/h}$**.

$$\text{Speed difference: } \mathbf{\Delta v \approx 11.24 \text{ km/h}}$$

This tiny speed difference, compared to the speed of light ($\approx 1.08$ billion $\text{km/h}$), illustrates just how close these protons are to the cosmic speed limit.