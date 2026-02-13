

You have reached the final challenge! This question is a "Conservation Law Obstacle Course." In particle physics, everything that _can_ happen _will_ happen, unless a fundamental law forbids it.

Your job is to play the referee: check if each reaction follows the rules. If it breaks a rule, you blow the whistle (Forbidden). If it follows all rules, you declare the game valid (Allowed) and name the force responsible.

Here is the checklist of rules we must apply to every single line:

1. **Charge ($Q$):** Total charge must be equal on both sides.
    
2. **Baryon Number ($B$):** Total number of baryons (protons, neutrons, hyperons) must be conserved. (Quarks have $B=1/3$, so 3 quarks = $B=1$).
    
3. **Lepton Number ($L$):** Total number of leptons must be conserved. _Crucially, this applies to each family separately ($L_e, L_\mu, L_\tau$)_.
    
4. **Energy/Mass:** The parent must be heavier than the daughters (for decays).
    
5. **Strangeness ($S$):** Conserved in Strong and Electromagnetic interactions, but _can_ change by 1 unit in Weak interactions.
    

Let's analyze them one by one.

---

### (a) ${}^{227}_{89}\text{Ac} \rightarrow {}^{223}_{87}\text{Fr} + \alpha$

- **Check Charge ($Z$):** Left $= 89$. Right $= 87 (\text{Fr}) + 2 (\alpha) = 89$. (OK)
    
- **Check Mass Number ($A$):** Left $= 227$. Right $= 223 + 4 = 227$. (OK)
    
- **Interaction:** This is a classic **Alpha Decay**. It is mediated by the **Strong Interaction** (formation of the alpha particle) and tunneling (quantum mechanics). In the context of nuclear decay classification, we just call it Alpha Decay.
    

**Verdict:** **Allowed** (Nuclear $\alpha$-decay).

---

### (b) ${}^{13}_{7}\text{N} + e^- \rightarrow {}^{13}_{6}\text{C} + \bar{\nu}_e$

- **Check Charge ($Q$):** Left $= +7 + (-1) = +6$. Right $= +6 + 0 = +6$. (OK)
    
- **Check Baryon Number ($B$):** 13 nucleons on both sides. (OK)
    
- **Check Lepton Number ($L_e$):**
    
    - Left: $e^-$ has $L_e = +1$. Total $= +1$.
        
    - Right: $\bar{\nu}_e$ (anti-neutrino) has $L_e = -1$. Total $= -1$.
        
    - **Mismatch!** $+1 \neq -1$.
        

**Verdict:** **Forbidden**.

_Reason:_ Lepton number conservation is violated. To make this work, you would need a regular neutrino ($\nu_e$), not an anti-neutrino. This looks like "Electron Capture," which should emit a $\nu_e$.

---

### (c) ${}^{235}_{92}\text{U} + n \rightarrow {}^{141}_{56}\text{Ba} + {}^{92}_{36}\text{Kr} + 3n$

- **Check Charge ($Z$):** Left $= 92$. Right $= 56 + 36 = 92$. (OK)
    
- **Check Mass Number ($A$):**
    
    - Left $= 235 + 1 = 236$.
        
    - Right $= 141 + 92 + 3(1) = 233 + 3 = 236$. (OK)
        
- **Interaction:** A heavy nucleus splits into two lighter ones after absorbing a neutron. This is **Nuclear Fission**.
    

**Verdict:** **Allowed** (Nuclear Fission).

---

### (d) $n + n \rightarrow \pi^0 + \gamma$

- **Check Charge ($Q$):** Left $= 0 + 0 = 0$. Right $= 0 + 0 = 0$. (OK)
    
- **Check Baryon Number ($B$):**
    
    - Left: Neutron ($B=1$) + Neutron ($B=1$) = **2**.
        
    - Right: Pion ($B=0$, meson) + Photon ($B=0$) = **0**.
        
    - **Mismatch!** $2 \neq 0$.
        

**Verdict:** **Forbidden**.

