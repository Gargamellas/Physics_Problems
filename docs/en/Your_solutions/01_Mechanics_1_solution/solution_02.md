# Physics I: Range Optimization in Projectile Motion

## Problem Statement
For a projectile motion on a level ground, the horizontal range $R$ as a function of the launch angle $\theta$ is given by:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

**Goal:** Show analytically that for a given initial velocity ($v_0$), the maximum range is achieved when the launch angle is $\theta = 45^\circ$.

---

## Analytical Proof Using Calculus

To find the angle $\theta$ that maximizes the range function $R(\theta)$, we need to find its critical points. We do this by taking the first derivative of the function with respect to $\theta$ and setting it to zero.

### Step 1: Define the Constants and Variables
* **Variable:** The launch angle $\theta$ (domain is $0^\circ \le \theta \le 90^\circ$).
* **Constants:** Initial velocity $v_0$ and gravitational acceleration $g$.

### Step 2: Take the First Derivative
We differentiate $R(\theta)$ with respect to $\theta$. Since $\frac{v_0^2}{g}$ is a constant, we only need to differentiate $\sin(2\theta)$ using the chain rule.
$$R'(\theta) = \frac{d}{d\theta} \left( \frac{v_0^2 \sin(2\theta)}{g} \right)$$
$$R'(\theta) = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2$$
$$R'(\theta) = \frac{2v_0^2 \cos(2\theta)}{g}$$

### Step 3: Set the Derivative to Zero
To find the maximum, we set $R'(\theta) = 0$:
$$\frac{2v_0^2 \cos(2\theta)}{g} = 0$$

Since $\frac{2v_0^2}{g}$ cannot be zero (assuming the projectile is actually launched), the trigonometric part must be zero:
$$\cos(2\theta) = 0$$

### Step 4: Solve for $\theta$
In the physical context of projectile motion, the angle $2\theta$ must be $90^\circ$ (or $\pi/2$ radians) for the cosine to be zero.
$$2\theta = 90^\circ$$
$$\mathbf{\theta = 45^\circ}$$

---

## Alternative Logical Proof (Trigonometric Property)
Without using calculus, we can analyze the maximum value of the sine function itself.
1. The range formula is $R(\theta) = \frac{v_0^2}{g} \sin(2\theta)$.
2. The maximum possible value for any sine function is $1$.
3. Therefore, $R$ is maximized when $\sin(2\theta) = 1$.
4. The sine of an angle equals $1$ when the angle is $90^\circ$.
$$2\theta = 90^\circ \implies \mathbf{\theta = 45^\circ}$$

### Conclusion
Both calculus optimization and trigonometric properties analytically prove that a launch angle of **$45^\circ$** yields the absolute maximum horizontal range for any given initial velocity.