# Cyclotron Motion: Electron in a Magnetic Field

## Problem Statement
An electron is accelerated from rest through a potential difference of 5000 V. It then enters a region of uniform magnetic field B = 0.1 T, perpendicular to its velocity. What is the radius of the circular path it will follow?

---

## Step-by-Step Solution

### Step 1: List the Constants
* **Mass of Electron ($m$):** $9.11 \times 10^{-31} \text{ kg}$
* **Charge of Electron ($q$):** $1.60 \times 10^{-19} \text{ C}$
* **Voltage ($\Delta V$):** $5000 \text{ V}$
* **Magnetic Field ($B$):** $0.1 \text{ T}$

### Step 2: The "Two-Phase" Logic
This problem occurs in two distinct phases:
1. **The Electric Gun (Acceleration):** Electric Potential Energy turns into Kinetic Energy.
   $$q \Delta V = \frac{1}{2} m v^2$$
2. **The Magnetic Blender (Circular Motion):** Magnetic Force provides the Centripetal Force.
   $$q v B = \frac{m v^2}{r} \implies r = \frac{mv}{qB}$$

> **Physics Cheat Code:** Instead of calculating the messy velocity ($v$) first and then plugging it into the radius formula, we can combine them algebraically to avoid rounding errors and save time!
> Solve the first equation for $v$: $v = \sqrt{\frac{2q\Delta V}{m}}$
> Substitute into the second equation: $r = \frac{m}{qB} \sqrt{\frac{2q\Delta V}{m}}$
> Simplify to get the **Master Formula**:
> **$$r = \frac{1}{B} \sqrt{\frac{2m\Delta V}{q}}$$**

### Step 3: Plug and Chug
Now, just carefully plug the constants into our Master Formula:
$$r = \frac{1}{0.1} \sqrt{\frac{2(9.11 \times 10^{-31})(5000)}{1.60 \times 10^{-19}}}$$
$$r = 10 \cdot \sqrt{\frac{9.11 \times 10^{-27}}{1.60 \times 10^{-19}}}$$
$$r = 10 \cdot \sqrt{5.69 \times 10^{-8}}$$
$$r = 10 \cdot (2.38 \times 10^{-4})$$
**$$r = 2.38 \times 10^{-3} \text{ meters}$$**

**Final Answer:**
The radius of the circular path is **$2.38 \times 10^{-3} \text{ m}$** (which is **$2.38 \text{ mm}$**).