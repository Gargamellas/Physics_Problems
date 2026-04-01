# Kinematics: Parametric Equations and Acceleration

## Problem Statement
The path equation is given in parametric form:
$$x(t) = 2t^2, \qquad y(t) = 3t^3$$

**Tasks:**
1. Eliminate the parameter $t$.
2. Describe/Draw the trajectory.
3. Calculate $\vec{v}(t)$, $|\vec{v}(t)|$, $\vec{a}(t)$, and $|\vec{a}(t)|$.
4. Is the acceleration constant?

---

## Step-by-Step Solution

### 1. Eliminate the parameter $t$
To find the Cartesian equation (the path without time), we isolate $t$ in one equation and substitute it into the other. 

From the $x$ equation:
$$x = 2t^2 \implies t^2 = \frac{x}{2}$$
Assuming $t \ge 0$, we take the square root: 
$$t = \left(\frac{x}{2}\right)^{1/2}$$

Substitute this $t$ value into the $y$ equation:
$$y = 3\left(\left(\frac{x}{2}\right)^{1/2}\right)^3 = 3\left(\frac{x}{2}\right)^{3/2}$$

To remove the fractional exponent and make it look cleaner, square both sides:
$$y^2 = 9\left(\frac{x}{2}\right)^3 = 9\left(\frac{x^3}{8}\right)$$
**$$y^2 = \frac{9}{8}x^3$$**

### 2. Draw the trajectory
The equation $y^2 = \frac{9}{8}x^3$ represents a curve known as a **semicubical parabola**.
* At $t = 0$, the object starts at the origin $(0,0)$.
* As $t$ increases, both $x$ and $y$ increase, moving the object into the first quadrant.
* Because $y$ grows cubically ($t^3$) while $x$ grows quadratically ($t^2$), the path curves upwards, becoming steeper over time.

### 3. Calculate Velocity and Acceleration Vectors
The position vector is $\vec{r}(t) = 2t^2\hat{i} + 3t^3\hat{j}$. We find velocity and acceleration using derivatives with respect to time ($t$).

**A. Velocity $\vec{v}(t)$:**
Take the first derivative of the position vector:
$$\vec{v}(t) = \frac{d}{dt}(2t^2)\hat{i} + \frac{d}{dt}(3t^3)\hat{j}$$
**$$\vec{v}(t) = 4t\hat{i} + 9t^2\hat{j}$$**

**B. Magnitude of Velocity $|\vec{v}(t)|$ (Speed):**
Use the Pythagorean theorem on the velocity components:
$$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2}$$
**$$|\vec{v}(t)| = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}$$**

**C. Acceleration $\vec{a}(t)$:**
Take the derivative of the velocity vector:
$$\vec{a}(t) = \frac{d}{dt}(4t)\hat{i} + \frac{d}{dt}(9t^2)\hat{j}$$
**$$\vec{a}(t) = 4\hat{i} + 18t\hat{j}$$**

**D. Magnitude of Acceleration $|\vec{a}(t)|$:**
Use the Pythagorean theorem on the acceleration components:
$$|\vec{a}(t)| = \sqrt{4^2 + (18t)^2}$$
**$$|\vec{a}(t)| = \sqrt{16 + 324t^2}$$**

### 4. Is the acceleration constant?
Let's look at the acceleration vector we found: $\vec{a}(t) = 4\hat{i} + 18t\hat{j}$.
* The $x$-component is **$4$**, which is constant.
* The $y$-component is **$18t$**, which changes as time ($t$) changes.

**Conclusion:** **No, the acceleration is not constant.** It is time-dependent (variable) because its vertical component continues to increase as time goes on.