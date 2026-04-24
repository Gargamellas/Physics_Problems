# Lorentz Force: Calculating Magnetic Force

## Problem Statement
A charged particle with charge $q = 2 \times 10^{-19} \text{ C}$ and mass $m = 4 \times 10^{-27} \text{ kg}$ enters a magnetic field of $B = 0.5 \text{ T}$ at a speed of $v = 10^6 \text{ m/s}$ perpendicular to the field. What is the magnitude of the Lorentz force acting on the particle?

---

## Step-by-Step Solution

### Step 1: Decode the Variables and Spot the Trap
* **Charge ($q$):** $2 \times 10^{-19} \text{ C}$
* **Speed ($v$):** $10^6 \text{ m/s}$
* **Magnetic Field ($B$):** $0.5 \text{ T}$
* **Angle ($\theta$):** $90^\circ$ (perpendicular)
* **Mass ($m$):** $4 \times 10^{-27} \text{ kg}$ $\rightarrow$ **TRAP!** We do not need the mass to find the magnetic force.

### Step 2: The Lorentz Force Formula
The magnitude of the magnetic force on a moving charge is given by the formula:
$$F = q \cdot v \cdot B \cdot \sin(\theta)$$

Since the particle enters perpendicular to the field, $\theta = 90^\circ$, and we know that $\sin(90^\circ) = 1$. The formula simplifies to:
$$F = q \cdot v \cdot B$$

### Step 3: Plug in the Values
Substitute the given numbers into the simplified formula:
$$F = (2 \times 10^{-19}) \cdot (10^6) \cdot (0.5)$$

*Cheat Code for calculation: Group the regular numbers together, and group the powers of 10 together:*
$$F = (2 \cdot 0.5) \cdot (10^{-19} \cdot 10^6)$$

Calculate the parts:
* $2 \cdot 0.5 = 1$
* $10^{-19} \cdot 10^6 = 10^{-19 + 6} = 10^{-13}$

$$F = 1 \cdot 10^{-13}$$

**Final Answer:**
The magnitude of the Lorentz force acting on the particle is **$10^{-13} \text{ N}$**.