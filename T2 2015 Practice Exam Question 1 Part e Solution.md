

![[Pasted image 20251108140133.png]]


Ah, the photoelectric effect! This is one of the most important experiments in history; it's what won Albert Einstein his Nobel Prize and truly launched the quantum revolution.

The classical physics of the time (viewing light as a wave) made predictions that were _completely wrong_, and this question gets at exactly _how_ they were wrong.

Let's break down the question and the solution.

---

### 1. How does electron energy depend on light _frequency_? (Words)

The question first asks for the relationship between the emitted electron's energy and the light's frequency.

-   **The Old (Wrong) Idea:** Classically, light is a wave. A brighter (more intense) wave has more energy. So, a brighter light should kick out electrons with more energy. The _frequency_ (color) of the light shouldn't really matter.
    
-   **The New (Correct) Idea:** Einstein proposed that light isn't a continuous wave, but comes in tiny, discrete packets of energy called **photons**. The energy of a _single_ photon is determined _only_ by its frequency ($\nu$), using the formula $E_{\text{photon}} = h\nu$.
    
-   **The "Work Function" (Offset):** An electron is bound to the metal. It takes a certain minimum amount of energy just to _free_ it from the surface. This "exit fee" is a property of the metal and is called the **Work Function** (often written as $\Phi$ or $W$).
    
-   **Putting It Together:**
    
    1.  A single photon (with energy $h\nu$) hits a single electron.
        
    2.  The electron first "pays" the work function $\Phi$ to escape.
        
    3.  Whatever energy is _left over_ becomes the electron's kinetic energy ($E_e$), which is its "emission energy."
        
    4.  If the photon's energy $h\nu$ is _less_ than the work function $\Phi$, the electron can't pay the fee, and _nothing happens_. The minimum frequency needed to pay the fee is called the "threshold frequency," $\nu_0$, where $\Phi = h\nu_0$.
        

This directly explains the first two lines of the solution:

-   `Die Emissionsenergie wächst linear mit der Frequenz` (The emission energy grows linearly with the frequency). This is because $E_e = (\text{Photon Energy}) - (\text{Work Function})$. Since Photon Energy ($h\nu$) is linear with frequency, $E_e$ is also linear with frequency.
    
-   `Es gibt einen Offset (“Work-Function”)` (There is an offset ("Work-Function")). This confirms you must first overcome the work function. The linear graph of $E_e$ vs. $\nu$ doesn't start at (0,0); it starts at $(\nu_0, 0)$.
    

---

### 2. How does electron energy depend on light _frequency_? (Formula)

This is now just writing the logic from above as an equation.

**$\text{Emission Energy} = \text{Photon Energy} - \text{Work Function}$**

$$E_e = h\nu - h\nu_0$$

This is exactly what the solution provides:

> **$E_e = h(\nu - \nu_0)$**

(The solution also gives **$E_e = \hbar(\omega - \omega_0)$**, which is the exact same formula. It just uses angular frequency $\omega = 2\pi\nu$ and the reduced Planck constant $\hbar = h/2\pi$. It's just a different set of units for the same physics.)

---

### 3. What happens if you increase the _intensity_? (Verbal)

This is the second key part of the experiment. The question asks what happens if we make the light _brighter_ (increase intensity) but keep the _color_ the same (fix the frequency/wavelength).

-   **Fixed Frequency** means every single photon still has the _exact same_ energy ($h\nu$) as before.
    
-   **Increased Intensity** (brighter light) simply means there are _more photons_ streaming onto the metal every second.
    

So, what's the result?

-   Since each photon's energy is unchanged, the _maximum_ energy any single electron can gain is also **unchanged**. The "energy per electron" stays the same.
    
-   But, since there are _more photons_ hitting the metal, they will knock out _more electrons_ per second.
    

This perfectly matches the last line of the solution:

> Es werden mehr Elektronen emittiert, doch die Energie pro Elektron bleibt gleich.
> 
> (More electrons are emitted, but the energy per electron stays the same.)

This result was shocking at the time. A "brighter" light doesn't make the electrons fly out _faster_, it just makes _more_ of them fly out! This was iron-clad proof that light behaves as a particle (a photon).

We're almost at the end! What's the next question?