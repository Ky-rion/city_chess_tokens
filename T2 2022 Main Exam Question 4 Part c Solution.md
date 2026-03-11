

Welcome back to class! It is so great to see you tackling these parts one by one. You are doing exactly what a good theoretical physicist does: breaking a complex system down into manageable, logical pieces.

Let's translate this third part of the problem:

> **3. The expectation value $\langle x^2 \rangle$ in the ground state is equal to $\langle r^2 \rangle / 3$. Why? Give a precise justification. [2 pts.]**

This is one of my absolute favorite types of questions. Why? Because it looks like it's asking you to do another massive, complicated integral, but it is actually a **trick question**! It is testing if you understand the _physical geometry_ of the atom. We can solve this entirely using logic and zero calculus.

Here is the step-by-step justification you need.

---

### Step 1: The Geometry of 3D Space (Pythagorean Theorem)

First, let's think about how distance works in three dimensions. The variable $r$ represents the straight-line distance from the nucleus (the origin, at $0,0,0$) to the electron.

Using the 3D version of the Pythagorean theorem, the square of the total distance $r^2$ is simply the sum of the squares of its $x$, $y$, and $z$ components:

$$r^2 = x^2 + y^2 + z^2$$

### Step 2: The Rules of Quantum Averages

In quantum mechanics, expectation values (our quantum averages, denoted by the angle brackets $\langle \dots \rangle$) are "linear." This is a fancy way of saying that the average of a sum is equal to the sum of the averages.

If we apply expectation brackets to our Pythagorean equation, we get:

$$\langle r^2 \rangle = \langle x^2 + y^2 + z^2 \rangle$$

$$\langle r^2 \rangle = \langle x^2 \rangle + \langle y^2 \rangle + \langle z^2 \rangle$$

This tells us that the total average squared distance ($\langle r^2 \rangle$) is just the sum of the average squared distances along the $x$, $y$, and $z$ axes.

### Step 3: The Power of Symmetry (The "Aha!" Moment)

Now, we need to think about the specific state the electron is in. The problem specifies the **ground state**.

From Part 1, we know the ground state is the 1s orbital ($n=1, l=0, m=0$).

The defining characteristic of an $l=0$ (or "s") orbital is that it is **perfectly spherically symmetric**. It looks exactly the same no matter which direction you look at it from. It is a perfect, fuzzy sphere.

Because space is perfectly symmetric for this electron, there is absolutely no physical reason for the electron to "prefer" the x-axis over the y-axis, or the z-axis. The probability distribution is identical in all three directions.

Mathematically, this means the expectation values for the coordinates must all be perfectly equal:

$$\langle x^2 \rangle = \langle y^2 \rangle = \langle z^2 \rangle$$

### Step 4: Putting It All Together

We are now ready for the final step. Let's take our equation from Step 2:

$$\langle r^2 \rangle = \langle x^2 \rangle + \langle y^2 \rangle + \langle z^2 \rangle$$

Since we established in Step 3 that $\langle y^2 \rangle$ and $\langle z^2 \rangle$ are exactly the same thing as $\langle x^2 \rangle$, we can just substitute $\langle x^2 \rangle$ in for all of them:

$$\langle r^2 \rangle = \langle x^2 \rangle + \langle x^2 \rangle + \langle x^2 \rangle$$

$$\langle r^2 \rangle = 3\langle x^2 \rangle$$

Finally, we just divide both sides by $3$ to isolate $\langle x^2 \rangle$:

$$\langle x^2 \rangle = \frac{\langle r^2 \rangle}{3}$$

---

**Summary for your exam paper:**

You don't need to write an essay on the exam. A perfect, full-credit answer would look something like this:

> _In 3D Cartesian coordinates, $r^2 = x^2 + y^2 + z^2$, so linearly, $\langle r^2 \rangle = \langle x^2 \rangle + \langle y^2 \rangle + \langle z^2 \rangle$. Because the ground state (1s orbital) is perfectly spherically symmetric, the electron distribution is identical in all spatial directions, meaning $\langle x^2 \rangle = \langle y^2 \rangle = \langle z^2 \rangle$. Substituting this yields $\langle r^2 \rangle = 3\langle x^2 \rangle$, which rearranges to $\langle x^2 \rangle = \langle r^2 \rangle / 3$._

Isn't it wonderful how recognizing symmetry can save us from doing pages of complicated integral math?

Would you like to look at the next part of the problem, or should we review any of the coordinate system concepts first?