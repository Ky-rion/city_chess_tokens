

Welcome back! I am thrilled to see you continuing your journey into quantum mechanics. This problem is an excellent exercise because it tests your understanding of the foundational vocabulary of quantum theory: operators, hermiticity, unitarity, and projectors.

Let's do what we did before and translate the German text to ensure we are entirely on the same page:

> **Which of the following statements are correct? Operators act in the respective space of square-integrable functions, Bra and Ket vectors are assumed to be orthonormal respectively.**
> 
> _Select all correct answers. Selecting wrong answers gives a point deduction._
> 
> _Text input required: Justify your answer(s) in the text box._
> 
> - a. $\cos(\alpha)|1\rangle\langle1| + \sin(\alpha)|2\rangle\langle2|$ is unitary for the 2-level system with basis $\{|1\rangle, |2\rangle\}$.
>     
> - b. $\frac{1}{2} [|a\rangle\langle a| - |a\rangle\langle b| - |b\rangle\langle a| + |b\rangle\langle b|]$ is a projector.
>     
> - c. Creation operators $a^\dagger$ are not hermitian.
>     
> - d. The multiplication operator $e^{i \cos(x)}$ is unitary.
>     
> - e. $\partial_p$ is not normal.
>     
> - f. Creation operators $a^\dagger$ are normal.
>     

To tackle these, we need a quick refresher on operator properties. An operator $O$ with an adjoint (complex conjugate transpose) $O^\dagger$ is:

- **Hermitian** if $O = O^\dagger$ (represents observable physical quantities).
    
- **Unitary** if $O^\dagger O = O O^\dagger = I$ (preserves probability).
    
- **Normal** if $O^\dagger O = O O^\dagger$ (commutes with its adjoint).
    
- **A Projector** if $P^2 = P$ and $P^\dagger = P$.
    

Let's evaluate each option step-by-step!

---

### Statement (a)

**Is $U = \cos(\alpha)|1\rangle\langle1| + \sin(\alpha)|2\rangle\langle2|$ unitary?**

**No. (This statement is FALSE).**

- **The Physics:** Let's check the unitarity condition $U^\dagger U = I$.
    
    Assuming $\alpha$ is a real number, the adjoint $U^\dagger$ is exactly the same as $U$.
    
    If we multiply them:
    
    $$U^\dagger U = \left( \cos(\alpha)|1\rangle\langle1| + \sin(\alpha)|2\rangle\langle2| \right) \left( \cos(\alpha)|1\rangle\langle1| + \sin(\alpha)|2\rangle\langle2| \right)$$
    
    Because $|1\rangle$ and $|2\rangle$ are orthonormal ($\langle1|1\rangle=1$, $\langle1|2\rangle=0$, etc.), the cross terms vanish, leaving us with:
    
    $$U^\dagger U = \cos^2(\alpha)|1\rangle\langle1| + \sin^2(\alpha)|2\rangle\langle2|$$
    
    For this to equal the identity operator $I = |1\rangle\langle1| + |2\rangle\langle2|$, we would need $\cos^2(\alpha) = 1$ **and** $\sin^2(\alpha) = 1$ simultaneously, which is mathematically impossible for any angle $\alpha$.
    

### Statement (b)

**Is $P = \frac{1}{2} [|a\rangle\langle a| - |a\rangle\langle b| - |b\rangle\langle a| + |b\rangle\langle b|]$ a projector?**

**Yes. (This statement is CORRECT).**

- **The Physics:** We can factor this expression neatly. Notice that it looks like a perfect square. Let's define a new state vector:
    
    $$|\psi\rangle = \frac{1}{\sqrt{2}}(|a\rangle - |b\rangle)$$
    
    If we take the outer product of this state with itself ($|\psi\rangle\langle\psi|$), we get exactly the expression for $P$.
    
    Is $|\psi\rangle$ normalized? Let's check its inner product:
    
    $$\langle\psi|\psi\rangle = \frac{1}{2} (\langle a| - \langle b|)(|a\rangle - |b\rangle) = \frac{1}{2} (\langle a|a\rangle - \langle a|b\rangle - \langle b|a\rangle + \langle b|b\rangle)$$
    
    Since the problem states the vectors are orthonormal, $\langle a|a\rangle=1$, $\langle b|b\rangle=1$, and the mixed terms are $0$. So, $\langle\psi|\psi\rangle = \frac{1}{2}(1 + 1) = 1$.
    
    Because $P = |\psi\rangle\langle\psi|$ and $|\psi\rangle$ is a properly normalized state, $P$ is a valid projection operator onto the state $|\psi\rangle$. It satisfies $P^2 = P$ and $P^\dagger = P$.
    

