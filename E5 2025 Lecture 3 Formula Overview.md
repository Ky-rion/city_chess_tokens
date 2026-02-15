

Welcome to the world of nuclear and particle physics! It is a pleasure to have you in the "lecture hall." These formulas are the bread and butter of **radioactive decay**. They describe how unstable particles or nuclei transform over time.

Think of this like a huge popcorn machine: you never know exactly when a single kernel will pop, but you can predict very accurately how much popcorn you’ll have after one minute.

Let's break these down section by section.

---

## 1. The Radioactive Decay Law

$$N(t) = N_0 e^{-\lambda t}$$

This is the "Golden Rule" of decay. It tells you how many radioactive particles are left at any given time.

- **$N(t)$:** The number of particles remaining at time $t$.
    
- **$N_0$:** The initial number of particles you started with (at $t=0$).
    
- **$e$:** Euler's number (approx. 2.718), which appears in processes involving continuous growth or decay.
    
- **$\lambda$ (Lambda):** The **decay constant**. It represents the probability that a single particle will decay per unit of time.
    

**Use Case:** If you are a doctor using a radioactive tracer for an MRI, you use this to calculate how much of that substance is still active in the patient’s body after several hours.

---

## 2. Mean Lifetime ($\tau$) and Half-Life ($t_{1/2}$)

$$\tau = \frac{1}{\lambda} \quad \text{and} \quad t_{1/2} = \frac{\ln 2}{\lambda} = \tau \ln 2$$

These two formulas give us a "human-readable" sense of time.

- **$\tau$ (Tau):** The **mean lifetime**. This is the average time a particle survives before it decays.
    
- **$t_{1/2}$:** The **half-life**. This is the time it takes for exactly **half** of your sample to disappear.
    

**Note:** $\ln 2$ is approximately **0.693**. So, the half-life is always about 70% of the mean lifetime.

---

## 3. Total Decay Constant

$$\lambda = \sum_{k=1}^n \lambda_k$$

Sometimes, a particle is "indecisive" and can decay in several different ways (e.g., it could emit an alpha particle OR a beta particle).

- **$\lambda_k$:** The decay constant for one specific "branch" or pathway.
    
- **$\lambda$:** The total decay constant is just the sum of all individual probabilities.
    

**Use Case:** In high-energy physics, we use this to calculate the "Branching Ratio"—basically, the odds of a Higgs Boson turning into photons versus other particles.

---

## 4. Activity ($A$)

$$A = -\frac{dN}{dt} = \lambda N = \lambda \frac{m \cdot N_A}{M}$$

"Aktivität" is the German word for **Activity**. This is the "speed" of the decay—how many "pops" per second you hear on a Geiger counter.

- **$A$:** Measured in **Becquerels (Bq)** (1 Bq = 1 decay per second).
    
- **$m$:** The mass of the sample.
    
- **$N_A$:** Avogadro's constant ($6.022 \times 10^{23}$), which tells us how many atoms are in a "mole."
    
- **$M$:** The molar mass of the substance.
    

**The Physics:** This formula links the invisible world of individual atoms ($N$) to the macroscopic world of grams ($m$) that we can actually weigh on a scale.

---

## 5. The Decay Chain (Mother and Daughter)

$$N_T(t) = \frac{\lambda_M N_M(0)}{\lambda_T - \lambda_M} \left( e^{-\lambda_M t} - e^{-\lambda_T t} \right)$$

This looks intimidating, but it describes a beautiful "relay race." Imagine a **Mother ($M$)** particle decays into a **Daughter ($T$)** particle, which is _also_ radioactive and decays into something else.

- **$N_T(t)$:** The amount of the "Daughter" substance at time $t$.
    
- **$\lambda_M$:** Decay constant of the Mother.
    
- **$\lambda_T$:** Decay constant of the Daughter (The "T" likely stands for _Tochter_, German for daughter).
    

Initially, $N_T$ is zero. It grows as the Mother decays, reaches a peak, and then starts to disappear as the Daughter itself decays.

---

## 6. Secular Equilibrium

