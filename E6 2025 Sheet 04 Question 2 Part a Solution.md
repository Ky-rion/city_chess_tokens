

![[Pasted image 20260125183725.png]]
![[Pasted image 20260125183737.png]]

Hello there! Welcome to the fascinating world of Solid State Physics. I would be delighted to be your "professor" for this session. Don't let the graph scare you; looking at a diffractogram is a bit like looking at a fingerprint—once you know what to look for, it tells you exactly who the suspect is (or in this case, what the crystal is).

I want to start with a **very important observation** to save you a lot of confusion.

### ⚠️ The "Trap" in the Question

If you look closely at the first image, there are two conflicting sets of numbers:

1.  **Top Paragraph:** Says lattice constant $a = 2.87 \text{ \AA}$ and wavelength $\lambda = 1.54 \text{ \AA}$.
    
2.  **Bottom Line (Part a):** Says "Annahme" (Assumption): $a = 4.8 \text{ \AA}$ and $\lambda = 1.5 \text{ \AA}$.
    

**We must use the numbers at the bottom ($a = 4.8 \text{ \AA}$, $\lambda = 1.5 \text{ \AA}$).**

Why? Because if you try to use the top numbers, the math won't match the graph! The solution provided by the other professor also strictly uses these bottom numbers. It looks like the problem sheet might have had a typo or was reusing an old text block.

---

### The Goal: Assigning "Miller Indices" (hkl)

Our goal is to figure out which atomic planes in the crystal caused those spikes in the graph. We call these planes by their coordinate names, the **Miller Indices $(hkl)$**.

We will follow the three steps shown in the solution image.

#### Step 1: Read the Graph ($2\theta$)

The graph shows **Intensity** on the y-axis vs. **Diffraction Angle ($2\theta$)** on the x-axis.

-   The x-axis represents the angle between the X-ray source and the detector.
    
-   The spikes (peaks) happen only at specific "magic angles" where the X-rays bounce off atomic layers and reinforce each other.
    

If you look at the solution image (Table 1, column 1), the professor simply looked at the graph and noted the x-position of each spike:

-   Peak 1: $2\theta \approx 25^\circ$
    
-   Peak 2: $2\theta \approx 36^\circ$
    
-   Peak 3: $2\theta \approx 45^\circ$
    
-   ...and so on.
    

**Note:** For the math, we usually need just $\theta$, not $2\theta$. So, we divide all those numbers by 2 (Table 1, column 2).

-   Peak 1: $\theta = 12.5^\circ$
    

#### Step 2: Calculate the Layer Spacing ($d$)

This is where the most famous equation in this field comes in: **Bragg's Law**.

$$n\lambda = 2d \sin(\theta)$$

-   **$n$:** The order of diffraction. The problem tells us to assume $n=1$.
    
-   **$\lambda$:** The wavelength of the X-ray (the "ruler" we are measuring with). We are using **1.5 Å** (or 0.15 nm).
    
-   **$\theta$:** The angle we just found.
    
-   **$d$:** The distance between the layers of atoms. This is what we want to find!
    

Rearranging the formula to solve for $d$:

$$d = \frac{\lambda}{2 \sin(\theta)}$$

Let's try it for the **first peak** ($2\theta = 25^\circ$, so $\theta = 12.5^\circ$):

$$d = \frac{1.5 \text{ \AA}}{2 \cdot \sin(12.5^\circ)}$$

$$d = \frac{1.5}{2 \cdot 0.2164} \approx 3.46 \text{ \AA}$$

_Note: The solution image writes this as **0.346 nm**. Remember that $1 \text{ nm} = 10 \text{ \AA}$, so $0.346 \text{ nm}$ is the exact same thing as $3.46 \text{ \AA}$._

The professor repeated this for every peak to get the list of $d$-spacings: $0.346, 0.243, 0.196 \dots$ (in nm).

#### Step 3: Assigning the (hkl) Triplets

Now we have the "fingerprints" (the $d$ values). We need to match them to a specific suspect: the cubic crystal planes.

For a cubic crystal, geometry tells us the distance $d$ is related to the lattice constant $a$ (the size of the cube) and the Miller indices $(h,k,l)$ by this formula:

$$d_{hkl} = \frac{a}{\sqrt{h^2 + k^2 + l^2}}$$

We know $a = 4.8 \text{ \AA}$ (from the assumption at the bottom). We have the $d$ values calculated in Step 2. We need to find integers $h, k, l$ that make the equation work.

**Let's analyze the first peak:**

We calculated $d \approx 3.46 \text{ \AA}$ (or $0.346 \text{ nm}$).

Let's plug it into the formula:

$$3.46 = \frac{4.8}{\sqrt{h^2 + k^2 + l^2}}$$

Solving for the square root term:

$$\sqrt{h^2 + k^2 + l^2} = \frac{4.8}{3.46} \approx 1.39$$

If we square that, we get:

$$h^2 + k^2 + l^2 \approx (1.39)^2 \approx 1.93$$

Since $h, k,$ and $l$ must be integers (whole numbers like 0, 1, 2...), the sum of their squares must be an integer. $1.93$ is very close to **2**.

Which integers, when squared and added, equal 2?

The only combination is **1, 1, 0**. ($1^2 + 1^2 + 0^2 = 2$).

**Conclusion for Peak 1:** The Miller Index is **(110)**.

**Let's check Peak 2:**

-   $d \approx 2.43 \text{ \AA}$ ($0.243 \text{ nm}$)
    
-   $\sqrt{h^2+k^2+l^2} = \frac{4.8}{2.43} \approx 1.97$
    
-   Square that: $(1.97)^2 \approx 3.9$ which is basically **4**.
    
-   Which integers square to sum to 4? **(2, 0, 0)** because $2^2 + 0 + 0 = 4$.
    
-   **Conclusion for Peak 2:** The Miller Index is **(200)**.
    

---

### Professor's Insight: The "Hidden" Information

You might wonder, "Why did we start with (110)? Why wasn't the first peak (100)?"

If you tried (100), the math would be:

$d = 4.8 / \sqrt{1} = 4.8 \text{ \AA}$.

If you plug $d=4.8$ back into Bragg's law, you'd get an angle $2\theta$ of about $18^\circ$.

**Look at the graph.** Is there a peak at $18^\circ$? **No.** The graph is flat there.

This tells us something profound about the crystal structure. When certain expected peaks (like 100) are missing, it's due to **Extinction Rules**. The fact that our sequence of $h^2+k^2+l^2$ goes $2, 4, 6, 8, 10$ is a classic signature of a **Body-Centered Cubic (BCC)** lattice. (I know the question didn't ask that, but it's a bonus fact for you!).

**Summary of the Solution Table:**

1.  Read the angles from the graph.
    
2.  Use Bragg's Law ($n\lambda = 2d \sin\theta$) to get distances ($d$).
    
3.  Use the Cubic formula ($d = a / \sqrt{h^2+k^2+l^2}$) to find integer combinations of $h,k,l$ that fit.
    

Would you like to move on to the next part of the question, or would you like to verify the calculation for the 3rd peak together?