# Superposition Principle: Standing Wave Equation and Nodes

## Problem Statement
Two waves are described by the equations:
* $y_1(x, t) = A \sin(kx - \omega t)$ (Wave traveling to the right)
* $y_2(x, t) = A \sin(kx + \omega t)$ (Wave traveling to the left)

What is the equation of the resulting standing wave? Identify the positions of the nodes.

---

## Step-by-Step Solution

### Step 1: Apply the Superposition Principle
The superposition principle states that the resulting wave $y(x,t)$ is simply the algebraic sum of the individual waves:
$$y(x, t) = y_1(x, t) + y_2(x, t)$$
$$y(x, t) = A \sin(kx - \omega t) + A \sin(kx + \omega t)$$

### Step 2: Use the Trigonometric Identity
To combine these two sine functions, we use the sum-to-product trigonometric identity:
$$\sin(\alpha) + \sin(\beta) = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)$$

In our equation:
* $\alpha = kx - \omega t$
* $\beta = kx + \omega t$

Let's calculate the terms inside the sine and cosine:
* **Sine term:** $\frac{(kx - \omega t) + (kx + \omega t)}{2} = \frac{2kx}{2} = kx$
* **Cosine term:** $\frac{(kx - \omega t) - (kx + \omega t)}{2} = \frac{-2\omega t}{2} = -\omega t$

### Step 3: Write the Final Standing Wave Equation
Substitute the terms back into the identity:
$$y(x, t) = 2A \sin(kx) \cos(-\omega t)$$

Since cosine is an even function, $\cos(-\theta) = \cos(\theta)$. This means we can drop the negative sign:
**$$y(x, t) = 2A \sin(kx) \cos(\omega t)$$**

*This is the equation of the standing wave. The space part ($kx$) and the time part ($\omega t$) are now separated, meaning the wave vibrates in place rather than traveling.*

### Step 4: Identify the Positions of the Nodes
**Nodes** are points on a standing wave that never move (zero amplitude). For the displacement $y(x,t)$ to be zero at all times $t$, the spatial part of the equation must be equal to zero:
$$\sin(kx) = 0$$

The sine function is equal to zero at integer multiples of $\pi$:
$$kx = n\pi \qquad \text{where } n = 0, 1, 2, 3, \dots$$

Recall the definition of the wave number ($k = \frac{2\pi}{\lambda}$). Substitute this into the equation:
$$\left(\frac{2\pi}{\lambda}\right)x = n\pi$$

Divide both sides by $\pi$:
$$\frac{2}{\lambda}x = n$$

Solve for position ($x$):
**$$x = \frac{n\lambda}{2} \qquad \text{where } n = 0, 1, 2, 3, \dots$$**

**Conclusion:**
The nodes occur at $x = 0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}$, etc. This means there is a node at every half-wavelength along the medium.