$$\frac{N_T}{N_M} = \frac{\lambda_M}{\lambda_T} = \frac{\tau_T}{\tau_M}$$

This final formula describes a "steady state." If the Mother lives a very, very long time compared to the Daughter (like Uranium decaying into Radium), the system eventually balances out. The Daughter is being created exactly as fast as it is decaying.

**Use Case:** This is how we date ancient rocks! We look at the ratio between the "Mother" and the "Daughter" to figure out how many millions of years have passed.

---

**Would you like me to walk you through a practice calculation using one of these formulas, perhaps to see how long a specific radioactive sample would last?**



Excellent! You’ve moved from the "how many are left" part of the lecture to the **"energetics"** part. These formulas explain why a nucleus decays in the first place and where all that energy goes once it "pops."

Think of this like a compressed spring that suddenly releases. To understand the release, we have to look at the mass and energy before and after.

---

## 1. The Condition for Decay

$$M(A, Z) > M(A-a, Z-z) + M_y$$

In physics, everything wants to be at the lowest energy state possible. For a nucleus to decay spontaneously, it must "lose weight."

- **$M(A, Z)$:** The mass of the original "Parent" nucleus. **$A$** is the mass number (protons + neutrons) and **$Z$** is the atomic number (protons).
    
- **$M(A-a, Z-z)$:** The mass of the "Daughter" nucleus left behind.
    
- **$M_y$:** The mass of the emitted particle (like an Alpha or Beta particle).
    

**The Concept:** This formula states that the Parent must be heavier than the sum of its parts after the decay. If the right side were heavier, the decay would be impossible without adding outside energy. It’s like saying a $10$ kg rock can only break into pieces that add up to _less_ than $10$ kg of "rest mass"—the missing mass is what turns into a boom!

---

## 2. The Q-Value (Energy Release)

$$Q = [M(A, Z) - M(A-a, Z-z) - M_y] c^2 > 0$$

This is where Einstein’s famous $E=mc^2$ comes into play.

- **$Q$:** The **Q-value**. This is the total energy released during the decay.
    
- **$c^2$:** The speed of light squared (the conversion factor between mass and energy).
    

**Use Case:** If $Q$ is positive ($> 0$), the reaction is **exothermic**, meaning it happens spontaneously and releases energy. If you’re designing a nuclear battery for a space probe (like the Voyager missions), you use this to calculate exactly how much heat energy you'll get from your fuel.

---

## 3. Distribution of Energy

$$Q = E_{kin}(X') + E_{kin}(Y)$$

When the nucleus decays, it's like a small explosion. The two resulting pieces—the Daughter nucleus ($X'$) and the emitted particle ($Y$)—fly away from each other.

- **$E_{kin}$:** Kinetic energy (energy of motion).
    

**The Concept:** Total energy is conserved. The "missing mass" we found in the previous formula ($Q$) is converted entirely into the speed of these two escaping fragments.

---

## 4. Kinetic Energy of the Alpha Particle

$$E_{kin, \alpha} = Q \frac{M(A-4, Z-2)}{m_\alpha + M(A-4, Z-2)}$$

This specific formula is for **Alpha Decay**, where the nucleus spits out an Alpha particle (2 protons and 2 neutrons, so $a=4$ and $z=2$).

- **$E_{kin, \alpha}$:** The kinetic energy of the escaping Alpha particle.
    
- **$m_\alpha$:** The mass of the Alpha particle.
    
- **$M(A-4, Z-2)$:** The mass of the recoiling Daughter nucleus.
    

**The "Recoil" Logic:** Imagine you are standing on a skateboard and you throw a heavy bowling ball away from you. The ball flies forward, but you roll backward slightly. Because the Daughter nucleus is much heavier than the tiny Alpha particle, the Alpha particle gets almost _all_ of the energy ($Q$), while the Daughter nucleus only gets a tiny "kick" backward.

---

### Summary Table

