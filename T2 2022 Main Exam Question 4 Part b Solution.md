

Welcome back! As your friendly neighborhood AI theoretical physics professor, I am absolutely thrilled to see your continued enthusiasm. You are diving right into the heart of quantum mechanics, and doing great.

Let's translate this second part so we are on the same page:

> **2. The ground state of the hydrogen atom is $\Psi_{100}(\vec{r}) = \frac{1}{\sqrt{\pi}}e^{-r}$. Calculate the expectation value of $r^2$ (Result: 3). [5 pts.]**

This is a classic and beautiful problem. We are given the wavefunction (the mathematical description of our electron) from the state we found in the previous question: $n=1, l=0, m=0$. The goal is to find the "expectation value" of $r^2$.

Here is how we break it down, step-by-step.

---

### Step 1: What is an "Expectation Value"?

In the quantum world, we cannot know the exact, pinpoint location of an electron. Instead, the wavefunction $\Psi$ gives us a _probability distribution_.

The **expectation value** (written with angle brackets, like $\langle r^2 \rangle$) is essentially the quantum mechanical version of an average. If you were to prepare millions of identical hydrogen atoms and measure $r^2$ (the square of the distance from the nucleus) for the electron in each one, the average of all those measurements would be the expectation value.

To find it mathematically, we use this fundamental formula:

$$\langle r^2 \rangle = \int_{\text{all space}} \Psi^*(\vec{r}) \cdot r^2 \cdot \Psi(\vec{r}) \, dV$$

- $\Psi^*$ is the complex conjugate of the wavefunction. (Since our given $\Psi$ has no imaginary numbers in it, $\Psi^* = \Psi$).
    
- $r^2$ is the thing we are trying to find the average of.
    
- $dV$ is our tiny piece of 3D volume.
    

---

### Step 2: Setting up the Integral in Spherical Coordinates

Because atoms are round, dealing with standard $x, y, z$ coordinates is a mathematical nightmare. Instead, physicists use **spherical coordinates**: $r$ (radius), $\theta$ (polar angle), and $\phi$ (azimuthal angle).

In spherical coordinates, integrating over "all space" means:

- $r$ goes from $0$ to $\infty$
    
- $\theta$ goes from $0$ to $\pi$
    
- $\phi$ goes from $0$ to $2\pi$
    

Crucially, our tiny volume piece $dV$ becomes $r^2 \sin\theta \, dr \, d\theta \, d\phi$.

Let's plug our wavefunction $\Psi_{100} = \frac{1}{\sqrt{\pi}}e^{-r}$ into the expectation value formula:

$$\langle r^2 \rangle = \int_0^{2\pi} \int_0^\pi \int_0^\infty \left( \frac{1}{\sqrt{\pi}}e^{-r} \right) \cdot r^2 \cdot \left( \frac{1}{\sqrt{\pi}}e^{-r} \right) \cdot (r^2 \sin\theta) \, dr \, d\theta \, d\phi$$

---

### Step 3: Solving the Math

Don't let the triple integral intimidate you! We can group the terms and separate the variables to make it much easier.

**1. Group everything together:**

- Constants: $\frac{1}{\sqrt{\pi}} \cdot \frac{1}{\sqrt{\pi}} = \frac{1}{\pi}$
    
- Exponentials: $e^{-r} \cdot e^{-r} = e^{-2r}$
    
- Radius terms: $r^2 \cdot r^2 = r^4$
    

So, our integral simplifies to:

$$\langle r^2 \rangle = \frac{1}{\pi} \int_0^{2\pi} d\phi \int_0^\pi \sin\theta \, d\theta \int_0^\infty r^4 e^{-2r} \, dr$$

**2. Solve the angular parts ($\theta$ and $\phi$):**

Because our wavefunction only depends on $r$ (it is perfectly spherical), the angular integrals are just standard constants!

- $\int_0^{2\pi} d\phi = 2\pi$
    
- $\int_0^\pi \sin\theta \, d\theta = 2$
    

Multiplying these gives $4\pi$. Now, multiply that by our constant $\frac{1}{\pi}$ out front: $\frac{4\pi}{\pi} = 4$.

Our massive physics equation has now shrunk to a single 1D integral:

$$\langle r^2 \rangle = 4 \int_0^\infty r^4 e^{-2r} \, dr$$

**3. Solve the radial part ($r$):**

To solve this, theoretical physicists rely on a standard integral formula (related to the Gamma function) that you will use constantly in this course:

> **The Handy Integral Trick:**
> 
> $$\int_0^\infty x^n e^{-ax} \, dx = \frac{n!}{a^{n+1}}$$

Looking at our integral, we can see that $n = 4$ and $a = 2$. Let's plug those in!

$$\int_0^\infty r^4 e^{-2r} \, dr = \frac{4!}{2^{4+1}} = \frac{4 \cdot 3 \cdot 2 \cdot 1}{2^5} = \frac{24}{32}$$

This fraction simplifies beautifully to $\frac{3}{4}$.

**4. The Final Calculation:**

Bring back the $4$ we saved from the angular parts:

$$\langle r^2 \rangle = 4 \cdot \left(\frac{3}{4}\right) = 3$$

And there we have it! The math perfectly matches the result given in the problem prompt. You have just successfully calculated a quantum expectation value.

---

Would you like me to show you how to calculate the expectation value of just the radius $\langle r \rangle$ using this exact same method to see how it differs?