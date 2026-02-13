

Here is your "Particle Physics Decay" cheat sheet. These rules are universal for strong interaction decays. If you memorize these three sections, you will be able to solve almost any question like this on an exam.

### 1. Angular Momentum Conservation (Spin)

**The Concept:** Spins don't just add up like normal numbers ($1+1=2$); they add up like vectors ($\vec{A} + \vec{B} = \vec{C}$).

- **The Master Equation:**
    
    $$J_{\text{parent}} = S_1 \oplus S_2 \oplus l$$
    
    _(Parent Spin = Vector sum of Daughter Spins + Orbital Angular Momentum)_
    
- **Step-by-Step Algorithm:**
    
    1. **Combine Daughter Spins:** Add the intrinsic spins of the daughters ($S_1, S_2$) to find the total channel spin ($S'$).
        
        $$|S_1 - S_2| \le S' \le S_1 + S_2$$
        
    2. **Add Orbital Momentum ($l$):** Use the "Triangle Inequality" to see which values of $l$ allow you to reach the Parent Spin ($J$).
        
        $$|l - S'| \le J \le l + S'$$
        
- **Important Constraint:** Orbital angular momentum ($l$) must always be an **integer** ($0, 1, 2, \dots$).
    

---

### 2. Parity Conservation ($P$)

**The Concept:** The Strong force conserves parity. Parity is **multiplicative**, not additive.

- **The Master Equation:**
    
    $$P_{\text{parent}} = P_{\text{daughter 1}} \times P_{\text{daughter 2}} \times P_{\text{orbital}}$$
    
- **The Orbital Parity Rule (Crucial!):**
    
    Moving particles have a parity determined solely by their orbital angular momentum ($l$).
    
    $$P_{\text{orbital}} = (-1)^l$$
    
    - If $l$ is **even** ($0, 2, \dots$) $\rightarrow$ Parity is **$+1$**.
        
    - If $l$ is **odd** ($1, 3, \dots$) $\rightarrow$ Parity is **$-1$**.
        

---

### 3. Intrinsic Properties to Memorize

You generally don't calculate these; you just have to know them.

| **Particle Type**       | **Examples**                                    | **Intrinsic Spin (S)** | **Intrinsic Parity (P)**        |
| ----------------------- | ----------------------------------------------- | ---------------------- | ------------------------------- |
| **Baryons**             | Proton ($p$), Neutron ($n$)                     | $1/2, 3/2, \dots$      | **$+1$**                        |
| **Anti-Baryons**        | Antiproton ($\bar{p}$), Antineutron ($\bar{n}$) | $1/2, 3/2, \dots$      | **$-1$** _(Opposite to matter)_ |
| **Pseudoscalar Mesons** | Pion ($\pi$), Kaon ($K$)                        | $0$                    | **$-1$**                        |
| **Vector Mesons**       | Rho ($\rho$), Omega ($\omega$)                  | $1$                    | **$-1$**                        |
| **Photon**              | $\gamma$                                        | $1$                    | **$-1$**                        |

> **Pro Tip:**
> 
> - **Fermions** (matter) and Anti-fermions have **opposite** parity.
>     
> - **Bosons** (force carriers/mesons) and Anti-bosons have the **same** parity.
>     

---

### 4. Exam Strategy Checklist

When you see a decay problem ($\Delta \rightarrow n + \pi$):

1. [ ] Write down $J$ and $P$ for every particle given.
    
2. [ ] Combine the daughter spins first.
    
3. [ ] Find allowed $l$ values using the Triangle Rule.
    
4. [ ] Check Parity for each allowed $l$.
    
5. [ ] Eliminate any $l$ values that violate Parity conservation.
    

**Would you like to try applying this cheat sheet to a slightly different particle decay problem to test your understanding?**