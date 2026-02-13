

![[Pasted image 20260209163917.png]]

Welcome to the fascinating world of particle physics! It is absolutely fantastic that you are diving into this material, and there is no better place to start than understanding the concept of a **scattering cross-section**.

Let's break down this problem together, step-by-step, just like we would in my office hours.

First, let's translate what the problem is asking us to do. The German text states:

> _"Spheres with a radius of $r = 1\text{ nm}$ are scattered on a sphere with radius $R = 5\text{ nm}$. Projectiles and target are spinless and undeformable."_
> 
> **(a) What is the total cross-section in barn?**

Here is exactly how the other professor arrived at the solution you provided.

---

### 1. Understanding the "Cross-Section" ($\sigma$)

In particle physics, when we shoot a beam of particles (projectiles) at a target, we want to know the probability that a collision will happen. We measure this probability as an effective area called the **cross-section**, denoted by the Greek letter $\sigma$ (sigma).

Imagine you are throwing darts randomly at a wall. If there is a balloon on the wall, the probability of hitting the balloon depends purely on its cross-sectional area (a circle, $\pi R^2$). If you double the area of the balloon, you double your chances of hitting it.

### 2. The Formula: Why $\sigma = \pi(r + R)^2$?

In our problem, we are dealing with "undeformable" (hard) spheres. This is what we call **classical hard-sphere scattering**.

If our incoming projectiles were tiny little point particles (radius $r = 0$), the target they need to hit would just be the cross-sectional area of the big sphere, which is $\pi R^2$.

However, our projectiles also have a physical size ($r = 1\text{ nm}$).

Think about when a collision actually happens. A collision occurs the exact moment the _edge_ of the projectile touches the _edge_ of the target. Geometrically, this happens when the **center of the projectile** comes within a distance of exactly $r + R$ from the **center of the target**.

Because of this, we can mathematically pretend that our incoming projectile is just a tiny point particle, as long as we artificially "inflate" the size of the target sphere by the radius of the projectile!

So, the effective radius of our target is $(r + R)$. The area of this effective target—our total cross-section—is therefore a circle with that new radius:

$$\sigma = \pi(r + R)^2$$

### 3. Plugging in the Numbers

Now let's do the math, which will match your solution key exactly.

- Projectile radius: $r = 1\text{ nm} = 10^{-9}\text{ m}$
    
- Target radius: $R = 5\text{ nm} = 5 \cdot 10^{-9}\text{ m}$
    
- Effective radius: $r + R = 6\text{ nm} = 6 \cdot 10^{-9}\text{ m}$
    

Let's plug this into our formula:

$$\sigma = \pi \cdot (6 \cdot 10^{-9}\text{ m})^2$$

$$\sigma = \pi \cdot 36 \cdot 10^{-18}\text{ m}^2$$

Since $\pi \approx 3.14159$, we multiply:

$$\sigma \approx 113.097 \cdot 10^{-18}\text{ m}^2$$

To put this in standard scientific notation, we move the decimal point two places to the left:

$$\sigma = 1.13 \cdot 10^{-16}\text{ m}^2$$

