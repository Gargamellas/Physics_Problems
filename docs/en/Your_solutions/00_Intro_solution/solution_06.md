# Function Analysis: Finding Local Extrema

This document demonstrates how to identify the local maxima or minima of a quadratic function using the derivative method.

## Problem Statement

Consider the function:

$$
f(x) = 3x^2 - 12x + 7
$$



**Goal:** Identify any local maxima or minima.

---

## Step 1: Find the First Derivative

To find the critical points (where the slope is zero), we first calculate the derivative $f'(x)$ with respect to $x$:

$$
f'(x) = \frac{d}{dx}(3x^2 - 12x + 7)
$$

Using the power rule:

$$
f'(x) = 6x - 12
$$

---

## Step 2: Solve for Critical Points

Set the derivative equal to zero to find the value of $x$ where the slope of the tangent line is horizontal:

$$
6x - 12 = 0
$$

$$
6x = 12
$$

$$
x = 2
$$

---

## Step 3: Determine the Nature of the Extrema

We use the **Second Derivative Test** to check if this point is a maximum or a minimum:

$$
f''(x) = \frac{d}{dx}(6x - 12) = 6
$$

Since $f''(x) = 6$, which is **greater than zero** ($f''(x) > 0$), the function is concave up at this point. Therefore, $x = 2$ is a **local minimum**.

---

## Step 4: Calculate the Function Value at the Minimum

Substitute $x = 2$ back into the original function $f(x)$ to find the $y$-coordinate:

$$
f(2) = 3(2)^2 - 12(2) + 7
$$

$$
f(2) = 3(4) - 24 + 7
$$

$$
f(2) = 12 - 24 + 7 = -5
$$

---

## Final Solution

The function $f(x) = 3x^2 - 12x + 7$ has a **local minimum** at the point:

$$
(2, -5)
$$

### Summary
* **Type:** Local Minimum
* **Coordinates:** $x = 2, y = -5$
* **Reasoning:** The parabola opens upwards ($a > 0$), and the first derivative is zero at $x = 2$.