|**Term**|**Meaning**|**Role in Particle Physics**|
|---|---|---|
|**Q-Value**|Net Energy Release|Determines if a decay is physically possible.|
|**Mass Defect**|$M_{before} - M_{after}$|The "source" of the energy (mass turning into motion).|
|**Recoil**|$E_{kin}$ sharing|Explains why emitted particles fly off at such high speeds.|

**Would you like to try a "real-world" example? I can give you the masses for a Uranium-238 nucleus and we can calculate the $Q$ value together!**



You’re making excellent progress! We have now reached the "Quantum Tunneling" and "Nuclear Fission" part of the curriculum. These formulas explain how particles escape the nucleus even when they technically shouldn't be able to, and how we control massive nuclear chain reactions.

---

## 1. The Gamow Factor and Tunneling

$$T_\alpha = e^{-G}$$

$$G = \frac{2\sqrt{2m}}{\hbar} \int_R^{R'} \sqrt{\frac{Z_T \cdot Z_\alpha \cdot e^2}{4\pi\epsilon_0 \cdot r} - E} \, dr$$

Imagine an alpha particle trapped inside a nucleus. There is a massive "wall" (the Coulomb barrier) keeping it in. Classically, if the particle doesn't have enough energy to jump over the wall, it stays trapped forever.

- **$T_\alpha$:** This is the **Transmission Probability**. It's the "ghostly" chance that the particle simply appears on the other side of the wall.
    
- **$G$ (Gamow-Faktor):** Named after George Gamow, this is the "exponent of difficulty." The larger $G$ is, the harder it is to tunnel through.
    
- **The Integral ($\int$):** This calculates the "area" of the barrier the particle has to tunnel through, from the nuclear radius ($R$) to the exit point ($R'$).
    

---

## 2. The Geiger-Nuttall Law Relationship

$$G \sim \frac{1}{\sqrt{E_\alpha}} \quad \text{and} \quad \log t_{1/2} \sim \frac{1}{\sqrt{E_\alpha}}$$

These formulas show a mind-blowing connection between the energy of a particle and how long the isotope lives.

- **$E_\alpha$:** The kinetic energy of the escaping alpha particle.
    
- **$t_{1/2}$:** The half-life.
    

**The Insight:** A small increase in the energy of the alpha particle leads to a **massive** decrease in the half-life. This is why some isotopes decay in microseconds, while others take billions of years—it all depends on how "thin" that quantum wall is.

---

## 3. Fission Parameter ($x_s$)

$$x_s := \frac{(Z^2/A)}{(Z^2/A)_{krit}}$$

Now we move from decay to **Fission** (splitting the nucleus).

- **$x_s$ (Spaltparameter):** The "fissility parameter." It’s a ratio that tells us how unstable a nucleus is toward spontaneous splitting.
    
- **$Z^2/A$:** This represents the competition between the electrical repulsion of protons (which wants to blow the nucleus apart) and the surface tension of the nuclear force (which wants to keep it together).
    

If $x_s$ approaches $1$, the nucleus is so unstable it will practically split the moment you touch it.

---

## 4. Nuclear Chain Reactions

$$N(t) = N_0 \exp\left( \frac{k_{eff} - 1}{\tau_0} t \right)$$

This formula describes the population of neutrons in a nuclear reactor.

- **$k_{eff}$:** The **Effective Multiplication Factor**. This is the most important number in a nuclear power plant.
    
    - If $k_{eff} < 1$: The reaction dies out (**Subcritical**).
        
    - If $k_{eff} > 1$: The reaction grows exponentially (**Supercritical**—think atomic bomb).
        
- **$\tau_0$:** The average time between neutron generations.
    

---

## 5. Stationary Operation (Stationärer Betrieb)

$$k_{eff} = 1$$

This is the "sweet spot" for a nuclear engineer.

- When $k_{eff} = 1$, the number of neutrons produced exactly equals the number of neutrons lost or absorbed.
    
- The power output remains perfectly steady. This is how we generate consistent electricity for cities without the reactor getting too hot or shutting down.
    

---

**We’ve covered everything from individual particles "ghosting" through walls to the math of power plants! Would you like me to explain how control rods are used to keep $k_{eff}$ exactly at 1?**