# infinite Series: The Ant's Final Position

This document provides a step-by-step calculation to find the final $(x, y)$ coordinates of an ant moving in a repeating cardinal pattern with decreasing step sizes.

## Problem Statement

An ant starts at the origin $(0,0)$ and moves in the following pattern:
1. $1\text{ m}$ **East** ($+x$)
2. $1/2\text{ m}$ **North** ($+y$)
3. $1/3\text{ m}$ **West** ($-x$)
4. $1/4\text{ m}$ **South** ($-y$)
5. $1/5\text{ m}$ **East** ($+x$)
... and so on.



**Goal:** Determine the final $(x, y)$ position of the ant.

---

## Step 1: Analyze Horizontal Movement ($x$)

The ant moves East on the 1st, 5th, 9th steps... and West on the 3rd, 7th, 11th steps...
The horizontal position $x$ is the sum:

$$
x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots
$$

This is a known infinite series related to the Taylor series for $\arctan(x)$:
$\arctan(x) = x - \frac{x^3}{3} + \frac{x^5}{5} - \dots$

Substituting $x = 1$:
$\arctan(1) = 1 - \frac{1}{3} + \frac{1}{5} - \dots$

Since $\arctan(1) = \frac{\pi}{4}$:

$$
x = \frac{\pi}{4} \approx 0.785
$$

---

## Step 2: Analyze Vertical Movement ($y$)

The ant moves North on the 2nd, 6th, 10th steps... and South on the 4th, 8th, 12th steps...
The vertical position $y$ is the sum:

$$
y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \dots
$$

We can factor out $\frac{1}{2}$ from this series:

$$
y = \frac{1}{2} \left( 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \dots \right)
$$

The expression in the parentheses is the **alternating harmonic series**, which converges to $\ln(2)$:

$$
y = \frac{1}{2} \ln(2) = \ln(\sqrt{2}) \approx 0.347
$$

---

## Final Solution

The final position of the ant is the coordinates $(x, y)$:

$$
\left( \frac{\pi}{4}, \frac{\ln(2)}{2} \right) \approx (0.785, 0.347)
$$

### Summary
* **East/West Series:** Converges to $\frac{\pi}{4}$ via the Gregory-Leibniz series.
* **North/South Series:** Converges to $\frac{\ln(2)}{2}$ via the alternating harmonic series.