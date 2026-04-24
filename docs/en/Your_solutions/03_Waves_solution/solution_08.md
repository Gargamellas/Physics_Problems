# Waves: Checking the Wave Equation

## Problem Statement
Which of the following functions can describe a traveling wave? 
Hint: check if it satisfies the wave equation:
$$\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}$$

a) $y(x,t) = A \cos(kx^2 - \omega t)$
b) $y(x,t) = A(x-vt)^2$
c) $y(x,t) = A \log(x+vt)$

---

## Step-by-Step Solution

To check if a function is a valid wave, we must take its second partial derivative with respect to $x$, and its second partial derivative with respect to $t$, and see if they balance perfectly in the wave equation.

### Test (a): $y(x,t) = A \cos(kx^2 - \omega t)$
Let's find the second derivative with respect to $t$ (treating $x$ as a constant):
1. First derivative: $\frac{\partial y}{\partial t} = A \omega \sin(kx^2 - \omega t)$
2. Second derivative: $\frac{\partial^2 y}{\partial t^2} = -A \omega^2 \cos(kx^2 - \omega t)$

Now, let's find the second derivative with respect to $x$ (treating $t$ as a constant):
1. First derivative: $\frac{\partial y}{\partial x} = -A \sin(kx^2 - \omega t) \cdot (2kx)$
2. Second derivative involves the product rule and gets very messy, resulting in terms with $x^2$. It will **not** match the simple cosine term we got for $t$.
* **Conclusion for (a):** Fails the wave equation. Not a traveling wave.

---

### Test (b): $y(x,t) = A(x-vt)^2$
Let's check the derivatives.
* **With respect to $x$:**
  1. $\frac{\partial y}{\partial x} = 2A(x-vt) \cdot (1) = 2A(x-vt)$
  2. $\frac{\partial^2 y}{\partial x^2} = 2A$

* **With respect to $t$:**
  1. $\frac{\partial y}{\partial t} = 2A(x-vt) \cdot (-v) = -2Av(x-vt)$
  2. $\frac{\partial^2 y}{\partial t^2} = -2Av \cdot (-v) = 2Av^2$

* **Plug into the wave equation:**
  $$2A \stackrel{?}{=} \frac{1}{v^2} (2Av^2)$$
  $$2A = 2A$$
* **Conclusion for (b):** The equation balances perfectly. **It IS a traveling wave.**

---

### Test (c): $y(x,t) = A \log(x+vt)$
Let's check the derivatives (using natural log, where derivative of $\log(u) = 1/u$).
* **With respect to $x$:**
  1. $\frac{\partial y}{\partial x} = A \cdot \frac{1}{x+vt} \cdot (1) = \frac{A}{x+vt}$
  2. $\frac{\partial^2 y}{\partial x^2} = \frac{-A}{(x+vt)^2}$

* **With respect to $t$:**
  1. $\frac{\partial y}{\partial t} = A \cdot \frac{1}{x+vt} \cdot (v) = \frac{Av}{x+vt}$
  2. $\frac{\partial^2 y}{\partial t^2} = \frac{-Av \cdot (v)}{(x+vt)^2} = \frac{-Av^2}{(x+vt)^2}$

* **Plug into the wave equation:**
  $$\frac{-A}{(x+vt)^2} \stackrel{?}{=} \frac{1}{v^2} \left( \frac{-Av^2}{(x+vt)^2} \right)$$
  $$\frac{-A}{(x+vt)^2} = \frac{-A}{(x+vt)^2}$$
* **Conclusion for (c):** The equation balances perfectly. **It IS a traveling wave.**

---

## Final Answer
Functions **(b)** and **(c)** can describe a traveling wave because they satisfy the wave equation. Function (a) cannot.