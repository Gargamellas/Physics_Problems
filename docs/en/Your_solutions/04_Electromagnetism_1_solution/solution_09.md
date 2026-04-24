# Vector Lorentz Force: 3D Cross Product

## Problem Statement
A proton moves with a velocity $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) \text{ m/s}$ in a region where the magnetic field is $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) \text{ T}$. What is the magnitude of the magnetic force this charge experiences?

---

## Step-by-Step Solution

### Step 1: Identify the Variables
* **Charge ($q$):** Since it is a proton, $q = +1.6 \times 10^{-19} \text{ C}$
* **Velocity ($\vec{v}$):** $\langle 2, -4, 1 \rangle$
* **Magnetic Field ($\vec{B}$):** $\langle 1, 2, -1 \rangle$

The Vector Lorentz Force formula is:
**$$\vec{F} = q(\vec{v} \times \vec{B})$$**

### Step 2: Calculate the Cross Product ($\vec{v} \times \vec{B}$)
To multiply two 3D vectors, we use the matrix determinant method. Set it up like this:
$$
\vec{v} \times \vec{B} = 
\begin{vmatrix} 
\hat{i} & \hat{j} & \hat{k} \\ 
2 & -4 & 1 \\ 
1 & 2 & -1 
\end{vmatrix}
$$

Now, apply the "Cover and Cross-Multiply" cheat code:
* **For $\hat{i}$ (Cover column $\hat{i}$):** $((-4)(-1) - (1)(2)) = (4 - 2) = 2\hat{i}$
* **For $\hat{j}$ (Cover column $\hat{j}$ and flip the sign!):** $-((2)(-1) - (1)(1)) = -(-2 - 1) = -(-3) = +3\hat{j}$
* **For $\hat{k}$ (Cover column $\hat{k}$):** $((2)(2) - (-4)(1)) = (4 - (-4)) = 4 + 4 = 8\hat{k}$

Result of the cross product:
**$$\vec{v} \times \vec{B} = 2\hat{i} + 3\hat{j} + 8\hat{k}$$**

### Step 3: Write the Force Vector ($\vec{F}$)
Multiply the cross product by the charge of the proton ($q$):
$$\vec{F} = (1.6 \times 10^{-19}) \cdot (2\hat{i} + 3\hat{j} + 8\hat{k}) \text{ N}$$

### Step 4: Find the Magnitude ($|\vec{F}|$)
To find the magnitude (length) of a 3D vector, we use the 3D Pythagorean theorem: $\text{Magnitude} = \sqrt{x^2 + y^2 + z^2}$.
First, let's find the magnitude of the cross product vector itself:
$$|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2}$$
$$|\vec{v} \times \vec{B}| = \sqrt{4 + 9 + 64}$$
$$|\vec{v} \times \vec{B}| = \sqrt{77} \approx 8.775$$

Now multiply by the charge to get the final force magnitude:
$$|\vec{F}| = q \cdot |\vec{v} \times \vec{B}|$$
$$|\vec{F}| = (1.6 \times 10^{-19}) \cdot \sqrt{77}$$
$$|\vec{F}| \approx 14.04 \times 10^{-19} \text{ N}$$

To write this in proper scientific notation (moving the decimal one place):
**$$|\vec{F}| \approx 1.40 \times 10^{-18} \text{ N