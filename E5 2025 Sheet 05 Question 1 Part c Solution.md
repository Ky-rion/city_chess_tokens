

![[Pasted image 20260128114252.png]]

Excellent! We are now moving from the "onion" (cross-section) and the "tube" (cylinder length) to the full **3D assembly** of our detector.

In Part (c), we are putting the lids on our jar. In particle physics, these lids are called **"End Caps."**

We want to catch particles that fly out along the beam line (forward and backward), not just the ones that fly out sideways. To do this, we build huge plugs containing the same detectors we used in the barrel.

Here is the breakdown of the calculation.

---

### 1. The Geometry: Barrel + End Caps

Think of the detector as three distinct pieces connected together:

1.  **The Barrel:** This is the central cylinder we calculated in part (b). Its length is $L_{barrel} = 1.92\text{ m}$.
    
2.  **The Left End Cap:** A stack of detectors plugging the left side.
    
3.  **The Right End Cap:** A stack of detectors plugging the right side.
    

The total length of the detector ($L_{det}$) is simply the length of the barrel plus the thickness of both end caps.

$$L_{det} = L_{barrel} + 2 \times (\text{Thickness of one End Cap})$$

### 2. What is in the End Cap?

The problem states that the end caps consist of the **tracking chamber, calorimeter, and muon chamber**, exactly as in exercise (a).

This means we take the radial thickness ($R$) of each layer we calculated in part (a) and turn it into a longitudinal thickness ($L$) for the end caps.

**Crucial Detail:** We do **not** include the Beam Pipe ($R_{beam}$) in this sum. Why? Because the beam pipe is a long tube that runs through the _entire_ machine. The end caps are donut-shaped disks that slide _over_ the beam pipe; they don't cover it up (otherwise the beam couldn't get in!).

So, the thickness of one End Cap is the sum of:

-   **Tracking Detector:** $0.96\text{ m}$
    
-   **ECAL:** $0.23\text{ m}$
    
-   **HCAL:** $1.40\text{ m}$
    
-   **Muon Chamber:** $3.00\text{ m}$
    

### 3. The Calculation

Let's do the math step-by-step.

**Step A: Calculate the thickness of one End Cap**

$$\text{End Cap Thickness} = R_{track} + R_{ECAL} + R_{HCAL} + R_{muon}$$

$$\text{End Cap Thickness} = 0.96\text{ m} + 0.23\text{ m} + 1.40\text{ m} + 3.00\text{ m}$$

$$\text{End Cap Thickness} = \mathbf{5.59\text{ m}}$$

**Step B: Add the two End Caps to the Barrel**

We have a barrel in the middle ($1.92\text{ m}$) and a $5.59\text{ m}$ plug on _each_ side.

$$L_{det} = 1.92\text{ m} + 2 \times (5.59\text{ m})$$

$$L_{det} = 1.92\text{ m} + 11.18\text{ m}$$

$$L_{det} = \mathbf{13.1\text{ m}}$$

---

### Final Result

The total length of your collider detector is **13.1 meters**.

**Professor's Summary:**

You have now designed a complete particle detector!

-   **Radius:** $5.61\text{ meters}$ (from part a)
    
-   **Length:** $13.1\text{ meters}$ (from part c)
    

This is a massive machine—roughly 11 meters wide and 13 meters long. For context, this is fairly compact compared to the real CMS detector at CERN (which is $15\text{ m}$ wide and $21\text{ m}$ long), but it uses the exact same principles!

Would you like to review the whole design, or is there another question on your homework sheet?