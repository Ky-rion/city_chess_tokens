

That's a great follow-up question! This problem connects the principles of **classical electromagnetism** (acceleration by a voltage) with **quantum mechanics** (the de Broglie wavelength). We'll need to use relativistic mechanics because the electron is accelerated to a very high energy.

The question asks for the **de Broglie wavelength ($\lambda$)** of an electron accelerated from rest by a potential difference of $2\text{ MV}$ (megavolts).

$$\lambda = \frac{h}{p}$$

---

## 1. Electron Energy and Relativistic Kinematics

The potential difference ($\Delta V$) accelerates the electron, converting potential energy into kinetic energy.

### A. Total Energy

When an electron (with charge $e$) is accelerated by a potential difference $\Delta V$, its gain in kinetic energy ($\Delta K$) is:

$$\Delta K = e \Delta V$$

Given the potential difference is $2\text{ MV}$, the kinetic energy is:

$$K = e \cdot (2\text{ MV}) = 2\text{ MeV}$$

(Since $1\text{ electron volt (eV)}$ is the energy gained by an electron moving through $1\text{ volt}$).

Now we must consider the electron's total energy ($E$). The total energy is the sum of its rest energy ($E_0$) and its kinetic energy ($K$):

$$E = E_0 + K$$

The rest energy of an electron ($m_e c^2$) is a fundamental constant we need:

$$E_0 = m_e c^2 \approx 0.511 \text{ MeV}$$

The electron's total energy is:

$$E = 0.511 \text{ MeV} + 2 \text{ MeV} = \mathbf{2.511 \text{ MeV}}$$

Since the kinetic energy ($2\text{ MeV}$) is significantly larger than the rest energy ($0.511\text{ MeV}$), this electron is **highly relativistic** ($K > E_0$). Therefore, we must use the **relativistic energy-momentum relation**.

---

## 2. Relativistic Momentum

The fundamental relativistic relationship connecting total energy ($E$), momentum ($p$), and rest energy ($E_0$) is:

$$E^2 = (pc)^2 + E_0^2$$

We need to solve for the momentum ($p$):

$$(pc)^2 = E^2 - E_0^2$$

$$p = \frac{\sqrt{E^2 - E_0^2}}{c}$$

Plugging in the energy values:

$$E = 2.511 \text{ MeV}$$

$$E_0 = 0.511 \text{ MeV}$$

$$pc = \sqrt{(2.511 \text{ MeV})^2 - (0.511 \text{ MeV})^2}$$

$$pc = \sqrt{6.305 \text{ MeV}^2 - 0.261 \text{ MeV}^2}$$

$$pc = \sqrt{6.044 \text{ MeV}^2}$$

$$pc \approx \mathbf{2.458 \text{ MeV}}$$

The momentum is $p = 2.458 \text{ MeV}/c$. This is the convenient unit for momentum in particle physics.

---

## 3. Calculating the de Broglie Wavelength

The de Broglie wavelength formula is $\lambda = h/p$. Since we used the reduced Planck constant ($\hbar = h/2\pi$) in the previous problem, it's often simpler to use:

$$\lambda = \frac{2\pi\hbar}{p}$$

We can re-write this to use the unit-friendly term $\hbar c$ and the momentum term $pc$:

$$\lambda = \frac{2\pi (\hbar c)}{(pc)}$$

From Part (a), we know the value of $\hbar c$ in the particle physics units ($\text{MeV}\cdot\text{fm}$):

$$\hbar c \approx 197.327 \text{ MeV}\cdot\text{fm}$$

Plugging in the values for $\hbar c$ and $pc$:

$$\lambda = \frac{2\pi \cdot (197.327 \text{ MeV}\cdot\text{fm})}{2.458 \text{ MeV}}$$

The $\text{MeV}$ units cancel out, leaving the length unit $\text{fm}$ (femtometers).

$$\lambda = \frac{1240.06 \text{ fm}}{2.458}$$

$$\lambda \approx \mathbf{504.5 \text{ fm}}$$

---

## Conclusion and Context

The de Broglie wavelength of an electron accelerated by a $2\text{ MV}$ potential difference is approximately **$504.5 \text{ fm}$**.

$$(\text{b) The de Broglie Wavelength: } \lambda \approx 504.5 \text{ fm})$$

### Physical Context

1.  **High Energy, Short Wavelength:** The electron's kinetic energy ($2\text{ MeV}$) is quite high, giving it a high momentum. In quantum mechanics, high momentum means a short wavelength.
    
2.  **Size Scale:** A femtometer ($\text{fm}$) is $10^{-15} \text{ m}$. The calculated wavelength ($504.5\text{ fm}$) is about **500 times the diameter of a proton** ($\approx 1.75\text{ fm}$) or a neutron. This high-energy electron, with its relatively short wavelength, is an excellent probe for studying the structure of atomic nuclei and protons/neutrons.