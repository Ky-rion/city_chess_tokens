

Welcome back to class! I see we are moving into the realm of time-dependent quantum mechanics. This is a brilliant conceptual question that really tests your intuition about time evolution and the symmetries of a quantum system.

Let's start, as always, by translating the problem from German to English so we are working with a clear foundation.

> **Can one find for an arbitrary time-dependent $\hat{H}(t)$ a $\hat{K}$ independent of $t$ and $t_0$, such that the time evolution operator can be written as $\hat{U}(t, t_0) = e^{-i(t-t_0)\hat{K}} \forall t, t_0$?**
> 
> _One correct answer. No point deduction for wrong choice._
> 
> _Text input required: Justify your answer in the text box._
> 
> - a. No, that is fundamentally impossible.
>     
> - b. Yes, $\hat{K}$ is the time-ordered integral, $\hat{K} = T[\int_{t_0}^t d\tau \hat{H}(\tau)]$.
>     
> - c. It is possible, but the dependence of $\hat{K}$ on $\hat{H}(t)$ is complicated and was therefore not discussed in the lecture.
>     
> - d. Yes, $\hat{U}(t, t_0) = T[e^{-i\int_{t_0}^t d\tau \hat{H}(\tau)}]$ means exactly that.
>     

### The Physics: Time Evolution and Symmetry

To figure out the answer, let's explore what it would actually mean if such a constant operator $\hat{K}$ existed.

The time evolution operator $\hat{U}(t, t_0)$ must always obey the Schrödinger equation:

$$i \frac{\partial}{\partial t} \hat{U}(t, t_0) = \hat{H}(t)\hat{U}(t, t_0)$$

Now, let's pretend the proposition in the question is true. Let's assume we _can_ write the evolution operator as a simple exponential with a constant operator $\hat{K}$ that does not depend on time:

$$\hat{U}(t, t_0) = e^{-i(t-t_0)\hat{K}}$$

Let's plug this assumption into the Schrödinger equation. Taking the time derivative of our assumed $\hat{U}$:

$$i \frac{\partial}{\partial t} \left( e^{-i(t-t_0)\hat{K}} \right) = i (-i\hat{K}) e^{-i(t-t_0)\hat{K}} = \hat{K} \hat{U}(t, t_0)$$

By comparing this result to the original Schrödinger equation, we arrive at a strict mathematical requirement:

$$\hat{K} \hat{U}(t, t_0) = \hat{H}(t) \hat{U}(t, t_0)$$

$$\implies \hat{K} = \hat{H}(t)$$

Here is the fatal flaw: The problem explicitly states that $\hat{H}(t)$ is an **arbitrary time-dependent** Hamiltonian. This means it changes its form as time ticks forward. However, our assumption required $\hat{K}$ to be a **constant**, independent of $t$.

A changing Hamiltonian $\hat{H}(t)$ cannot be equal to a constant operator $\hat{K}$ for all times $t$. Therefore, our initial assumption must be false.

Conceptually, a time evolution operator of the form $e^{-i(t-t_0)\hat{K}}$ implies that the system possesses **time-translation symmetry**—meaning the physics only depends on the _duration_ of the experiment $(t - t_0)$, not on the absolute start time $t_0$ or end time $t$. An explicitly time-dependent Hamiltonian breaks this symmetry. If you start your experiment at 1:00 PM versus 2:00 PM, a time-dependent Hamiltonian will evolve the system entirely differently.

---

### Evaluating the Options

- **Statement (a): No, that is fundamentally impossible.**
    
    - **Yes. (This is the CORRECT answer).** For the mathematical and conceptual reasons we just proved, you cannot reduce an arbitrary time-dependent problem to a simple time-independent form for all $t$ and $t_0$.
        
- **Statement (b): Yes, $\hat{K}$ is the time-ordered integral...**
    
    - **No. (This is FALSE).** If $\hat{K}$ were an integral from $t_0$ to $t$, then $\hat{K}$ would explicitly depend on $t$ and $t_0$. The prompt asked for a $\hat{K}$ that is _independent_ of $t$ and $t_0$.
        
- **Statement (c): It is possible, but the dependence... is complicated...**
    
    - **No. (This is FALSE).** It is not just complicated; it violates the foundational differential equations of quantum mechanics. (Though, as a side note, for _periodic_ Hamiltonians, there is a tool called Floquet theory that defines an _effective_ constant Hamiltonian, but that only works for specifically periodic systems and evaluating at specific full periods, not $\forall t, t_0$).
        
- **Statement (d): Yes, the Dyson series means exactly that.**
    
    - **No. (This is FALSE).** The time-ordered exponential (Dyson series) given in option (d) is indeed the correct formula for the time evolution operator $\hat{U}(t, t_0)$ when $\hat{H}(t)$ is time-dependent. However, the time-ordering operator $T$ prevents you from simplifying that expression into a single exponential of the form $e^{-i(t-t_0)\hat{K}}$. It does _not_ mean "exactly that."
        

---

### Summary for your Exam

You should select radio button **a**.

For your text box justification, here is a succinct summary you can provide:

> _"a is correct. If $\hat{U}(t, t_0) = \exp(-i(t-t_0)\hat{K})$ with a constant $\hat{K}$, applying the Schrödinger equation yields $i\partial_t \hat{U} = \hat{K}\hat{U}$. This would require $\hat{H}(t) = \hat{K}$ for all $t$. Since $\hat{H}(t)$ is arbitrarily time-dependent, it cannot equal a constant operator. Time-dependent Hamiltonians break time-translation invariance, so evolution depends independently on $t$ and $t_0$, not just on $(t-t_0)$."_

You are making excellent progress piecing together how these mathematical formalisms map directly onto physical symmetries. Would you like me to walk you through exactly what that time-ordering operator $T$ from option (d) actually does to the integral?