### Statement (c)

**Are creation operators $a^\dagger$ _not_ hermitian?**

**Yes. (This statement is CORRECT).**

- **The Physics:** A Hermitian operator must equal its own adjoint ($O = O^\dagger$). By definition, the adjoint of the creation operator $a^\dagger$ is the annihilation operator $a$.
    
    Since $a^\dagger$ adds a quantum of energy (e.g., a photon) and $a$ destroys one, they do completely different things to a system. Therefore, $a^\dagger \neq a$, meaning it is indeed **not** Hermitian.
    

### Statement (d)

**Is the multiplication operator $e^{i \cos(x)}$ unitary?**

**Yes. (This statement is CORRECT).**

- **The Physics:** Let $U = e^{i \cos(x)}$. The adjoint of a complex exponential multiplication operator is just its complex conjugate, so $U^\dagger = e^{-i \cos(x)}$.
    
    Let's check the unitary condition $U^\dagger U = I$:
    
    $$U^\dagger U = e^{-i \cos(x)} e^{i \cos(x)} = e^0 = 1$$
    
    Multiplying by $1$ is the same as the identity operator. Therefore, it is unitary.
    

### Statement (e)

**Is $\partial_p$ _not_ normal?**

**No. (This statement is FALSE).**

- **The Physics:** An operator is normal if it commutes with its adjoint ($O^\dagger O = O O^\dagger$).
    
    In momentum space, the derivative operator $O = \frac{\partial}{\partial p}$ is anti-Hermitian, meaning its adjoint is $O^\dagger = -\frac{\partial}{\partial p}$.
    
    Let's check the commutator:
    
    $$O^\dagger O = \left(-\frac{\partial}{\partial p}\right) \left(\frac{\partial}{\partial p}\right) = -\frac{\partial^2}{\partial p^2}$$
    
    $$O O^\dagger = \left(\frac{\partial}{\partial p}\right) \left(-\frac{\partial}{\partial p}\right) = -\frac{\partial^2}{\partial p^2}$$
    
    Since both sides equal $-\frac{\partial^2}{\partial p^2}$, the operator _does_ commute with its adjoint. Therefore, it **is** normal. The statement claims it is not, so the statement is false.
    

### Statement (f)

**Are creation operators $a^\dagger$ normal?**

**No. (This statement is FALSE).**

- **The Physics:** As we defined above, an operator is normal if $O^\dagger O = O O^\dagger$. For $a^\dagger$, this means we need to check if $a a^\dagger = a^\dagger a$.
    
    This leads us directly to the fundamental commutation relation of quantum mechanics: $[a, a^\dagger] = a a^\dagger - a^\dagger a = 1$.
    
    Because $a a^\dagger - a^\dagger a = 1$ (and not $0$), they do not commute. Therefore, $a^\dagger$ is **not** normal.
    

---

### Summary for your Exam

You should check boxes **b, c, and d**.

For the required text box justification, you can use this concise summary:

> _"a is false because $U^\dagger U = \cos^2(\alpha)|1\rangle\langle1| + \sin^2(\alpha)|2\rangle\langle2| \neq I$. b is correct because $P$ factors into $|\psi\rangle\langle\psi|$ where $|\psi\rangle = (|a\rangle - |b\rangle)/\sqrt{2}$, which is normalized, satisfying $P^2=P$ and $P^\dagger=P$. c is correct because $(a^\dagger)^\dagger = a \neq a^\dagger$. d is correct because $U^\dagger U = e^{-i \cos(x)} e^{i \cos(x)} = 1 = I$. e is false because $\partial_p$ is anti-Hermitian ($\partial_p^\dagger = -\partial_p$) and commutes with itself, making it normal. f is false because $[a, a^\dagger] = 1 \neq 0$, so it does not commute with its adjoint."_

Would you like me to explain more about the creation and annihilation operators ($a$ and $a^\dagger$) and how they act on the quantum harmonic oscillator?