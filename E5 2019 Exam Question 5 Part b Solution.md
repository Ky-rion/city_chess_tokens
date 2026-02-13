

![[Pasted image 20260209163934.png]]

Welcome back! Excellent job making it through part (a). You've grasped the total cross-section, which tells us _if_ a collision happens. But in particle physics, we usually want to know much more than that. We want to know exactly _where_ the particles bounce after they hit!

That brings us to part (b). Let's translate the problem and unpack this beautiful bit of geometry.

### The Problem Translated

> **Problem Statement (b):** Provide the differential cross-section $\frac{d\sigma}{d\theta}$. To do this, first determine the relationship between the impact parameter $b$ and the scattering angle $\theta$ using a sketch. The result can be simplified using the formula $\sin(2x) = 2\sin(x)\cos(x)$.

### Key Concepts Before We Begin

To understand the professor's solution, we need three new vocabulary words:

1. **Impact Parameter ($b$):** Imagine aiming a pool cue at a billiard ball. If you aim dead center, $b = 0$. If you aim slightly off-center, $b$ is the distance between your aiming line and the center line. It's how "off-center" the incoming projectile is.
    
2. **Scattering Angle ($\theta$):** This is the angle at which the projectile deflects away from its original straight-line path after the collision.
    
3. **Differential Cross-Section ($\frac{d\sigma}{d\theta}$):** In part (a), we found the _total_ target area ($\sigma$). The differential cross-section is like slicing that total area into tiny rings. It tells us how a tiny change in the target area ($d\sigma$) corresponds to a tiny change in the scattering angle ($d\theta$). It answers the question: "If I throw a particle at this specific spot, at what angle will it bounce away?"
    

---

### Walking Through the Solution

Let's break down the mathematical solution step-by-step.

#### Step 1: The Geometry of the Bounce

The solution starts by defining the geometry:

> _Sketch with two touching circles with radii $r$ and $R$, impact parameter $b$, and scattering angle $\theta$._
> 
> _Angle to the normal of the sphere surfaces: $\alpha \Rightarrow$ Scattering angle $\theta = \pi - 2\alpha \Rightarrow \alpha = (\pi - \theta)/2$_

Imagine the exact moment the small sphere ($r$) strikes the large sphere ($R$). Draw a straight line connecting their centers. This is called the **normal line**.

When the projectile hits, it bounces off this normal line just like light reflecting off a mirror: the angle of incidence equals the angle of reflection. Let's call this angle $\alpha$.

Because a straight line is $180^\circ$ (or $\pi$ radians), the angle of deflection ($\theta$) plus the incoming angle and outgoing angle ($2\alpha$) must add up to $\pi$.

Therefore: $\theta + 2\alpha = \pi$.

If we rearrange this to solve for $\alpha$, we get:

$$\alpha = \frac{\pi - \theta}{2}$$

#### Step 2: Connecting Impact Parameter ($b$) to the Angle ($\theta$)

> _$\sin\alpha = b/(r+R)$_
> 
> _$\Rightarrow b = (r+R)\sin((\pi-\theta)/2) = (r+R)\cos(\theta/2)$_

If you draw a right triangle where the hypotenuse connects the centers of the two spheres at impact (length = $r + R$), the opposite side of that triangle is the impact parameter $b$. Using basic trigonometry (SOH CAH TOA):

$$\sin(\alpha) = \frac{\text{Opposite}}{\text{Hypotenuse}} = \frac{b}{r+R}$$

Now, we substitute the $\alpha$ we found in Step 1:

$$b = (r+R)\sin\left(\frac{\pi - \theta}{2}\right)$$

In trigonometry, there is a handy identity: $\sin(\frac{\pi}{2} - x) = \cos(x)$. Using this, the equation beautifully simplifies to:

$$b = (r+R)\cos\left(\frac{\theta}{2}\right)$$

_This is the crucial relationship between how off-center you aim ($b$) and how much the particle deflects ($\theta$)._

#### Step 3: Taking the Derivative

> _$\frac{db}{d\theta} = -(r+R)/2 \sin(\theta/2)$_

To find the differential cross-section, we need to know how fast $b$ changes as $\theta$ changes. We do this by taking the derivative of our equation from Step 2 with respect to $\theta$.

The derivative of $\cos(\theta/2)$ is $-\frac{1}{2}\sin(\theta/2)$. So:

$$\frac{db}{d\theta} = -\frac{1}{2}(r+R)\sin\left(\frac{\theta}{2}\right)$$

#### Step 4: Putting it Together

> _$d\sigma = 2\pi b \, db$_
> 
> _$\frac{d\sigma}{d\theta} = 2\pi b \left| \frac{db}{d\theta} \right|$_

Think of the target area like a bullseye. A tiny ring on that bullseye has a circumference of $2\pi b$ and a thickness of $d b$. So, the area of that tiny ring is $d\sigma = 2\pi b \, db$.

To find $\frac{d\sigma}{d\theta}$, we divide both sides by $d\theta$. We use the absolute value $\left| \frac{db}{d\theta} \right|$ because an area ($d\sigma$) must always be a positive number, even if the derivative is negative (which just means as the angle gets bigger, the impact parameter gets smaller).

Now, we just plug in our $b$ from Step 2, and our absolute derivative from Step 3:

$$\frac{d\sigma}{d\theta} = 2\pi \cdot \left[ (r+R)\cos\left(\frac{\theta}{2}\right) \right] \cdot \left[ \frac{1}{2}(r+R)\sin\left(\frac{\theta}{2}\right) \right]$$

Group the terms together:

$$\frac{d\sigma}{d\theta} = \pi (r+R)^2 \cos\left(\frac{\theta}{2}\right)\sin\left(\frac{\theta}{2}\right)$$

#### Step 5: The Final Simplification

> _$= \pi(r+R)^2 \cos(\theta/2)\sin(\theta/2) = \frac{\pi}{2}(r+R)^2 \sin\theta$_

The problem gave us a helpful hint: $\sin(2x) = 2\sin(x)\cos(x)$.

If we divide that by 2, we get: $\sin(x)\cos(x) = \frac{1}{2}\sin(2x)$.

If we let $x = \theta/2$, we can apply this identity to our equation:

$$\cos\left(\frac{\theta}{2}\right)\sin\left(\frac{\theta}{2}\right) = \frac{1}{2}\sin(\theta)$$

Substitute that back into our big equation, and we arrive at the final, beautifully elegant answer:

$$\frac{d\sigma}{d\theta} = \frac{\pi}{2}(r+R)^2 \sin(\theta)$$

---

And there you have it! You've just calculated how particles map out into space after scattering off a hard sphere.

Are you ready to tackle part (c), or would you like to discuss what this final equation tells us physically about where the particles end up?