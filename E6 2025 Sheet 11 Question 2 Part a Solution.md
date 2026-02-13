

![[Pasted image 20260206202352.png]]
![[Pasted image 20260206202538.png]]

Hello there! Welcome to our solid-state physics tutorial. I am delighted to step in as your professor for this session. It is excellent that you are starting with the basics of Brillouin Zones and Fermi surfaces—these are the absolute bread and butter of understanding electronic properties in metals.

Let's break down **Part (a)** of your problem. We are going to deconstruct the solution provided by the other professor (images `image_c8113d.png` and `image_c8117c.png`) and make sure you intuitively understand the geometry behind it.

### The Setup: The "Map" and the "Water"

To solve this, imagine we are working with a map and a bucket of water.

1. **The Map (Reciprocal Space):** This is the grid defined by the crystal lattice.
    
2. **The Water (Electrons):** This is the "Fermi sea" of electrons that we pour onto the map.
    

---

### Step 1: Constructing the Map (The Brillouin Zones)

First, look at **Figure a** in the solution image.

We start with a square lattice in real space with a lattice constant $a$. In solid-state physics, we always move to **reciprocal space** (k-space) to understand energy.

- For a square lattice, the reciprocal lattice is also a square lattice.
    
- The spacing between reciprocal lattice points is $b = \frac{2\pi}{a}$.
    

**How do we draw the zones?**

We use the **Wigner-Seitz construction** (bisecting lines between lattice points):

1. **1st Brillouin Zone (1. BZ):** This is the area enclosed by the perpendicular bisectors of the shortest lattice vectors. In **Figure a**, this is the central **Blue Square**. Its boundaries are at $k_x = \pm \frac{\pi}{a}$ and $k_y = \pm \frac{\pi}{a}$.
    
2. **2nd Brillouin Zone (2. BZ):** This is the area you reach by crossing the boundaries of the 1st zone. In **Figure a**, these are the four **Yellow Triangles** attached to the sides of the blue square.
    
3. **3rd Brillouin Zone (3. BZ):** This is the next layer out. In **Figure a**, these are the four **Green Squares** at the corners of the diagram.
    

Together, these zones tile the reciprocal space perfectly.

---

### Step 2: Pouring the Water (The Fermi Sphere)

Now we add the electrons. The problem states we have a **free electron gas**.

- **Energy Dispersion:** $E_k = \frac{\hbar^2 k^2}{2m}$. This means energy depends only on the magnitude of the momentum vector $|\vec{k}|$.
    
- **Shape:** Because energy depends only on distance from the center ($k$), the surface of constant energy (the Fermi Surface) is a **circle** (or a sphere in 3D).
    

**How big is the circle?**

The problem gives us the radius of this Fermi circle:

$$k_F = 1.2 \frac{\pi}{a}$$

This number, **1.2**, is crucial. Let's compare it to the geometry of our 1st Brillouin Zone (the blue square):

1. **Distance to the edge (face) of the square:** $\frac{\pi}{a}$ (Let's call this **1.0** units).
    
2. **Distance to the corner of the square:** Using Pythagoras, $\sqrt{1^2 + 1^2} \frac{\pi}{a} \approx 1.41 \frac{\pi}{a}$ (Let's call this **1.41** units).
    

**The Comparison:**

Our Fermi circle radius is **1.2**.

- It is **larger** than the distance to the edge ($1.2 > 1.0$).
    
- It is **smaller** than the distance to the corner ($1.2 < 1.41$).
    

**Visualizing Figure a:**

Look at the dashed circle in **Figure a**.

- Because $1.2 > 1.0$, the circle **bursts out** of the blue square. It crosses the boundaries. This means electrons "spill" into the **2nd Brillouin Zone** (the yellow triangles).
    
- Because $1.2 < 1.41$, the circle **does not reach** the corners of the blue square. This means the corners of the 1st Brillouin Zone are **empty** (no electrons there).
    
- Does it reach the **3rd Zone**? The 3rd zone starts further out. As the German text notes ("_jedoch nicht bis in die dritte hinein_"), the radius isn't large enough to reach the green areas.
    

---

### Step 3: The Reduced Zone Scheme (Figure b)

This is the part that often confuses students. The **Reduced Zone Scheme** is a way of organizing the information. Instead of drawing a huge map spreading out, we "fold" everything back into the first square (the first Brillouin Zone).

We treat each band separately.

#### **1. Band (First Box in Figure b)**

- **Concept:** This represents the electrons that fit inside the 1st Brillouin Zone.
    
- **Observation:** Recall that our circle covered the center of the blue square but **missed the corners**.
    
- **Result:** The 1st Band is mostly full (green), but has empty pockets at the corners (white).
    
- **Physics Lingo:** These empty corners act as "hole pockets." If you apply an electric field, conduction happens here via these holes.
    

#### **2. Band (Second Box in Figure b)**

- **Concept:** This represents the electrons that spilled over into the 2nd Brillouin Zone.
    
- **Observation:** In **Figure a**, the circle overlapped into the yellow triangles. These are four small "lens" shaped segments of the circle.
    
- **Translation:** In the reduced scheme, we shift these pieces by a reciprocal lattice vector ($2\pi/a$) to move them back into the central square.
    
    - The spill-over on the right shifts to the left edge.
        
    - The spill-over on the top shifts to the bottom edge.
        
- **Result:** You get the image labeled **"2.Band"**. It shows four small pockets of electrons centered on the edges of the square.
    
- **Physics Lingo:** These are "electron pockets."
    

#### **3. Band (Third Box in Figure b)**

- **Concept:** Did any electrons reach the 3rd zone?
    
- **Observation:** As we calculated, $k_F = 1.2 \pi/a$ was not big enough to reach the 3rd zone.
    
- **Result:** The box is completely white (empty). There are no electrons in the 3rd energy band.
    

---

### Summary Interpretation

So, if you were to look at this material:

1. **Band 1** is almost full (conducts via holes).
    
2. **Band 2** is slightly full (conducts via electrons).
    
3. **Band 3** is empty (insulator).
    

The diagram in **Figure b** perfectly summarizes this occupation using the reduced zone scheme, derived strictly from comparing the radius $k_F$ to the geometry of the square grid!

Does that distinction between the "Extended" view (Figure a) and the "Reduced" view (Figure b) make sense to you now?