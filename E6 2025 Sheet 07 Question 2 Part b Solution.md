

![[Pasted image 20260125185459.png]]

Excellent! Let's tackle part (b). This is where we apply the "secret code" logic to real shapes.

The goal here is to find the **Miller Indices** `(h k l)` for the orange planes shown in the pictures.

### The "Recipe" for Miller Indices

Before we look at the specific images, here is the 3-step recipe you will always use:

1.  **Find Intercepts:** Where does the plane cut the axes $x, y, z$ (or $a, b, c$)? Write these down in terms of unit lengths (e.g., $1$, $1/2$, $\infty$).
    
2.  **Invert:** Take the reciprocal of each number ($1/x$).
    
3.  **Reduce:** If you have fractions, clear them to get the smallest whole numbers.
    

> **Crucial Rule:** If a plane is **parallel** to an axis, it never touches it. Mathematically, we say the intercept is at infinity ($\infty$). The reciprocal of infinity ($1/\infty$) is **0**.

---

### Step-by-Step Solutions

Let's analyze the images from left to right, assuming the origin $(0,0,0)$ is at the **back-left-bottom** corner of the cube.

#### 1. The First Crystal: (101)

-   **Visual Check:** The orange plane looks like a ramp. It touches the front-bottom edge and goes up to the back-top edge.
    
-   **The Intercepts:**
    
    -   **a-axis (front):** The plane cuts the $a$-axis at **1** unit length (the front-left corner).
        
    -   **b-axis (side):** The plane runs parallel to the side-to-side direction. It never gets closer to or further from the right wall. Intercept = **$\infty$**.
        
    -   **c-axis (up):** The plane cuts the vertical $c$-axis at the top (height of **1**).
        
-   **Calculation:**
    
    1.  Intercepts: $1, \infty, 1$
        
    2.  Invert: $1/1, 1/\infty, 1/1$
        
    3.  Result: **(1 0 1)**
        

#### 2. The Second Crystal: (002)

-   **Visual Check:** This is a flat sheet hovering in the middle of the crystal.
    
-   **The Intercepts:**
    
    -   **a-axis:** Parallel (never touches). Intercept = **$\infty$**.
        
    -   **b-axis:** Parallel (never touches). Intercept = **$\infty$**.
        
    -   **c-axis:** Look closely. The plane passes right through the central atom. In a body-centered structure, that central atom is exactly in the middle. So, it cuts the vertical axis at **$1/2$**.
        
-   **Calculation:**
    
    1.  Intercepts: $\infty, \infty, 1/2$
        
    2.  Invert: $0, 0, 2$ (since $1 / (1/2) = 2$)
        
    3.  Result: **(0 0 2)**
        

> **Professor's Note:** You might wonder, "Why isn't it (001)?" If the plane were at the very top of the box, it would be (001). Since this plane cuts the spacing in _half_, the index doubles to 2. Higher indices = planes are closer together!

#### 3. The Third Crystal: (110)

-   **Visual Check:** This is a vertical wall cutting diagonally across the room.
    
-   **The Intercepts:**
    
    -   **a-axis:** The plane cuts through the front-left vertical edge. That is $a=$ **1**.
        
    -   **b-axis:** The plane cuts through the back-right vertical edge. That is $b=$ **1**.
        
    -   **c-axis:** The plane is a vertical wall; it shoots straight up parallel to the $c$-axis. Intercept = **$\infty$**.
        
-   **Calculation:**
    
    1.  Intercepts: $1, 1, \infty$
        
    2.  Invert: $1/1, 1/1, 0$
        
    3.  Result: **(1 1 0)**
        

#### 4. The Fourth Crystal: (112)

-   **Visual Check:** This is a triangle. It looks like the previous diagonal wall, but it has been tipped over so it hits the back wall halfway up.
    
-   **The Intercepts:**
    
    -   **a-axis:** Touches the front-left corner ($a=$ **1**).
        
    -   **b-axis:** Touches the back-right corner ($b=$ **1**).
        
    -   **c-axis:** Look at the label in the diagram. It explicitly says **"c/2"**. This means the plane intersects the back vertical axis exactly halfway up. Intercept = **$1/2$**.
        
-   **Calculation:**
    
    1.  Intercepts: $1, 1, 1/2$
        
    2.  Invert: $1/1, 1/1, 2$
        
    3.  Result: **(1 1 2)**
        

---

### Summary Verification

The professor's solution image confirms our derivations:

-   Left: **(101)**
    
-   Middle-Left: **(002)**
    
-   Middle-Right: **(110)**
    
-   Right: **(112)**
    

**Next Step for you:**

Just to verify you are comfortable with the "Invert" step: If I had a plane that cut the axes at $a=1$, $b=2$, and $c=3$, what would the Miller Indices be? (Hint: You will need to find a common denominator!)