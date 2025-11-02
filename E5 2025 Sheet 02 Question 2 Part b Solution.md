

Ah, an excellent follow-up! This is the practical application of the beautiful formula we just derived.

Let's get right to it.

### 1. The Strategy: Connecting (a) and (b)

In part (a), we proved a crucial relationship:

> The total cross section ($\sigma$) for all scattering events with an impact parameter **$b < b_0$** is given by **$\sigma = \pi b_0^2$**.

We _also_ know that the impact parameter $b$ and the scattering angle $\theta$ are **inversely related**.

-   A head-on collision ($b=0$) gives the maximum scattering angle ($\theta = 180^\circ$).
    
-   A distant miss ($b \to \infty$) gives no scattering ($\theta = 0^\circ$).
    

This means that the condition "all scattering angles **larger than $\theta_0$**" is _exactly the same_ as the condition "all impact parameters **smaller than $b_0$**," where $b_0$ is the specific impact parameter that causes a $_0$ scatter.

Therefore, to solve this problem, we don't need to do that complicated integral again! We just need to:

1.  Use the formula we derived: $\sigma = \pi b_0^2$
    
2.  Find the value for $b_0$ that corresponds to our given angles ($\theta_0 = 10^\circ$ and $\theta_0 = 20^\circ$).
    
3.  The formula connecting them, which we used in our derivation, is:
    
    $$b_0 = \frac{k}{2E} \cot(\theta_0/2)$$
    

Combining these, the formula we need to calculate is:

$$\sigma = \pi \left( \frac{k}{2E} \cot(\theta_0/2) \right)^2$$

---

### 2. The "Setup": Calculating Our Constants

First, let's find the value of all the constants in that equation.

-   **$E$ (Energy):** Given as $E = 10 \text{ MeV}$.
    
-   **$k$ (The "Charge Constant"):** We defined this in the last problem. It's $k = \frac{Z_1 Z_2 e^2}{4\pi\epsilon_0}$.
    
    -   $Z_1$ is the charge of the $\alpha$ particle = **2**
        
    -   $Z_2$ is the charge of the gold nucleus = **79**
        
    -   $\frac{e^2}{4\pi\epsilon_0}$ is a fundamental constant. In particle physics, we almost never plug in all those SI units. We use a very handy "magic number":
        
        $$\frac{e^2}{4\pi\epsilon_0} = \alpha \hbar c \approx 1.44 \text{ MeV fm}$$
        
        (where $\alpha$ is the fine-structure constant, $\hbar$ is the reduced Planck constant, and $c$ is the speed of light. The product is $1.44$ Mega-electron-Volts times femtometers).
        

Now, let's calculate $k$:

$$k = Z_1 Z_2 \cdot (1.44 \text{ MeV fm})$$

$$k = (2)(79) \cdot (1.44 \text{ MeV fm})$$

$$k = 158 \cdot (1.44 \text{ MeV fm}) \approx \textbf{227.5 MeV fm}$$

Next, let's find the constant part of our $b_0$ equation, $\frac{k}{2E}$:

$$\frac{k}{2E} = \frac{227.5 \text{ MeV fm}}{2 \cdot 10 \text{ MeV}}$$

$$\frac{k}{2E} = \frac{227.5 \text{ MeV fm}}{20 \text{ MeV}} = \textbf{11.375 fm}$$

This is great! All the complicated physics has been boiled down to one number. Our formula is now simple:

$$\sigma = \pi \left( 11.375 \text{ fm} \cdot \cot(\theta_0/2) \right)^2$$

---

### 3. Case 1: Scattering angles larger than $10^\circ$

Here, our minimum angle is $\theta_0 = 10^\circ$.

1.  Find the half-angle:
    
    $\theta_0/2 = 5^\circ$
    
2.  Find the cotangent:
    
    $\cot(5^\circ) \approx 11.430$
    
3.  Plug into our formula:
    
    $$\sigma = \pi \left( 11.375 \text{ fm} \cdot 11.430 \right)^2$$
    
    $$\sigma = \pi \left( 130.0 \text{ fm} \right)^2$$
    
    $$\sigma = \pi \cdot (16900 \text{ fm}^2)$$
    
    $$\sigma \approx 53093 \text{ fm}^2$$
    

This is a valid answer, but in nuclear physics, we use a special unit for area called the **barn (b)**. It's defined as:

> $1 \text{ barn} = 10^{-28} \text{ m}^2$
> 
> A handy conversion is: $\mathbf{1 \text{ barn} = 100 \text{ fm}^2}$

So, to convert our answer to barns, we divide by 100:

$$\sigma = \frac{53093 \text{ fm}^2}{100 \text{ fm}^2 / \text{b}} \approx \textbf{531 barns}$$

---

### 4. Case 2: Scattering angles larger than $20^\circ$

Now, our minimum angle is $\theta_0 = 20^\circ$.

1.  Find the half-angle:
    
    $\theta_0/2 = 10^\circ$
    
2.  Find the cotangent:
    
    $\cot(10^\circ) \approx 5.671$
    
3.  Plug into our formula:
    
    $$\sigma = \pi \left( 11.375 \text{ fm} \cdot 5.671 \right)^2$$
    
    $$\sigma = \pi \left( 64.51 \text{ fm} \right)^2$$
    
    $$\sigma = \pi \cdot (4161.5 \text{ fm}^2)$$
    
    $$\sigma \approx 13074 \text{ fm}^2$$
    
4.  Convert to barns:
    
    $$\sigma = \frac{13074 \text{ fm}^2}{100 \text{ fm}^2 / \text{b}} \approx \textbf{131 barns}$$
    

---

### 5. Final Results and Interpretation

Let's look at our two results:

-   Cross section for $\theta > 10^\circ$: **$\sigma \approx 531 \text{ b}$**
    
-   Cross section for $\theta > 20^\circ$: **$\sigma \approx 131 \text{ b}$**
    

Notice that the cross section for scattering at angles _larger than 10 degrees_ is about 4 times bigger than for scattering at angles _larger than 20 degrees_.

This teaches us a fundamental lesson from the Rutherford experiment:

The vast majority of scattering events happen at very small angles.

By excluding just the first 10 degrees of scattering, we lose a huge part of the total cross section. This is because the $\cot(\theta/2)$ term in the formula squared gets enormous as $\theta$ approaches zero.

This is precisely what Rutherford observed: most $\alpha$ particles went through with only tiny deflections, while only a very few scattered at large angles.

Does this step-by-step calculation and the physical interpretation make sense?