# Optimization: Maximizing the Area of a Rectangle

This document provides a step-by-step calculus solution to find the dimensions of a rectangle with the maximum possible area inscribed under a parabolic curve.

## Problem Statement

A rectangle is placed in the first quadrant with:
- One side on the x-axis.
- One side on the y-axis.
- One vertex on the curve $y = 3 - x^2$.



**Goal:** Find the dimensions ($x$ and $y$) that maximize the area of this rectangle.

---

## Step 1: Define the Area Function

A point $(x, y)$ on the curve defines the top-right corner of the rectangle. 
- The width is $x$.
- The height is $y = 3 - x^2$.

The Area ($A$) of the rectangle is:

$$
A = \text{width} \times \text{height} = x \cdot y
$$

Substituting the curve equation:

$$
A(x) = x(3 - x^2) = 3x - x^3
$$

---

## Step 2: Find the Critical Points

To find the maximum area, we take the derivative of the area function with respect to $x$ and set it to zero:

$$
A'(x) = \frac{d}{dx}(3x - x^3)
$$

$$
A'(x) = 3 - 3x^2
$$

Set the derivative to zero:

$$
3 - 3x^2 = 0
$$

$$
3x^2 = 3 \implies x^2 = 1
$$

Since the rectangle is in the first quadrant, we take the positive root:

$$
x = 1
$$

---

## Step 3: Verify the Maximum

We use the Second Derivative Test to ensure this point is a maximum:

$$
A''(x) = -6x
$$

Substituting $x = 1$:

$$
A''(1) = -6(1) = -6
$$

Since $A''(x) < 0$, the function is concave down at $x = 1$, confirming a **local maximum**.

---

## Step 4: Calculate the Dimensions and Maximum Area

Now, find the corresponding height ($y$) by substituting $x = 1$ back into the curve equation:

$$
y = 3 - (1)^2 = 2
$$

**The Maximum Area is:**

$$
A = 1 \times 2 = 2 \text{ square units}
$$

---

## Final Solution

The dimensions of the rectangle with the maximum area are:

$$
\text{Width } (x) = 1, \quad \text{Height } (y) = 2
$$

### Summary
- **Critical Value:** $x = 1$
- **Maximized Dimensions:** $1 \times 2$
- **Total Area:** $2$