_Reason:_ Baryon number is not conserved. You cannot make two neutrons disappear into pure energy/mesons.

---

### (e) ${}^{60}_{28}\text{Ni}^* \rightarrow {}^{60}_{28}\text{Ni} + \gamma$

- **Check Charge & Mass:** Unchanged. (OK)
    
- **Process:** An excited nucleus ($*$) drops to its ground state by emitting a high-energy photon.
    
- **Interaction:** This is a **Gamma Decay**. It is an **Electromagnetic Interaction**.
    

**Verdict:** **Allowed** (Electromagnetic / $\gamma$-decay).

---

### (f) $n \rightarrow p + e^- + \bar{\nu}_e$

- **Check Charge ($Q$):** Left $= 0$. Right $= +1 + (-1) + 0 = 0$. (OK)
    
- **Check Baryon Number ($B$):** Left $= 1$. Right $= 1$ (proton). (OK)
    
- **Check Lepton Number ($L_e$):**
    
    - Left $= 0$.
        
    - Right: $e^-$ ($L=+1$) + $\bar{\nu}_e$ ($L=-1$) = $0$. (OK)
        
- **Interaction:** A neutron decaying into a proton is the definition of **Beta Decay**. Since neutrinos are involved, this is the **Weak Interaction**.
    

**Verdict:** **Allowed** (Weak Interaction / $\beta^-$-decay).

---

### (g) $e^+ \rightarrow \mu^+ + \nu_\mu + \bar{\nu}_e$

- **Check Energy/Mass:**
    
    - Parent: Positron ($e^+$) mass $\approx 0.511 \text{ MeV}$.
        
    - Daughter: Muon ($\mu^+$) mass $\approx 105 \text{ MeV}$.
        
    - **Problem:** You cannot create a heavy muon from a light positron! This violates conservation of energy.
        

**Verdict:** **Forbidden**.

_Reason:_ Violation of Energy Conservation (Mass of parent < Mass of products).

---

### (h) $\Omega^- \rightarrow \Xi^0 + \pi^-$

- **Hint Check:** $\Omega^-$ ($sss$), $\Xi^0$ ($uss$ - _wait, problem says $ssu$ which is correct_), $\pi^-$ ($d\bar{u}$).
    
- **Check Charge ($Q$):** Left $= -1$. Right $= 0 + (-1) = -1$. (OK)
    
- **Check Baryon Number ($B$):** Left $= 1$ (3 quarks). Right $= 1$ (3 quarks) + $0$ (meson). (OK)
    
- **Check Strangeness ($S$):**
    
    - Left ($\Omega^-$): 3 strange quarks $\rightarrow S = -3$.
        
    - Right ($\Xi^0$): 2 strange quarks $\rightarrow S = -2$. ($\pi^-$ has $S=0$).
        
    - **Change:** $\Delta S = 1$.
        
    - **Rule:** Strangeness can change by exactly 1 unit in **Weak Interactions**.
        
- **Interaction:** Since Strangeness is violated (but only by 1), this is allowed via the **Weak Interaction**.
    

**Verdict:** **Allowed** (Weak Interaction).

---

### Summary Table

|**Reaction**|**Status**|**Reason / Interaction**|
|---|---|---|
|**(a)**|**Allowed**|Strong (Alpha Decay)|
|**(b)**|**Forbidden**|Lepton Number violation ($L_e$)|
|**(c)**|**Allowed**|Nuclear Fission|
|**(d)**|**Forbidden**|Baryon Number violation|
|**(e)**|**Allowed**|Electromagnetic (Gamma Decay)|
|**(f)**|**Allowed**|Weak ($\beta$-decay)|
|**(g)**|**Forbidden**|Energy Conservation (Mass)|
|**(h)**|**Allowed**|Weak Decay ($\Delta S = 1$)|

And there you have it! You have successfully completed the exam review. You've analyzed accelerators, detectors, radioactive decay, nuclear stability, scattering structure, and conservation laws.

**Is there anything else I can help you with today? Good luck with your studies!**