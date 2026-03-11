

Hello again! It's wonderful to see you tackling the next part of the exam. We are moving from the deep philosophical foundations of quantum mechanics straight into the nuts and bolts of atomic physics.

Before we crunch the numbers, let's translate the text and understand the physical phenomenon at play here.

### The Translation

**1.2 Auger Effect**

_Given a helium atom in a doubly excited eigenstate with quantum numbers $n_1 = 2$ and $n_2 = 3$. Let the energy of the doubly excited state be $E_2 + E_3$, as without electron repulsion. [2 Pts.]_

_Due to the Auger effect, one of the electrons transitions to the ground state with energy $E_1$. With what energy $E$ is the other electron emitted? Calculate the concrete number in atomic units._

---

### The Physics: What is the Auger Effect?

Imagine an atom with an empty spot in one of its lower, inner electron shells. An electron from a higher, outer shell will naturally want to "fall" down to fill that lower-energy vacancy.

Usually, when an electron drops to a lower energy state, the atom releases the excess energy by spitting out a photon (light). But atoms have another trick up their sleeves: the **Auger Effect** (pronounced _oh-zhay_, named after Pierre Auger).

Instead of emitting a photon, the electron dropping down transfers its excess energy _directly_ to another electron in the atom. If this energy is large enough, it acts like a microscopic billiard break, kicking that second electron completely out of the atom. The electron that gets ejected is called an **Auger electron**, and the energy it carries away is purely kinetic.

In our problem's specific scenario:

1. We have a highly unstable Helium atom where both electrons are excited (one is at $n=2$, the other is at $n=3$).
    
2. One electron drops all the way down to the ground state ($n=1$).
    
3. It gives its energy to the other electron, which absorbs it and flies away, leaving us with a positively charged Helium ion ($He^+$) and a free electron.
    

---

### Step-by-Step Calculation

The question asks us to use **atomic units** (a.u.) and gives us a massive simplification: we can pretend electron-electron repulsion doesn't exist. This means we can treat these electrons as if they are independently orbiting a bare nucleus.

**Step 1: The Energy Formula**

In atomic units, the energy of an electron in a hydrogen-like atom (a single electron orbiting a nucleus of charge $Z$) is given by the formula:

$$E_n = -\frac{Z^2}{2n^2}$$

Since we are dealing with Helium, our atomic number is **$Z=2$**.

**Step 2: Calculate the Energy Levels**

Let's find the specific energies for the levels mentioned in the problem:

- **Ground state ($n=1$):**
    
    $$E_1 = -\frac{2^2}{2(1)^2} = -2 \text{ a.u.}$$
    
- **First excited state ($n=2$):**
    
    $$E_2 = -\frac{2^2}{2(2)^2} = -\frac{4}{8} = -\frac{1}{2} \text{ a.u.}$$
    
- **Second excited state ($n=3$):**
    
    $$E_3 = -\frac{2^2}{2(3)^2} = -\frac{4}{18} = -\frac{2}{9} \text{ a.u.}$$
    

**Step 3: Apply Conservation of Energy**

One of the most sacred rules in physics is that total energy must be conserved. The energy we start with must equal the energy we end up with.

- **Initial State:** Both electrons are excited.
    
    $$E_{initial} = E_2 + E_3$$
    
- **Final State:** One electron is in the ground state ($E_1$), and the other is flying away free. Because the Auger electron has escaped the pull of the nucleus, its potential energy is zero, and it only has kinetic energy, which the problem labels $E$.
    
    $$E_{final} = E_1 + E$$
    

Now, we set them equal to each other and solve for $E$:

$$E_{initial} = E_{final}$$

$$E_2 + E_3 = E_1 + E$$

$$E = E_2 + E_3 - E_1$$

**Step 4: The Final Math**

Plug in the fractions we calculated in Step 2:

$$E = \left(-\frac{1}{2}\right) + \left(-\frac{2}{9}\right) - (-2)$$

$$E = -\frac{9}{18} - \frac{4}{18} + \frac{36}{18}$$

$$E = \frac{23}{18} \text{ a.u.}$$

If you want to write that as a decimal, it's roughly **1.278 a.u.**

---

You just calculated the emission energy of an Auger electron!

In reality, the electrons in a helium atom _do_ repel each other, which shifts these energy levels. Would you like me to show you how physicists use a technique called "Perturbation Theory" to correct for that electron-electron repulsion and get an exact real-world number?