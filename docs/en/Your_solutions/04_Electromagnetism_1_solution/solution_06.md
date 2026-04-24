# Electric Field from a System of Two Charges

## Problem Statement
Two point charges are given:
* $q_1 = +q$ at point $(-a, 0)$
* $q_2 = +2q$ at point $(a, 0)$

Find the general field vectors, the zero field conditions, calculate the field for specific values ($a = 0.2\text{m}$, $y = 0.3\text{m}$, $q = 2\mu\text{C}$), and investigate the limit $y \gg a$.

---

## Step-by-Step Solution

### 1. General Field Vectors
According to the Superposition Principle, the total electric field is the vector sum of the fields from each charge: $\vec{E} = \vec{E}_1 + \vec{E}_2$.
The electric field vector from a point charge is $\vec{E} = k \frac{q}{r^3} \vec{r}$, where $\vec{r}$ is the distance vector from the charge to the point.

* **Vector $\vec{r}_1$ (from $-a$):** $(x+a)\hat{i} + y\hat{j}$
* **Vector $\vec{r}_2$ (from $+a$):** $(x-a)\hat{i} + y\hat{j}$

**General Field $\vec{E}(x,y)$:**
$$\vec{E}(x,y) = kq \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} + 2kq \frac{(x-a)\hat{i} + y\hat{j}}{((x-a)^2 + y^2)^{3/2}}$$

**Field on the y-axis $\vec{E}(0,y)$:** Plug in $x=0$.
$$\vec{E}(0,y) = \frac{kq}{(a^2 + y^2)^{3/2}} [a\hat{i} + y\hat{j}] + \frac{2kq}{(a^2 + y^2)^{3/2}} [-a\hat{i} + y\hat{j}]$$
Factor out common terms:
$$\vec{E}(0,y) = \frac{kq}{(a^2 + y^2)^{3/2}} [(a - 2a)\hat{i} + (y + 2y)\hat{j}]$$
**$$\vec{E}(0,y) = \frac{kq}{(a^2 + y^2)^{3/2}} [-a\hat{i} + 3y\hat{j}]$$**

**Field on the x-axis $\vec{E}(x,0)$:** Plug in $y=0$.
**$$\vec{E}(x,0) = kq \left[ \frac{(x+a)}{|x+a|^3} + \frac{2(x-a)}{|x-a|^3} \right] \hat{i}$$**

---

### 2. Zero Field Conditions ($\vec{E} = 0$)
For the total field to be zero, both $E_x = 0$ and $E_y = 0$ must be true.
* **Condition for $E_y = 0$:** The $y$-components from both charges push in the same vertical direction (both up or both down) because both charges are positive. The only way the vertical field cancels out is if we are directly on the axis connecting them. Therefore, **$y = 0$**.
* **Condition for $\vec{E} = 0$:** Since $y$ must be $0$, the zero point lies on the x-axis *between* the two charges (where their horizontal pushes directly oppose each other).
Let the distance from the $+q$ charge be $d$. The distance from the $+2q$ charge will be $(2a - d)$.
Set their magnitudes equal:
$$k\frac{q}{d^2} = k\frac{2q}{(2a - d)^2}$$
$$\frac{1}{d^2} = \frac{2}{(2a - d)^2}$$
Take the square root of both sides (the standard physics cheat code):
$$\frac{1}{d} = \frac{\sqrt{2}}{2a - d}$$
$$2a - d = d\sqrt{2}$$
$$d(\sqrt{2} + 1) = 2a \implies d = 2a(\sqrt{2} - 1)$$
To find the exact x-coordinate, start at $-a$ and add $d$:
$$x = -a + 2a(\sqrt{2} - 1) = a(2\sqrt{2} - 3) \approx -0.17a$$
**The zero field point is located at $(a(2\sqrt{2} - 3), 0)$.**

---

### 3. Calculation for Specific Values
Given: $a = 0.2\text{ m}$, $y = 0.3\text{ m}$, $q = 2\times 10^{-6}\text{ C}$, $k = 9\times 10^9$.
We need $\vec{E}(0, 0.3)$. Using the formula from Step 1:
$$\vec{E} = \frac{(9\times 10^9)(2\times 10^{-6})}{(0.2^2 + 0.3^2)^{1.5}} [-0.2\hat{i} + 3(0.3)\hat{j}]$$
$$\vec{E} = \frac{18000}{(0.13)^{1.5}} [-0.2\hat{i} + 0.9\hat{j}]$$
$$\vec{E} \approx \frac{18000}{0.04687} [-0.2\hat{i} + 0.9\hat{j}]$$
$$\vec{E} \approx 384000 [-0.2\hat{i} + 0.9\hat{j}]$$
**Vector Result:** $\vec{E} \approx -76800\hat{i} + 345600\hat{j} \text{ N/C}$
**Magnitude:** $|\vec{E}| = \sqrt{(-76800)^2 + (345600)^2} \approx 354,000 \text{ N/C}$

---

### 4. Investigating the Limit $y \gg a$ (The "Zoom-Out" Cheat Code)
What happens if we move very far away along the y-axis ($y$ is much greater than $a$)?
Look at our equation: $\vec{E}(0,y) = \frac{kq}{(a^2 + y^2)^{3/2}} [-a\hat{i} + 3y\hat{j}]$
If $y \gg a$, then $a^2$ becomes negligible compared to $y^2$. Also, the $-a\hat{i}$ term becomes negligible compared to $3y\hat{j}$.
$$\vec{E}(0,y) \approx \frac{kq}{(y^2)^{3/2}} [3y\hat{j}]$$
$$\vec{E}(0,y) \approx \frac{kq}{y^3} [3y\hat{j}] = \frac{k(3q)}{y^2} \hat{j}$$
