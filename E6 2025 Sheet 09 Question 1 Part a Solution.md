

![[Pasted image 20260126135159.png]]

Hello there! Welcome to your first solid-state physics session. I'm delighted to walk you through this. Solid-state physics is fascinating because it is the playground where classical mechanics (things you can see and touch) shakes hands with quantum mechanics (the behavior of atoms and subatomic particles).

This problem is a classic "bridge" problem. It takes a concept you probably know from high school physics (Force) and translates it into the language of quantum mechanics (Wavevectors).

Let's break down part **a)** step-by-step, using the solution provided by your other professor.

### 1. The Translation (What are we asked?)

First, let's make sure we understand exactly what the German text is asking.

**The Question (Image 1):**

> "In the derivation, we consider a piece of metal to which an electric field $\vec{E}$ is applied. Use $\vec{F} = \dot{\vec{p}}$ to find an expression for the time rate of change of the mean reciprocal vector $\frac{\partial \langle \vec{k} \rangle}{\partial t} |_{el}$ caused by the electric field."

**The Goal:**

We want to find a formula that tells us: _How fast does the electrons' quantum state ($\vec{k}$) change when we push on them with an electric field ($\vec{E}$)?_

---

### 2. The Physics: Step-by-Step Derivation

To solve this, we are going to chain together three simple concepts.

#### Step 1: Classical Force (The Push)

Imagine an electron floating in space. If you turn on an Electric Field ($\vec{E}$), the electron feels a force.

The formula for electric force is:

$$\vec{F} = q \cdot \vec{E}$$

Since the charge ($q$) of an electron is usually written as $-e$ (where $e$ is the elementary charge), the force is:

$$\vec{F} = -e\vec{E}$$

_(Note: In the solution provided in Image 2, the professor writes $\vec{F} = -\vec{E}e$. This is the same thing, just rearranged.)_

#### Step 2: Newton's Law (The Motion)

Now, what does a Force _do_? Newton told us that Force equals the rate of change of momentum ($\vec{p}$). This is exactly the hint given in the question text: $\vec{F} = \dot{\vec{p}}$.

_(Note: The dot over the $p$ is a physics shorthand for "time derivative", or $\frac{d\vec{p}}{dt}$.)_

So, if we combine Step 1 and Step 2, we get:

$$\dot{\vec{p}} = -e\vec{E}$$

This tells us that the momentum of the electron is changing over time because the electric field is pushing it.

#### Step 3: The Quantum Leap (The Translation)

Here is where we leave classical physics and enter solid-state physics. In this world, we describe electrons not just as particles with mass $m$ and velocity $v$, but as waves.

We describe the "state" of an electron using a **Wavevector**, denoted as $\vec{k}$.

There is a fundamental bridge connecting the classical momentum ($\vec{p}$) to the quantum wavevector ($\vec{k}$). This is the **de Broglie relation**:

$$\vec{p} = \hbar \vec{k}$$

Here, $\hbar$ (pronounced "h-bar") is the reduced Planck constant. It is just a number that acts as the exchange rate between the classical world and the quantum world.

If momentum is changing ($\dot{\vec{p}}$), then the wavevector must be changing too, because $\hbar$ is just a constant number.

$$\dot{\vec{p}} = \frac{d}{dt}(\hbar \vec{k}) = \hbar \frac{d\vec{k}}{dt}$$

### 3. Putting it together (The Solution Explanation)

Now, look at the solution in the second image. The professor has simply chained these equalities together in one line:

$$\vec{F} = -\vec{E}e = \dot{\vec{p}} = m\frac{\partial \langle \vec{v} \rangle}{\partial t} = \hbar \frac{\partial \langle \vec{k} \rangle}{\partial t}$$

Let's ignore the velocity part ($m\frac{\partial \langle \vec{v} \rangle}{\partial t}$) for a second—that's just the classical way of writing it ($F=ma$). We care about the quantum way.

Take the beginning and the end of that chain:

$$-e\vec{E} = \hbar \frac{\partial \langle \vec{k} \rangle}{\partial t}$$

Now, we just want to isolate the change in the wavevector ($\frac{\partial \langle \vec{k} \rangle}{\partial t}$). To do that, we divide both sides by $\hbar$:

$$\frac{\partial \langle \vec{k} \rangle}{\partial t} = -\frac{e\vec{E}}{\hbar}$$

**And that is the answer shown in the second image!**

---

### Professor's Insight: What does this actually mean?

You might be wondering, "Why do we care about $\vec{k}$ changing?"

In a metal, you don't just have one electron; you have billions of them. We picture them filling up a sphere in "k-space" (imagine a ball of occupied states). This is called the **Fermi Sphere**.

1.  **No Field:** The sphere is centered at zero. For every electron moving right, there is one moving left. The _average_ $\vec{k}$ ($\langle \vec{k} \rangle$) is zero. No current flows.
    
2.  **Field On:** The electric field applies a force. Our equation tells us that **$\vec{k}$ changes linearly with time**.
    
3.  **The Shift:** This means the _entire sphere of electrons_ starts drifting through k-space. The center of the sphere ($\langle \vec{k} \rangle$) moves away from zero.
    

This drift is essentially what **electric current** is! We have mathematically described how electricity starts to flow at a quantum level.

Would you like me to explain part b) next, or do you have questions about the "Fermi Sphere" concept first?