# Damped Harmonic Oscillator: Step-by-Step Analysis

## Problem Statement
Analyze the damped harmonic oscillator described by the equation:
$$m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0$$
Investigate the general solution, classify the damping cases, and prepare for numerical/graphical analysis.

---

## Step 1: The General Solution
To solve this 2nd-order linear differential equation, we guess a solution of the form $x(t) = e^{rt}$. Substituting this into the equation gives us the **characteristic equation**:
$$mr^2 + br + k = 0$$

Using the quadratic formula to solve for $r$:
$$r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}$$

The general solution is a linear combination of these roots:
$$x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}$$

---

## Step 2: Classification of Damping Cases
The behavior of the system entirely depends on what is inside the square root: the discriminant **$(b^2 - 4mk)$**.

1. **Underdamped ($b^2 - 4mk < 0$):**
   The friction ($b$) is weak. The roots are complex numbers. The system oscillates back and forth, but the amplitude slowly decays over time. 
   *(Phase Portrait: Spirals inward toward the origin).*

2. **Critically Damped ($b^2 - 4mk = 0$):**
   The friction is perfectly balanced. The roots are real and equal. The system returns to the equilibrium position ($x=0$) as fast as possible without oscillating. 
   *(Phase Portrait: Curves directly into the origin).*

3. **Overdamped ($b^2 - 4mk > 0$):**
   The friction ($b$) is extremely strong (like moving in honey). The roots are real and distinct. The system slowly creeps back to equilibrium without ever crossing the zero line.
   *(Phase Portrait: Slowly approaches the origin without spiraling).*

---

## Step 3: Numerical Solution (RK4 Method)
To solve this numerically (e.g., in Python or JavaScript) using the Runge-Kutta 4th Order (RK4) method, we must split the 2nd-order equation into two 1st-order equations.
Let velocity be $v = \frac{dx}{dt}$.
1. $\frac{dx}{dt} = v$
2. $\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x$

We use RK4 to step through time ($t$), continuously updating position ($x$) and velocity ($v$).

---

## Step 4 & 5: Effect of Parameter 'b' and $x(t)$ Graph
* As $b$ increases from $0$, the oscillations in the $x(t)$ graph die out faster (Underdamped).
* At the critical point $b_c = 2\sqrt{mk}$, oscillations vanish completely (Critically Damped).
* If $b$ increases further, the return to $x=0$ simply becomes slower and flatter (Overdamped).

## Step 6: The Phase Portrait
A phase portrait plots **Velocity ($v$) vs. Position ($x$)**.
* **Underdamped:** Forms a shrinking spiral.
* **Critically/Overdamped:** Forms a curve that heads directly to $(0,0)$ without looping around the axes.