# Definite Integrals: Area Under a Curve

This document provides a step-by-step calculation of the area under a trigonometric curve using integration.

## Problem Statement

Calculate the area under the curve for the function:

$$
f(x) = \sin(x)
$$

From $x = 0$ to $x = \pi$.



---

## Step 1: Set up the Definite Integral

The area $A$ under a curve $f(x)$ between two points $a$ and $b$ is given by the definite integral:

$$
A = \int_{a}^{b} f(x) \, dx
$$

For this problem:

$$
A = \int_{0}^{\pi} \sin(x) \, dx
$$

---

## Step 2: Find the Antiderivative

To solve the integral, we need the antiderivative of $\sin(x)$. Recall that:

$$
\frac{d}{dx}(-\cos(x)) = \sin(x)
$$

So, the antiderivative is $-\cos(x)$.

---

## Step 3: Apply the Fundamental Theorem of Calculus

We evaluate the antiderivative at the upper limit ($\pi$) and subtract the value at the lower limit ($0$):

$$
A = \left[ -\cos(x) \right]_{0}^{\pi}
$$

$$
A = (-\cos(\pi)) - (-\cos(0))
$$

---

## Step 4: Substitute Trigonometric Values

Using the unit circle values:
* $\cos(\pi) = -1$
* $\cos(0) = 1$

$$
A = (-(-1)) - (-(1))
$$

$$
A = 1 - (-1)
$$

$$
A = 1 + 1 = 2
$$

---

## Final Solution

The total area under the curve of $f(x) = \sin(x)$ from $0$ to $\pi$ is:

$$
2 \text{ square units}
$$

### Summary
* **Function:** $\sin(x)$
* **Limits:** $[0, \pi]$
* **Result:** $2$