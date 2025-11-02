

This is a great question, as it forces us to use a completely different method to (hopefully!) get the same result. The prompt is asking us to solve $\int \frac{1}{y} dx$ by making _x_ our integration variable, rather than introducing a new parameter $t$.

The result is indeed the same: **$I(z_0) = -2\pi$**.

Let's see how this alternative method works.

---

### 1. 🎯 The Strategy: Integrate with Respect to $x$

Instead of parameterizing everything with $t$, the prompt tells us to "integrate directly over $dx$." This means we need to:

1.  Express $y$ as a function of $x$.
    
2.  Integrate the resulting expression with respect to $x$ over the path.
    

From (1.b), we know our path $\gamma(z_0)$ is a circle defined by $x^2 + y^2 + z^2 = 1$ and $z = z_0$.

Let's simplify this by setting $R = \sqrt{1 - (z_0)^2}$. Our path is the circle $x^2 + y^2 = R^2$.

If we solve for $y$, we get:

$$y = \pm \sqrt{R^2 - x^2}$$

### 2. ↔️ Step 2: Splitting the Path

Here's the tricky part: a single function $y(x)$ cannot describe the _entire_ closed circle.

-   $y = +\sqrt{R^2 - x^2}$ describes the **top half** of the circle.
    
-   $y = -\sqrt{R^2 - x^2}$ describes the **bottom half** of the circle.
    

To integrate over the full closed loop $\gamma(z_0)$, we must split the integral into two pieces. Let's assume our path $\gamma(z_0)$ travels in the standard counter-clockwise direction (as we did in 1.b):

1.  **Top Path ($\gamma_{top}$):** The path goes along the top half $y = +\sqrt{R^2 - x^2}$. Here, $x$ moves from the rightmost point ($x=R$) to the leftmost point ($x=-R$).
    
2.  **Bottom Path ($\gamma_{bottom}$):** The path continues along the bottom half $y = -\sqrt{R^2 - x^2}$. Here, $x$ moves from the leftmost point ($x=-R$) back to the rightmost point ($x=R$).
    

### 3. 🧮 Step 3: Setting up and Solving the Integrals

The total integral is the sum of the integrals over these two paths:

$$I(z_0) = \int_{\gamma(z_0)} \frac{1}{y} dx = \int_{\gamma_{top}} \frac{1}{y} dx + \int_{\gamma_{bottom}} \frac{1}{y} dx$$

Now, let's substitute the expressions for $y$ and the correct integration bounds for $x$:

-   For $\gamma_{top}$:
    
    $$\int_{\gamma_{top}} \frac{1}{y} dx = \int_{x=R}^{x=-R} \frac{1}{+\sqrt{R^2 - x^2}} dx$$
    
-   For $\gamma_{bottom}$:
    
    $$\int_{\gamma_{bottom}} \frac{1}{y} dx = \int_{x=-R}^{x=R} \frac{1}{-\sqrt{R^2 - x^2}} dx$$
    
    Let's add them together:
    
    $$I(z_0) = \int_{R}^{-R} \frac{1}{\sqrt{R^2 - x^2}} dx + \int_{-R}^{R} -\frac{1}{\sqrt{R^2 - x^2}} dx$$
    
    We can flip the integration bounds of the first integral, which adds a minus sign:
    
    $$I(z_0) = -\int_{-R}^{R} \frac{1}{\sqrt{R^2 - x^2}} dx - \int_{-R}^{R} \frac{1}{\sqrt{R^2 - x^2}} dx$$
    
    Now both integrals are identical. We can combine them:
    
    $$I(z_0) = -2 \int_{-R}^{R} \frac{1}{\sqrt{R^2 - x^2}} dx$$
    
    This is a famous standard integral. The antiderivative of $\frac{1}{\sqrt{R^2 - x^2}}$ is $\arcsin\left(\frac{x}{R}\right)$.
    

## Now we just apply the bounds $x=-R$ and $x=R$. (This is where we use the hint that "$dx$ is a total differential"—it's the justification for using the Fundamental Theorem of Calculus):

$$I(z_0) = -2 \left[ \arcsin\left(\frac{x}{R}\right) \right]_{-R}^{R}$$

$$I(z_0) = -2 \left( \arcsin\left(\frac{R}{R}\right) - \arcsin\left(\frac{-R}{R}\right) \right)$$

$$I(z_0) = -2 \left( \arcsin(1) - \arcsin(-1) \right)$$

We know that $\arcsin(1) = \frac{\pi}{2}$ and $\arcsin(-1) = -\frac{\pi}{2}$.

$$I(z_0) = -2 \left( \frac{\pi}{2} - \left(-\frac{\pi}{2}\right) \right)$$

$$I(z_0) = -2 \left( \frac{\pi}{2} + \frac{\pi}{2} \right)$$

$$I(z_0) = -2 (\pi)$$

$$I(z_0) = -2\pi$$

### 💡 Conclusion

Once again, we get the exact same answer!

This confirms our result from (1.b) using a completely different calculation. Both methods show that the integral is **$-2\pi$**, a non-zero constant that is independent of the specific circle $z_0$ we choose. This is a very powerful and (as you said) baffling result, and it's a perfect example of what makes this area of physics and math so interesting.

This result is a key building block for more advanced concepts like Stokes' Theorem.

Now, would you like to discuss _why_ this baffling result happens—why the integral is constant even when the path length changes?