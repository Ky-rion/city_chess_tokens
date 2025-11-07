

This is an excellent question! It gets at what happens when the _first_ correction to the energy is zero.

First, let's look at our new conditions. The problem states we must now set **$D_1 = D_2 = 0$**.

Let's see what this does to our findings from part (c):

-   $E_1(\lambda) \approx a + \lambda E_1^{(1)} = a + \lambda (D_1) = a + 0$
    
-   $E_2(\lambda) \approx b + \lambda E_2^{(1)} = b + \lambda (D_2) = b + 0$
    

This tells us that to first order, the energies _don't change at all_! The diagonal terms $D_1$ and $D_2$ were responsible for the first-order shift. Since they are gone, the first change to the energy must appear at the _second order_ (the $\lambda^2$ term).

Our goal is to find the approximation:

$$E_n \approx E_n^{(0)} + \lambda E_n^{(1)} + \lambda^2 E_n^{(2)}$$

Since $E_n^{(1)} = 0$, we are looking for:

$$E_n \approx E_n^{(0)} + \lambda^2 E_n^{(2)}$$

We have two ways to solve this. Method 1 is to use the "official" formula from perturbation theory. Method 2 is to use the _hint_ given in the problem, which is a clever shortcut. Let's do both!

---

### Method 1: The Standard Perturbation Theory Formula

The general formula for the **second-order energy correction** $E_n^{(2)}$ for a non-degenerate state $n$ is:

$$E_n^{(2)} = \sum_{k \neq n} \frac{|\langle k^{(0)} | \hat{V} | n^{(0)} \rangle|^2}{E_n^{(0)} - E_k^{(0)}}$$

Let's break this down:

-   We sum over all other states $k$ that are not our state $n$. In our $2 \times 2$ system, this is easy: if $n=1$, the sum is just $k=2$. If $n=2$, the sum is just $k=1$.
    
-   $\hat{V}$ is our perturbation. With $D_1=D_2=0$, our perturbation matrix is now:
    
    $$\hat{V} = \begin{pmatrix} 0 & C^* \\ C & 0 \end{pmatrix}$$
    
-   The numerator $|\langle k^{(0)} | \hat{V} | n^{(0)} \rangle|^2$ is the squared magnitude of the "off-diagonal" matrix element. This term "connects" state $n$ to state $k$.
    
-   The denominator $E_n^{(0)} - E_k^{(0)}$ is the energy difference between the two unperturbed states.
    

This formula has a beautiful physical meaning: the second-order correction to state $n$ is caused by the perturbation "mixing" it with all other states $k$. The strength of this mixing depends on how strongly the perturbation connects the states (the numerator) and how far apart they are in energy (the denominator).

#### 1. Calculation for $E_1^{(2)}$ (the $\lambda^2$ correction to $a$)

-   $n=1$ and $k=2$
    
-   $E_1^{(0)} = a$ and $E_2^{(0)} = b$
    

$$E_1^{(2)} = \frac{|\langle 2^{(0)} | \hat{V} | 1^{(0)} \rangle|^2}{E_1^{(0)} - E_2^{(0)}} = \frac{|\langle 2^{(0)} | \hat{V} | 1^{(0)} \rangle|^2}{a - b}$$

Let's calculate the numerator's matrix element:

$$\langle 2^{(0)} | \hat{V} | 1^{(0)} \rangle = \begin{pmatrix} 0 & 1 \end{pmatrix} \begin{pmatrix} 0 & C^* \\ C & 0 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix}$$

$$\qquad = \begin{pmatrix} 0 & 1 \end{pmatrix} \left( \begin{pmatrix} 0 \\ C \end{pmatrix} \right) = (0 \cdot 0) + (1 \cdot C) = C$$

The numerator is then $|C|^2$.

So, the second-order correction is:

$E_1^{(2)} = \frac{|C|^2}{a - b}$

#### 2. Calculation for $E_2^{(2)}$ (the $\lambda^2$ correction to $b$)

-   $n=2$ and $k=1$
    
-   $E_2^{(0)} = b$ and $E_1^{(0)} = a$
    

$$E_2^{(2)} = \frac{|\langle 1^{(0)} | \hat{V} | 2^{(0)} \rangle|^2}{E_2^{(0)} - E_1^{(0)}} = \frac{|\langle 1^{(0)} | \hat{V} | 2^{(0)} \rangle|^2}{b - a}$$

Let's calculate the numerator's matrix element:

$$\langle 1^{(0)} | \hat{V} | 2^{(0)} \rangle = \begin{pmatrix} 1 & 0 \end{pmatrix} \begin{pmatrix} 0 & C^* \\ C & 0 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix}$$

