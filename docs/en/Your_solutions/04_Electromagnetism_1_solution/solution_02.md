# Electric Potential: Center of a Square

## Problem Statement
Point charges of +1C, -2C, +3C, and -4C are placed at the corners of a square with sides of 1.0 m (in order). Calculate the electric potential at the center of the square.

---





### Step 1: Find the Distance to the Center ($r$)
First, we need the distance from any corner of the square to its center. 
Using the Pythagorean theorem for a square with side $a = 1.0 \text{ m}$, the diagonal is $a\sqrt{2}$. The distance to the center ($r$) is half of the diagonal:
$$r = \frac{1.0 \cdot \sqrt{2}}{2} = \frac{\sqrt{2}}{2} \text{ meters}$$

### Step 2: Use the Superposition Principle for Potential
The total electric potential at the center is the algebraic sum of the potentials from all four individual charges:
$$V_{total} = V_1 + V_2 + V_3 + V_4$$

The formula for the electric potential of a single point charge is $V = k \frac{q}{r}$. Since $k$ (Coulomb's constant) and $r$ (distance to center) are the exact same for all four charges, we can factor them out:
$$V_{total} = \frac{k}{r} (q_1 + q_2 + q_3 + q_4)$$

### Step 3: Plug in the Values
Now, just add the charges together (like money in a bank account, keeping the signs):
* Sum of charges = $(+1) + (-2) + (+3) + (-4) = -2 \text{ C}$

Substitute the sum and the distance ($r$) into our factored equation:
$$V_{total} = \frac{k}{\frac{\sqrt{2}}{2}} \cdot (-2)$$

### Step 4: Simplify the Math
When dividing by a fraction, we flip it and multiply:
$$V_{total} = k \cdot \frac{2}{\sqrt{2}} \cdot (-2)$$
$$V_{total} = \frac{-4k}{\sqrt{2}}$$

To rationalize the denominator (multiply top and bottom by $\sqrt{2}$):
$$V_{total} = -2\sqrt{2}k$$

**Final Answer:**
The total electric potential at the center of the square is **$-2\sqrt{2}k$ Volts** (where $k \approx 8.99 \times 10^9 \text{ N m}^2/\text{C}^2$).