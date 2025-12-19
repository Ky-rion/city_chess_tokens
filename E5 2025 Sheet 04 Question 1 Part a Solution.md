

Welcome to the fascinating world of nuclear physics! I am delighted to be your guide. Don't worry if this looks intimidating at first glance—it's essentially a giant accounting problem where the currency is energy instead of money.

We are going to look at how splitting a single uranium atom releases a tremendous amount of energy, and then we'll see what happens when we scale that up to just one gram of material.

Here is the step-by-step breakdown.

---

### Part 1: The Concept (The "Liquid Drop" Model)

To answer this, we need to use the **Bethe-Weizsäcker Formula**, also known as the **Semi-Empirical Mass Formula (SEMF)**.

Imagine the nucleus of an atom is like a drop of liquid.

1.  **Volume Term:** The more particles (nucleons) you have, the more "glue" (binding energy) holds them together.
    
2.  **Surface Term:** Particles on the surface don't have neighbors on all sides, so they are held less tightly. This reduces the binding energy.
    
3.  **Coulomb Term:** Protons are positively charged and hate being near each other. They try to push the nucleus apart, reducing binding energy.
    
4.  **Asymmetry Term:** Nuclei like to have an equal number of protons and neutrons. If the balance is off, the nucleus is less stable.
    
5.  **Pairing Term:** Protons and neutrons like to form pairs. (We will neglect this term for this estimation as its effect is small compared to the total energy).
    

The Formula:

The Binding Energy $B$ for a nucleus with Mass Number $A$ and Atomic Number $Z$ is roughly:

$$B(A, Z) = a_v A - a_s A^{2/3} - a_c \frac{Z(Z-1)}{A^{1/3}} - a_{sym} \frac{(A-2Z)^2}{A}$$

Since the problem asks for an estimate and doesn't provide specific constants, I will use a standard set found in most textbooks (like Krane's _Introductory Nuclear Physics_):

-   $a_v = 15.5$ MeV (Volume constant)
    
-   $a_s = 16.8$ MeV (Surface constant)
    
-   $a_c = 0.72$ MeV (Coulomb constant)
    
-   $a_{sym} = 23.0$ MeV (Symmetry constant)
    

_(Note: MeV stands for Mega-electron Volts, a unit of energy used in particle physics)._

---

### Part 2: Calculating the Binding Energies

The reaction is:

$${}^{235}_{92}\text{U} + n \rightarrow {}^{89}_{36}\text{Kr} + {}^{144}_{56}\text{Ba} + 3n$$

To find the energy released ($Q$), we calculate the total binding energy of the products (the stuff we made) and subtract the binding energy of the reactants (the stuff we started with).

$$Q = [B(\text{Kr}) + B(\text{Ba})] - B(\text{U})$$

(Note: Free neutrons 'n' have zero binding energy, so we ignore them in this step).

#### 1. Uranium-235 (${}^{235}_{92}\text{U}$)

-   $A = 235$, $Z = 92$
    
-   **Volume:** $15.5 \times 235 = 3642.5$
    
-   **Surface:** $16.8 \times (235)^{2/3} \approx 16.8 \times 38.06 \approx 639.4$
    
-   **Coulomb:** $0.72 \times \frac{92(91)}{235^{1/3}} \approx 0.72 \times \frac{8372}{6.17} \approx 976.8$
    
-   **Symmetry:** $23.0 \times \frac{(235 - 2(92))^2}{235} = 23.0 \times \frac{51^2}{235} \approx 254.5$
    

$$B(\text{U}) \approx 3642.5 - 639.4 - 976.8 - 254.5 = \mathbf{1771.8 \text{ MeV}}$$

#### 2. Krypton-89 (${}^{89}_{36}\text{Kr}$)

-   $A = 89$, $Z = 36$
    
-   **Volume:** $15.5 \times 89 = 1379.5$
    
-   **Surface:** $16.8 \times (89)^{2/3} \approx 16.8 \times 19.94 \approx 335.0$
    
-   **Coulomb:** $0.72 \times \frac{36(35)}{89^{1/3}} \approx 0.72 \times \frac{1260}{4.46} \approx 203.4$
    
-   **Symmetry:** $23.0 \times \frac{(89 - 72)^2}{89} = 23.0 \times \frac{289}{89} \approx 74.7$
    

$$B(\text{Kr}) \approx 1379.5 - 335.0 - 203.4 - 74.7 = \mathbf{766.4 \text{ MeV}}$$

#### 3. Barium-144 (${}^{144}_{56}\text{Ba}$)

-   $A = 144$, $Z = 56$
    
-   **Volume:** $15.5 \times 144 = 2232.0$
    
-   **Surface:** $16.8 \times (144)^{2/3} \approx 16.8 \times 27.49 \approx 461.8$
    
-   **Coulomb:** $0.72 \times \frac{56(55)}{144^{1/3}} \approx 0.72 \times \frac{3080}{5.24} \approx 423.2$
    
-   **Symmetry:** $23.0 \times \frac{(144 - 112)^2}{144} = 23.0 \times \frac{1024}{144} \approx 163.6$
    

$$B(\text{Ba}) \approx 2232.0 - 461.8 - 423.2 - 163.6 = \mathbf{1183.4 \text{ MeV}}$$

---

### Part 3: Total Energy Released per Reaction

Now we compare the "after" energy to the "before" energy.

-   **Total Binding Energy AFTER:** $766.4 \text{ (Kr)} + 1183.4 \text{ (Ba)} = 1949.8 \text{ MeV}$
    
-   **Total Binding Energy BEFORE:** $1771.8 \text{ MeV}$
    

$$Q = 1949.8 - 1771.8 = \mathbf{178 \text{ MeV}}$$

So, roughly 178 MeV of energy is released every time a single Uranium atom splits.

(Note: In precise experiments, the total energy is often cited around 200 MeV, so our estimate using the formula is quite accurate!)

---

### Part 4: Energy from 1 gram of Uranium-235

Now for the real-world application. How much energy is in 1 gram?

1. How many atoms are in 1 gram?

The molar mass of ${}^{235}\text{U}$ is $235 \text{ g/mol}$.

Using Avogadro's number ($N_A \approx 6.022 \times 10^{23}$):

$$\text{Number of atoms} = \frac{1 \text{ g}}{235 \text{ g/mol}} \times 6.022 \times 10^{23} \text{ atoms/mol} \approx 2.56 \times 10^{21} \text{ atoms}$$

2. Total Energy Calculation

Multiply the number of atoms by the energy per atom:

$$E_{total} = (2.56 \times 10^{21}) \times (178 \text{ MeV}) \approx 4.56 \times 10^{23} \text{ MeV}$$

3. Converting to Joules

This number is too big to make sense of in MeV. Let's convert to Joules ($1 \text{ MeV} = 1.602 \times 10^{-13} \text{ J}$).

$$E_{Joules} = (4.56 \times 10^{23}) \times (1.602 \times 10^{-13}) \approx \mathbf{7.3 \times 10^{10} \text{ Joules}}$$

### Final Answer Summary

-   **Energy per reaction:** Approximately **178 MeV**.
    
-   **Energy from 1g of U-235:** Approximately **$7.3 \times 10^{10}$ Joules**.
    

Just to give you perspective on how massive that is:

$7.3 \times 10^{10}$ Joules is roughly equivalent to burning 2.5 metric tons of coal. That is why nuclear energy is so incredibly dense—one gram of fuel does the work of a truckload of coal!

Would you like me to walk you through how the units of "MeV" are derived, or are you happy with this result?