$$\qquad = \begin{pmatrix} 1 & 0 \end{pmatrix} \left( \begin{pmatrix} C^* \\ 0 \end{pmatrix} \right) = (1 \cdot C^*) + (0 \cdot 0) = C^*$$

The numerator is $|C^*|^2$. Remember that $|z^*|^2 = |z|^2$, so this is just $|C|^2$.

So, the second-order correction is:

$E_2^{(2)} = \frac{|C|^2}{b - a}$

Notice that $E_2^{(2)} = -E_1^{(2)}$. This is a very common feature called **level repulsion**. The perturbation "pushes" the two energy levels apart from each other.

---

### Final Answer (from Method 1)

Let's assemble the full approximations to second order:

-   Eigenvalue 1:
    
    $$E_1(\lambda) \approx E_1^{(0)} + \lambda^2 E_1^{(2)} = a + \lambda^2 \frac{|C|^2}{a - b}$$
    
-   Eigenvalue 2:
    
    $$E_2(\lambda) \approx E_2^{(0)} + \lambda^2 E_2^{(2)} = b + \lambda^2 \frac{|C|^2}{b - a} = b - \lambda^2 \frac{|C|^2}{a - b}$$
    

---

### Method 2: Using the Hint (Expanding the Exact Solution)

This is a fantastic way to check our answer. The hint tells us to use a Taylor expansion:

$\sqrt{1 + bx^2} \approx 1 + \frac{1}{2}bx^2$

Let's start with our exact solution from part (b):

$$E_\pm = \frac{ (a+b) + \lambda(D_1 + D_2) \pm \sqrt{ ((a-b) + \lambda(D_1 - D_2))^2 + 4\lambda^2 |C|^2 } }{2}$$

Now, apply our new condition, $D_1 = D_2 = 0$:

$$E_\pm = \frac{ (a+b) \pm \sqrt{ (a-b)^2 + 4\lambda^2 |C|^2 } }{2}$$

We need to make the square root look like the hint. Let's factor out the $(a-b)^2$ term from inside the root:

$$\sqrt{ (a-b)^2 \left( 1 + \frac{4\lambda^2 |C|^2}{(a-b)^2} \right) } = (a-b) \sqrt{ 1 + \frac{4\lambda^2 |C|^2}{(a-b)^2} }$$

(Assuming $a > b$, so $\sqrt{(a-b)^2} = a-b$)

This is now in the form $\sqrt{1 + bx^2}$!

-   $x^2 \rightarrow \lambda^2$
    
-   $b \rightarrow \frac{4|C|^2}{(a-b)^2}$
    

Now, apply the hint $\sqrt{...} \approx 1 + \frac{1}{2}bx^2$:

$$(a-b) \left[ 1 + \frac{1}{2} \left( \frac{4\lambda^2 |C|^2}{(a-b)^2} \right) \right]$$

$$= (a-b) \left[ 1 + \frac{2\lambda^2 |C|^2}{(a-b)^2} \right]$$

$$= (a-b) + \frac{2\lambda^2 |C|^2}{a-b}$$

This is our approximation for the square root term. Let's plug it back into the formula for $E_\pm$:

$$E_\pm \approx \frac{ (a+b) \pm \left[ (a-b) + \frac{2\lambda^2 |C|^2}{a-b} \right] }{2}$$

Now we just separate the $E_+$ and $E_-$ solutions:

-   $E_+$ Solution (corresponds to $E_1$):
    
    $$E_+ \approx \frac{ (a+b) + (a-b) + \frac{2\lambda^2 |C|^2}{a-b} }{2} = \frac{ 2a + \frac{2\lambda^2 |C|^2}{a-b} }{2}$$
    
    $E_+ \approx a + \frac{\lambda^2 |C|^2}{a - b}$
    
-   $E_-$ Solution (corresponds to $E_2$):
    
    $$E_- \approx \frac{ (a+b) - \left[ (a-b) + \frac{2\lambda^2 |C|^2}{a-b} \right] }{2} = \frac{ 2b - \frac{2\lambda^2 |C|^2}{a-b} }{2}$$
    
    $E_- \approx b - \frac{\lambda^2 |C|^2}{a - b}$
    

As you can see, the results from both methods match perfectly! This gives us great confidence in our answer.

We have now seen how the diagonal elements of the perturbation ($D_1, D_2$) shift the energy in first order, and the off-diagonal elements ($C, C^*$) shift the energy in second order.

The next logical step in a full perturbation theory treatment would be to find the corrections to the _eigenstates_ (the eigenfunctions). Would you like to see how we calculate the first-order correction to the states $|1\rangle$ and $|2\rangle$?