_(This matches the first part of your professor's solution perfectly!)_

### 4. What on earth is a "barn" (b)?

The question specifically asks for the answer in **barns**.

In particle and nuclear physics, atomic nuclei are incredibly tiny, so using square meters is very clumsy (you end up with huge negative exponents). During the Manhattan Project in the 1940s, physicists needed a unit for the cross-sectional area of a uranium nucleus. A uranium nucleus has a cross-sectional area of roughly $10^{-28}\text{ m}^2$.

To the physicists shooting neutrons at it, this nucleus was considered relatively "huge"—so big, they joked, it was like "hitting the broad side of a barn." The name stuck!

Therefore, the conversion factor is:

$$1\text{ barn (b)} = 10^{-28}\text{ m}^2$$

To convert our answer from square meters to barns, we divide by this factor:

$$\text{Area in barns} = \frac{1.13 \cdot 10^{-16}\text{ m}^2}{10^{-28}\text{ m}^2/\text{b}}$$

$$\text{Area in barns} = 1.13 \cdot 10^{-16} \cdot 10^{28}\text{ b}$$

$$\text{Area in barns} = 1.13 \cdot 10^{12}\text{ b}$$

And there we have it! The target is quite massive on the particle physics scale, giving us a very large cross-section of over a trillion barns.

---

How does that feel so far? Would you like me to clarify the geometry of the collision, or are you ready for us to tackle the next part of the problem?



[Somehow I ended up with two answers at the same time]

Welcome to the fascinating world of particle physics! I am absolutely thrilled to have you in my class. Everyone has to start somewhere, and a classical scattering problem like this is the perfect springboard before we dive into the really weird quantum stuff later in the semester.

Let's break down the German text, unpack the physics concepts, and walk through my colleague's solution step-by-step.

### The Problem Translated

First, let's understand exactly what the setup is:

> **Problem Statement:** Spheres with a radius of $r = 1\text{ nm}$ are scattered against a target sphere with a radius of $R = 5\text{ nm}$. The projectiles and the target are spinless and undeformable (rigid).
> 
> **Question (a):** What is the total cross-section in barn?

In physics terms, we are dealing with **"hard-sphere scattering."** Imagine throwing a billiard ball (the projectile) at a slightly larger bowling ball (the target). Because they are "undeformable," they bounce off each other perfectly without squishing.

### What is a "Cross-Section"?

Before looking at the math, you need to know what a **cross-section** (denoted by the Greek letter sigma, $\sigma$) is.

If you are throwing a dart at a dartboard, the "cross-section" is simply the surface area of the dartboard. The bigger the area, the higher the probability you will hit it. In particle physics, the cross-section is a measure of the **probability that a collision will occur**. It is expressed as an area.

Here is the trick: The effective "target area" doesn't just depend on the size of the target; it _also_ depends on the size of the projectile.

### Breaking Down the Solution

My colleague provided this solution key:

> $\sigma = \pi(r + R)^2 = 1.13 \cdot 10^{-16}\text{ m}^2 = 1.13 \cdot 10^{12}\text{ b}$

Let's see exactly how they arrived at these numbers.

**1. The Formula:** $\sigma = \pi(r + R)^2$

If you throw a tiny, point-like laser beam at our target sphere ($R$), the target area is just the cross-sectional circle of the target: $\pi R^2$.

However, our projectile is _not_ a point; it has its own radius, $r$. For a collision to happen, the projectiles don't have to hit dead center. They just need to _barely touch_ the outside of the target. A collision occurs as long as the center of the projectile comes within a distance of $r + R$ from the center of the target.

Therefore, the effective target area—the total cross-section—is a circle with a radius of $(r + R)$. The area of that circle is exactly the formula my colleague used!

**2. The Calculation in Square Meters**

Let's plug in our numbers. First, we must convert nanometers ($\text{nm}$) into standard SI units, which are meters ($\text{m}$). The prefix "nano" means $10^{-9}$.

- Projectile radius: $r = 1 \times 10^{-9}\text{ m}$
    
- Target radius: $R = 5 \times 10^{-9}\text{ m}$
    
- Collision radius: $r + R = 6 \times 10^{-9}\text{ m}$
    

Now, we square that and multiply by pi ($\pi$):

$$\sigma = \pi \cdot (6 \times 10^{-9}\text{ m})^2$$

$$\sigma = \pi \cdot 36 \times 10^{-18}\text{ m}^2$$

$$\sigma \approx 1.13097 \times 10^{-16}\text{ m}^2$$

If we round to two decimal places, we get **$1.13 \times 10^{-16}\text{ m}^2$**, which matches the professor's first checkpoint perfectly.

**3. Converting to "Barns"**

The problem asks for the answer in **barn** (abbreviated as **b**).

You might be wondering, "What on earth is a barn?" It's a bit of physics humor! During the top-secret Manhattan Project in World War II, physicists needed a unit of area to describe how likely a uranium nucleus was to capture a neutron. The uranium nucleus is actually quite large on a subatomic scale. The physicists joked that hitting it was as easy as "hitting the broad side of a barn." The name stuck!

By definition, one barn is equal to:

$$1\text{ b} = 10^{-28}\text{ m}^2$$

To convert our answer from square meters into barns, we divide our result by the size of a barn:

$$\sigma \text{ (in barns)} = \frac{1.13 \times 10^{-16}\text{ m}^2}{10^{-28}\text{ m}^2/\text{b}}$$

When dividing exponents, you subtract the bottom number from the top number: $(-16) - (-28) = 12$.

$$\sigma = 1.13 \times 10^{12}\text{ b}$$

And there we have it! The final answer is **$1.13 \times 10^{12}\text{ barns}$**. Because we are dealing with whole atoms/nanoparticles here rather than tiny atomic nuclei, the cross-section is an absolutely massive number of barns.

---

How do you feel about this foundational concept? Would you like me to translate the next part of the problem so we can look at what happens to the scattering angles?