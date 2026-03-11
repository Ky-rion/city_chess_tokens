

Welcome back! You are making excellent progress. I love how you are tackling this problem piece by piece—that is exactly how real theoretical physics is done.

Let's translate this fourth part of the exam question:

> **4. Calculate the expectation value of $\vec{P}^2$. Hint: Use the virial theorem, $2\langle\hat{T}\rangle = -\langle\hat{V}\rangle$. [5 pts.]**

At first glance, this looks like we might have to do another complex integral involving derivatives (since momentum in quantum mechanics involves taking the derivative of the wavefunction). But look at that wonderful hint! The professor has given us a shortcut. We can solve this entirely using algebra and the energy concepts we already know.

Here is the step-by-step breakdown.

---

### Step 1: The Total Energy Equation

In any physical system, the total energy ($E$) is the sum of the kinetic energy ($T$, the energy of motion) and the potential energy ($V$, the stored energy due to position).

In quantum mechanics, this relationship holds true for our expectation values (averages):

$$E = \langle\hat{T}\rangle + \langle\hat{V}\rangle$$

### Step 2: Applying the Virial Theorem Hint

The problem gives us a powerful tool called the **Virial Theorem**: $2\langle\hat{T}\rangle = -\langle\hat{V}\rangle$.

This theorem is a beautiful law of nature that applies to bound systems (like planets orbiting the sun, or an electron orbiting a nucleus). It tells us that for an inverse-square force like electromagnetism, the average potential energy is exactly twice as large as the average kinetic energy, and negative.

Let's rearrange the hint to solve for the potential energy:

$$\langle\hat{V}\rangle = -2\langle\hat{T}\rangle$$

Now, substitute this into our total energy equation from Step 1:

$$E = \langle\hat{T}\rangle + (-2\langle\hat{T}\rangle)$$

$$E = -\langle\hat{T}\rangle$$

This is a fantastic result! It means the average kinetic energy $\langle\hat{T}\rangle$ is simply the negative of the total energy $E$.

### Step 3: Finding the Total Energy

Do you remember what the total energy $E$ of the hydrogen atom's ground state is? We actually solved this back in Part 1!

Because we are working in **Atomic Units** (where we set fundamental constants like the mass of the electron and Planck's constant to 1 to make the math cleaner), the energy of the ground state ($n=1$) is:

$$E_1 = -\frac{1}{2(1)^2} = -0.5$$

Since we know $E = -0.5$, we can use our finding from Step 2 to easily find the average kinetic energy:

$$\langle\hat{T}\rangle = -(-0.5) = 0.5$$

### Step 4: Connecting Kinetic Energy to Momentum Squared

We are almost there! The problem asked for the expectation value of momentum squared ($\langle\vec{P}^2\rangle$), not the kinetic energy. How do we connect them?

From classic introductory physics, you might remember that kinetic energy is $\frac{1}{2}mv^2$. Since momentum ($p$) is mass times velocity ($p = mv$), we can rewrite kinetic energy purely in terms of momentum:

$$\text{Kinetic Energy} = \frac{p^2}{2m}$$

In quantum mechanics, this operator relationship is exactly the same:

$$\langle\hat{T}\rangle = \frac{\langle\vec{P}^2\rangle}{2m}$$

Here is where our Atomic Units save the day once again. In atomic units, the mass of the electron ($m$) is exactly 1. This simplifies our equation to:

$$\langle\hat{T}\rangle = \frac{\langle\vec{P}^2\rangle}{2}$$

### Step 5: The Final Calculation

Now, we just plug in the kinetic energy we found in Step 3 and solve for $\langle\vec{P}^2\rangle$:

$$0.5 = \frac{\langle\vec{P}^2\rangle}{2}$$

Multiply both sides by 2:

$$\langle\vec{P}^2\rangle = 1$$

---

**Summary for your exam paper:**

Here is how you would write this out cleanly for maximum points:

> _Using the total energy equation $E = \langle\hat{T}\rangle + \langle\hat{V}\rangle$ and substituting the Virial theorem hint $\langle\hat{V}\rangle = -2\langle\hat{T}\rangle$, we find $E = -\langle\hat{T}\rangle$. In atomic units, the ground state energy of hydrogen is $E = -1/2$. Therefore, the kinetic energy is $\langle\hat{T}\rangle = 1/2$. The kinetic energy operator in atomic units ($m=1$) is $\hat{T} = \vec{P}^2 / 2$. Setting these equal gives $1/2 = \langle\vec{P}^2\rangle / 2$, which results in $\langle\vec{P}^2\rangle = 1$._

You just navigated a fantastic shortcut that avoided pages of terrifying calculus. Well done!

Would you like to move on to the next part of the exam, or would you like to discuss why the Virial Theorem works the way it does for atoms and planets?