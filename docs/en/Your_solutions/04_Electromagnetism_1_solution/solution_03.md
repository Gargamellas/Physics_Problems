# Electrostatic Equilibrium: Finding the Balance Point

## Problem Statement
Find the equilibrium position for a charge $q_3 = +1\text{C}$ placed on the line between a charge $q_1 = +4\text{C}$ and a charge $q_2 = +9\text{C}$, which are separated by a distance of 2 m.

---

## Step-by-Step Solution

### Step 1: Set Up the Logic
For $q_3$ to be in equilibrium, the electric force pushing it to the right (from $q_1$) must perfectly balance the electric force pushing it to the left (from $q_2$). 
* Let $q_1$ be at position $x = 0$.
* Let $q_2$ be at position $x = 2$.
* Let $q_3$ be at an unknown distance $x$ from $q_1$.
* Therefore, the distance from $q_3$ to $q_2$ is $(2 - x)$.

### Step 2: Set the Forces Equal ($F_1 = F_2$)
Using Coulomb's Law ($F = k \frac{q_a q_b}{r^2}$):
$$k \frac{q_1 \cdot q_3}{x^2} = k \frac{q_2 \cdot q_3}{(2 - x)^2}$$



$$\frac{q_1}{x^2} = \frac{q_2}{(2 - x)^2}$$

### Step 3: Plug in the Values and Solve
Substitute $q_1 = 4$ and $q_2 = 9$:
$$\frac{4}{x^2} = \frac{9}{(2 - x)^2}$$



$$\sqrt{\frac{4}{x^2}} = \sqrt{\frac{9}{(2 - x)^2}}$$
$$\frac{2}{x} = \frac{3}{2 - x}$$

### Step 4: Cross-Multiply
Now it is a simple linear equation:
$$2 \cdot (2 - x) = 3 \cdot x$$
$$4 - 2x = 3x$$
$$4 = 5x$$
$$x = \frac{4}{5} = 0.8 \text{ meters}$$

**Final Answer:**
The equilibrium position is **0.8 meters** away from the $q_1$ (+4C) charge.