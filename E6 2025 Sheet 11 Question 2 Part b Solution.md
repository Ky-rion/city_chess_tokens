

![[Pasted image 20260206202937.png]]

Welcome back to class! I am happy to guide you through Part (b).

In Part (a), we looked at **Free Electrons**. Those electrons could fly around anywhere, like gas particles, and their energy graph was a simple parabola ($k^2$).

In Part (b), we are switching to the **Tight-Binding Model**. This is a very different physical picture. Here, electrons are "tightly bound" to atoms and can only "hop" from one atom to its neighbor. Because they are on a grid, their energy behaves like a wave on a grid—it oscillates. That is why you see **cosine** functions in the equation instead of just $k^2$.

Let's break down the solution provided in the image step-by-step.

### 1. The Energy Equation

The problem gives us the **dispersion relation** (the relationship between energy $E$ and momentum $k$):

$$E_{\vec{k}} = -t \left[ \cos(k_x a) + \cos(k_y a) - 2 \right]$$

Here is what the symbols mean:

- **$t$**: The "hopping parameter." It represents the energy associated with an electron hopping from one site to the next. It is usually a positive number.
    
- **$a$**: The lattice constant (distance between atoms).
    
- **$\cos(k a)$**: This tells us the energy is periodic. The cosine function always stays between **+1** and **-1**.
    

To find the minimum and maximum energy, we just have to play with the cosine values.

---

### 2. Finding the Minimum Energy ($E_{min}$)

We want to find the lowest possible value for $E_{\vec{k}}$.

Looking at the equation, we have a minus sign in front: $-t [\dots]$.

To make the total energy small (or close to zero), we need the part inside the brackets $[\dots]$ to be as **large (positive)** as possible, or effectively zero if we can't make it positive enough to counteract the offset.

We know the maximum value of any cosine is **+1**. This happens when the angle is 0.

- **Location:** The center of the Brillouin Zone, often called the $\Gamma$-point.
    
- **Coordinates:** $k_x = 0$ and $k_y = 0$.
    

Let's plug $\vec{k} = (0,0)$ into the equation:

$$E_{min} = -t \left[ \cos(0) + \cos(0) - 2 \right]$$

$$E_{min} = -t \left[ 1 + 1 - 2 \right]$$

$$E_{min} = -t \left[ 0 \right]$$

$$E_{min} = 0$$

So, the bottom of the energy band is at **0**.

---

### 3. Finding the Maximum Energy ($E_{max}$)

Now we want the highest possible energy.

Because of the leading minus sign ($-t$), to get a huge positive number, we need the inside of the bracket $[\dots]$ to be a **large negative number**.

We know the minimum value of any cosine is **-1**. This happens when the angle is $\pi$ ($180^\circ$).

- **Location:** The corner of the Brillouin Zone.
    
- **Coordinates:** $k_x = \frac{\pi}{a}$ and $k_y = \frac{\pi}{a}$.
    
    _(Note: If we plug this in, the argument of the cosine becomes $\frac{\pi}{a} \cdot a = \pi$.)_
    

Let's plug $\vec{k} = (\frac{\pi}{a}, \frac{\pi}{a})$ into the equation:

$$E_{max} = -t \left[ \cos(\pi) + \cos(\pi) - 2 \right]$$

$$E_{max} = -t \left[ (-1) + (-1) - 2 \right]$$

$$E_{max} = -t \left[ -4 \right]$$

$$E_{max} = +4t$$

So, the top of the energy band is at **4t**.

---

### 4. Calculating the Bandwidth ($W$)

The **Bandwidth** is simply the "width" of the energy range available to the electrons. It is the difference between the ceiling and the floor.

$$W = E_{max} - E_{min}$$

$$W = 4t - 0$$

$$W = 4t$$

### Summary of the Professor's Solution

The German text in your second image confirms exactly this:

1. **Minimum:** It states "_Das Band Minimum liegt im Zentrum..._" (The band minimum lies in the center) at $\vec{k}=(0,0)$ with a value of **0**.
    
2. **Maximum:** It states "_Das Bandmaximum liegt bei..._" (The band maximum lies at) $\vec{k}=(\frac{\pi}{a}, \frac{\pi}{a})$ with a value of **4t**.
    
3. **Bandwidth:** It concludes "_Die Bandbreite ist demnach_" (The bandwidth is therefore) **4t**.
    

**Physics Takeaway:**

The bandwidth ($4t$) tells us how mobile the electrons are. If $t$ is large (strong hopping), the band is wide, and electrons move easily (high velocity). If $t$ is small, the band is flat (narrow bandwidth), and electrons are heavy and slow.

Would you like to move on to the next part of the question?