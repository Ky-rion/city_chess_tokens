

https://gemini.google.com/share/d3198665ca89


Hello! Come in, have a seat. It is wonderful to have you in my office. Don't worry if the notes look like ancient hieroglyphics right now—particle physics often looks like that until you find the narrative hidden in the math.

These notes describe one of the most fundamental tools we have in physics: **Electron Scattering**. Think of this as using a very high-powered electron microscope to "see" inside the atomic nucleus.

Here is an overview of the material, structured from the basic concepts to the advanced applications, exactly as we would build it up in a lecture.

---

### 1. The Basics: Rutherford Scattering

The story begins with the simplest approximation. We imagine shooting an electron at a nucleus.

- **The Assumption:** We assume the nucleus is a fixed, heavy **point charge** (no size) and we ignore the "spin" of the electron.
    
- **The Physics:** The interaction is purely electromagnetic (Coulomb force). We use **Fermi's Golden Rule** to calculate the probability of the electron bouncing off.
    
- **The Result:** This gives us the **Rutherford Cross-Section** $(\frac{d\sigma}{d\Omega})_{Rutherford}$.
    
    - The "Cross-Section" ($\sigma$) effectively tells us how "big" the target looks to the incoming beam—it is a measure of the probability of a collision.
        
    - A key signature of Rutherford scattering is that the probability drops off sharply with the scattering angle $\theta$, specifically proportional to $\frac{1}{\sin^4(\theta/2)}$.
        

### 2. Adding Reality: Mott Scattering

Rutherford is a great start, but it fails in real experiments because electrons are not just simple charged balls; they are quantum particles with **spin**.

- **The Correction:** When we account for the electron's spin and relativistic effects (when the electron moves close to the speed of light, $v \approx c$), we get the **Mott Cross-Section**.
    
- **The Formula:**
    
    $$\left(\frac{d\sigma}{d\Omega}\right)^*_{Mott} = \left(\frac{d\sigma}{d\Omega}\right)_{Rutherford} \cdot \left(1 - \beta^2 \sin^2\frac{\theta}{2}\right)$$
    
- **Key Takeaway:** The Mott cross-section is the "Rutherford" cross-section multiplied by a correction factor for spin and relativity.
    

### 3. The "Blob" Factor: The Form Factor $F(q)$

This is perhaps the most important concept in these notes. Real nuclei are **not** points; they have a volume and a shape.

- **The Definition:** To account for the fact that the charge is spread out, we introduce the **Form Factor**, $F(\vec{q})$.
    
- **The Modification:** The actual cross-section becomes the Mott cross-section multiplied by the square of this form factor:
    
    $$\frac{d\sigma}{d\Omega} = \left(\frac{d\sigma}{d\Omega}\right)^*_{Mott} \cdot |F(\vec{q})|^2$$
    
- **The Physical Meaning:** The Form Factor is actually the **Fourier Transform of the charge distribution** $\rho(r)$ of the nucleus.
    
    - If the nucleus were a point, $F(q) = 1$.
        
    - Since it is a "blob" of charge, $F(q) < 1$ as the momentum transfer increases.
        

### 4. Measuring the Size of the Nucleus

We can use the Form Factor to measure the radius of a nucleus.

- **The Trick:** We look at the Form Factor $F(q)$ when the momentum transfer $q$ is very small (near zero).
    
- **The Formula:** The slope of the Form Factor at this point gives us the **mean square radius** $\langle r^2 \rangle$:
    
    $$\langle r^2 \rangle = -6\hbar^2 \frac{dF(q^2)}{dq^2} \bigg|_{q=0}$$
    
- **Result:** This is how we know, for example, that the proton radius is roughly $0.8 \text{ fm}$ (femtometers).
    

### 5. Deep Dive: The Rosenbluth Formula

Finally, the notes move to scattering off individual **nucleons** (protons and neutrons). This is harder because protons and neutrons have strong magnetic moments and they recoil (bounce back) significantly when hit.

- **Two Form Factors:** We need two factors now:
    
    1. $G_E(Q^2)$: The **Electric** form factor (charge distribution).
        
    2. $G_M(Q^2)$: The **Magnetic** form factor (magnetic moment distribution).
        
- **The Rosenbluth Formula:** This formula combines these two to describe electron-proton scattering. By plotting the data in a specific way (the "Rosenbluth plot"), experimentalists can separate $G_E$ and $G_M$ to understand the internal structure of the proton.
    

---

### Professor's Cheat Sheet: What to memorize for the Exam

If I were writing your exam, these are the questions I would ask based on these notes:

1. **Relation between Charge & Form Factor:** You **must** know that the Form Factor $F(\vec{q})$ is the Fourier transform of the charge density $\rho(r)$.
    
    - _Exam Question:_ "Given a charge distribution $\rho(r)$, how do you calculate the form factor?"
        
2. **The Hierarchy of Cross-Sections:**
    
    - **Rutherford:** Point target, no electron spin.
        
    - **Mott:** Point target, **with** electron spin (adds $\cos^2(\theta/2)$ factor effectively).
        
    - **Form Factor:** Extended target (multiplied by $|F(q)|^2$).
        
3. **Determination of Radius:** Know that the root-mean-square radius is determined by the **slope** of the Form Factor at $q^2=0$.
    
4. **The Dipole Fit:** The proton's form factor is often approximated by a "Dipole" shape, which corresponds to an exponential charge distribution in real space.
    
5. **Nucleon Differences:**
    
    - Proton: Has electric charge ($G_E(0)=1$) and magnetic moment ($G_M(0) = \mu_p$).
        
    - Neutron: Has **no** net electric charge ($G_E(0)=0$) but **does** have a magnetic moment ($G_M(0) = \mu_n$).
        

Does this overview help you see the "story" in the notes? Would you like me to walk you through the specific derivation of the nuclear radius on Page 11?