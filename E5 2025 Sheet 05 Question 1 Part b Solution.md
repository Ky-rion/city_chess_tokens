

![[Pasted image 20260128114236.png]]

Hello again! It is great to see you continuing with the design. We have built the _thickness_ of our detector onion, and now we need to decide how _long_ to make the tube.

In Part (b), we are calculating the length of the **Tracking Detector cylinder**.

To do this, we have to use some trigonometry. We are essentially asking: "How long does this tube need to be so that a particle flying out at a specific angle hits the side of the tube instead of flying out the open end?"

Here is the step-by-step breakdown.

---

### 1. The Geometry of the Problem

Imagine the detector is a soda can.

-   The collision happens in the exact center of the can.
    
-   If a particle flies out at $90^\circ$ (straight up), it definitely hits the side (the "barrel").
    
-   If a particle flies out at a very shallow angle (close to the horizontal axis), it might miss the barrel and fly out the flat ends (the "endcaps").
    

We want to make the barrel long enough so that any particle with an angle $\cos \theta \le 0.7$ passes through the **full radius** of the tracking detector before it reaches the end of the cylinder.

### 2. Translating the German Diagram

In the solution image you provided, there is a small handwritten triangle. Here is what the labels mean:

-   **$R_{Strahl}$**: This is $R_{beam}$ (Strahl = Beam).
    
-   **$R_{Spur}$**: This is $R_{track}$ (Spur = Track).
    
-   **$L_{zylinder}/2$**: This is half the length of the cylinder.
    

We use **half** the length because the collision happens in the middle. We are calculating the distance from the center point to one end of the tube.

### 3. Step-by-Step Calculation

#### Step A: Find the Radius we need to cover

We need the particle to cross the _entire_ tracking detector. This means it must cross the beam pipe radius _plus_ the tracking detector thickness. We calculated these in Part (a).

$$R_{total} = R_{beam} + R_{track}$$

$$R_{total} = 0.02\text{ m} + 0.96\text{ m} = \mathbf{0.98\text{ m}}$$

#### Step B: Convert the "Cut-off" Angle

The problem gives us the condition: $\cos \theta \le 0.7$.

This number (0.7) represents the limit of our detector's coverage. We need to convert this cosine value into an actual angle ($\theta$) and then into a tangent value, because tangent relates the "opposite" side (Radius) to the "adjacent" side (Length).

1.  **Find the angle:**
    
    $$\theta_{max} = \arccos(0.7) \approx 45.57^\circ$$
    
    _(This matches the solution sheet, which rounds it to $45.6^\circ$)_
    
2.  **Find the Tangent:**
    
    $$\tan(45.6^\circ) \approx \mathbf{1.02}$$
    

#### Step C: The Trigonometry Equation

Now we look at the right-angled triangle formed by the particle's path.

-   **Opposite Side:** The Radius ($0.98\text{ m}$)
    
-   **Adjacent Side:** Half the Length ($L/2$)
    

Using the definition of tangent ($\tan = \frac{\text{Opposite}}{\text{Adjacent}}$):

$$\tan(\theta) = \frac{R_{total}}{L / 2}$$

#### Step D: Solve for L (Length)

We rearrange the formula to solve for $L$:

1.  Move $L/2$ to the left:
    
    $$\frac{L}{2} \cdot \tan(\theta) = R_{total}$$
    
2.  Isolate $L$:
    
    $$L = \frac{2 \cdot R_{total}}{\tan(\theta)}$$
    

Now, plug in our numbers:

$$L = \frac{2 \cdot 0.98\text{ m}}{1.02}$$

$$L = \frac{1.96\text{ m}}{1.02}$$

$$L \approx \mathbf{1.92\text{ m}}$$

---

### Conclusion

The cylinder of your tracking detector needs to be **1.92 meters long**.

This ensures that any particle flying out at an angle of roughly $45^\circ$ or steeper will pass through all 20 layers of your silicon tracker, allowing you to measure its momentum accurately. If the cylinder were shorter, these particles would escape out the ends before the tracker could finish measuring them!

Ready for the next part of the collider design?