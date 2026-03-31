# Kinematics: Path Intersection and Minimum Distance Analysis

## Problem Statement
Alice and Bob are moving along parametric paths defined by:
* **Alice's Path:** $A(t) = (2+t, 8-3t)$
* **Bob's Path:** $B(t) = (2t-1, 2t+2)$

**Objectives:**
1. Determine if their paths intersect.
2. Determine if they collide (arrive at the same point at the same time).
3. If they do not collide, find the minimum distance between them and when it occurs.

---

## 1. Path Intersection
To find if the *paths* intersect, we must check if there is a spatial coordinate $(x, y)$ that both Alice and Bob visit. Because they might visit this point at different times, we eliminate the parameter $t$ to find the Cartesian line equations for both paths.

**Alice's Path:**
$$x = 2 + t_A \implies t_A = x - 2$$
Substitute $t_A$ into her $y$ equation:
$$y = 8 - 3(x - 2) = 8 - 3x + 6$$
**Equation for Alice's line:** $y = -3x + 14$

**Bob's Path:**
$$x = 2t_B - 1 \implies t_B = \frac{x + 1}{2}$$
Substitute $t_B$ into his $y$ equation:
$$y = 2\left(\frac{x + 1}{2}\right) + 2$$
**Equation for Bob's line:** $y = x + 3$

Set the two Cartesian equations equal to find the intersection point:
$$-3x + 14 = x + 3$$
$$11 = 4x \implies x = 2.75$$

Substitute $x = 2.75$ back into Bob's line equation to find $y$:
$$y = 2.75 + 3 = 5.75$$

**Conclusion:** Yes, their paths intersect at the Cartesian point **(2.75, 5.75)**.

---

## 2. Collision Check
A collision only occurs if they reach the intersection point at the *exact same time* $t$. To verify this, we set $A(t) = B(t)$ and check if there is a single $t$ that satisfies both dimensions.

**Comparing x-coordinates:**
$$2 + t = 2t - 1 \implies t = 3$$

**Comparing y-coordinates:**
$$8 - 3t = 2t + 2 \implies 6 = 5t \implies t = 1.2$$

**Conclusion:** Since $t = 3$ does not equal $t = 1.2$, they arrive at the intersection point at different times. **They do not collide.**

---

## 3. Minimum Distance Optimization
Since there is no collision, we must find the exact time $t$ when the distance between Alice and Bob is minimized. 

Let $D(t)$ be the distance between Alice and Bob at time $t$. To simplify the calculus, it is standard practice to minimize the square of the distance, $f(t) = D(t)^2$, using the distance formula:
$$f(t) = (x_B - x_A)^2 + (y_B - y_A)^2$$

Substitute their parametric equations into the formula:
$$f(t) = ((2t - 1) - (2 + t))^2 + ((2t + 2) - (8 - 3t))^2$$
$$f(t) = (t - 3)^2 + (5t - 6)^2$$

Expand the binomials:
$$f(t) = (t^2 - 6t + 9) + (25t^2 - 60t + 36)$$
$$f(t) = 26t^2 - 66t + 45$$

To find the minimum, we take the first derivative of $f(t)$ with respect to $t$ and set it to zero:
$$f'(t) = 52t - 66 = 0$$
$$52t = 66 \implies t = \frac{66}{52} = \frac{33}{26} \approx 1.269$$

To find the minimum distance squared, plug $t = \frac{33}{26}$ back into $f(t)$:
$$f\left(\frac{33}{26}\right) = 26\left(\frac{33}{26}\right)^2 - 66\left(\frac{33}{26}\right) + 45$$
$$f\left(\frac{33}{26}\right) = \frac{33^2}{26} - \frac{66 \cdot 33}{26} + \frac{45 \cdot 26}{26}$$
$$f\left(\frac{33}{26}\right) = \frac{1089 - 2178 + 1170}{26} = \frac{81}{26}$$

Finally, take the square root to find the actual minimum distance $D_{min}$:
$$D_{min} = \sqrt{\frac{81}{26}} = \frac{9}{\sqrt{26}} = \frac{9\sqrt{26}}{26} \approx 1.765$$

### Final Summary
* **Path Intersection:** Yes, at point (2.75, 5.75)
* **Collision:** No
* **Time of Minimum Distance:** $t = \frac{33}{26}$ (approx 1.269)
* **Minimum Distance:** $\frac{9\sqrt{26}}{26}$ (approx 1.765)