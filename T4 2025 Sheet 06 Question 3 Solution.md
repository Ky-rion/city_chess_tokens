

Hello there! It is wonderful to have you in my "office hours." This particular problem—the physics of ice skating—is one of my absolute favorites because it completely shatters a myth that many of us were told in grade school.

We often hear: "Ice skates slide because the high pressure of the blade melts the ice, creating a layer of water to glide on." It sounds intuitive, right? But as physicists, we don't trust intuition; we trust the equations!

Let’s look at "Aufgabe 3" (Task 3) and the handwritten solution you provided to see why this explanation simply doesn't hold water (pun intended).

### 1. The Tool: Clausius-Clapeyron Relation

To solve this, we need to understand how the melting temperature of a substance changes when we squeeze it (apply pressure). The mathematical tool for this is the Clausius-Clapeyron relation.

The handwritten notes begin by recalling this fundamental equality:

$$\frac{dP}{dT}\bigg|_{\text{coex}} = \frac{L}{T \Delta v}$$

Here is what these terms mean:

-   $\frac{dP}{dT}$: The slope of the phase boundary line. It tells us how much pressure ($P$) we need to apply to change the melting temperature ($T$) by one degree.
    
-   $L$: The Latent Heat (energy required to melt the ice).
    
-   $T$: The absolute temperature (freezing point, $273.15 \text{ K}$).
    
-   $\Delta v$: The change in specific volume between the two phases (liquid minus solid).
    

---

### 2. The Setup: Crunching the Numbers

Let's look at the data provided in the problem image and how the professor used it in the notes.

The Volume Anomaly

Water is weird. Usually, solids are denser than liquids. But ice is less dense than water (that's why ice cubes float!).

-   Specific volume of liquid water: $v_{\text{liq}} \approx 1.000 \text{ cm}^3/\text{g}$.
    
-   Specific volume of ice: $v_{\text{solid}} \approx 1.091 \text{ cm}^3/\text{g}$.
    

So, the change in volume is negative:

$$\Delta v = v_{\text{liq}} - v_{\text{solid}} = 1.000 - 1.091 = -0.091 \text{ cm}^3/\text{g}$$

Because $\Delta v$ is negative, the slope $\frac{dP}{dT}$ will be negative. This confirms that increasing pressure does lower the melting point. But the question is: by how much?

Calculating the Slope

The solution substitutes the values into the Clausius-Clapeyron equation. We must be careful with units (converting grams to kilograms or $\text{cm}^3$ to $\text{m}^3$ to match Pascals).

Using the values from the notes:

$$\frac{dP}{dT} \approx \frac{1}{273.15 \text{ K}} \cdot \frac{334.72 \text{ J/g}}{-0.091 \cdot 10^{-6} \text{ m}^3/\text{g}}$$

The calculation yields a massive number:

$$\frac{dP}{dT} \approx -13.47 \times 10^6 \text{ Pa/K}$$

---

### 3. The Interpretation: What does this number mean?

This result is the "smoking gun." It tells us that to lower the melting point of ice by just 1 Kelvin (or 1°C), you must increase the pressure by approximately 13.5 million Pascals (or about 135 Bar).

The notes rewrite this as:

$$\Delta P \approx 1347 \frac{\text{N}}{\text{cm}^2} \text{ per degree Kelvin}$$

---

### 4. The Reality Check: Can a skater do this?

Now, we do a "back-of-the-envelope" calculation to see if a human skater can generate this kind of pressure.

The Scenario

Imagine you want to go skating on a day when it is $-1^\circ\text{C}$ outside (which is actually quite warm for winter; usually it is colder, like $-5^\circ\text{C}$ or $-10^\circ\text{C}$). To melt the ice solely by pressure, you need to lower the melting point by at least $1 \text{ K}$.

According to our calculation, you need to exert 135 Bar of pressure on the ice.

The Example from the Solution

The professor's notes provide a stark example to illustrate the absurdity of this.

If your skate blade has a contact area of roughly $10 \text{ cm}^2$ (a reasonable estimate for a blade flat on the ice), and you need to generate $1347 \text{ N/cm}^2$ of pressure:

$$\text{Force required} = \text{Pressure} \times \text{Area} = 1347 \frac{\text{N}}{\text{cm}^2} \times 10 \text{ cm}^2 = 13,470 \text{ N}$$

Since Force $= mass \times gravity$ ($F=mg$), the mass required is:

$$m \approx \frac{13470}{9.81} \approx 1373 \text{ kg}$$

### Conclusion

To melt ice at just $-1^\circ\text{C}$ via pressure, a skater would need to weigh over 1,000 kg (a metric ton)! Since typical skaters weigh around $70\text{ kg}$, they generate nowhere near enough pressure to melt the ice, especially if it is $-5^\circ\text{C}$ or $-10^\circ\text{C}$ outside.

Therefore, the "pressure melting" explanation is incorrect. (The real reason involves friction heating and a "pre-melting" liquid-like layer that exists naturally on ice surfaces, but that's a story for another lecture!).

Would you like me to walk you through the math of the unit conversions (like cm³/g to m³/kg) to ensure you are comfortable with those steps?