# Kinematics: Velocity and Acceleration Vectors

## Problem Statement
The position of an object is given by the vector function:
$$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$$

**Objective:** Find the object's velocity ($\vec{v}$) and acceleration ($\vec{a}$) vectors as a function of time.

---

## Step-by-Step Solution

In kinematics, the relationship between position, velocity, and acceleration is defined by derivatives with respect to time ($t$). Since this is a 2D vector, we differentiate the $\hat{i}$ (x-axis) and $\hat{j}$ (y-axis) components separately.

### Step 1: Find the Velocity Vector $\vec{v}(t)$
Velocity is the first derivative of the position vector with respect to time:
$$\vec{v}(t) = \frac{d}{dt} \vec{r}(t)$$

Taking the derivative of each component:
* **$\hat{i}$ component:** $\frac{d}{dt}(3t^2) = 6t$
* **$\hat{j}$ component:** $\frac{d}{dt}(5t - 8t^2) = 5 - 16t$

Combining them gives the velocity vector:
**$$\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$$**

### Step 2: Find the Acceleration Vector $\vec{a}(t)$
Acceleration is the first derivative of the velocity vector (or the second derivative of position) with respect to time:
$$\vec{a}(t) = \frac{d}{dt} \vec{v}(t)$$

Taking the derivative of the velocity components:
* **$\hat{i}$ component:** $\frac{d}{dt}(6t) = 6$
* **$\hat{j}$ component:** $\frac{d}{dt}(5 - 16t) = -16$

Combining them gives the acceleration vector:
**$$\vec{a}(t) = 6\hat{i} - 16\hat{j}$$**

---

## Final Answer
* **Velocity:** $\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$
* **Acceleration:** $\vec{a}(t) = 6\hat{i} - 16\hat{j}$