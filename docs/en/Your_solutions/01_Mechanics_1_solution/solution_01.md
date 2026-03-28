# Physics I: Projectile Motion Analysis

This document provides a comprehensive step-by-step solution for a standard projectile motion problem in mechanics.

## 1. Problem Statement
A projectile is fired from the ground with:
- **Initial Velocity ($v_0$):** $100 \, \text{m/s}$
- **Launch Angle ($\theta$):** $37^\circ$
- **Assumption:** No air resistance.
- **Gravity ($g$):** $\approx 10 \, \text{m/s}^2$ (for simplicity)

---

## 2. Initial Velocity Components
First, we resolve the initial velocity into horizontal ($x$) and vertical ($y$) components using trigonometry:

* $v_{0x} = v_0 \cdot \cos(37^\circ) = 100 \cdot 0.8 = \mathbf{80 \, \text{m/s}}$
* $v_{0y} = v_0 \cdot \sin(37^\circ) = 100 \cdot 0.6 = \mathbf{60 \, \text{m/s}}$

---

## 3. Differential Equations of Motion
We derive the equations by integrating the constant acceleration due to gravity.

### Horizontal Direction ($x$):
Since there is no air resistance, acceleration $a_x = 0$.
$$\frac{d^2x}{dt^2} = 0$$
Integrating once for velocity ($v_x$):
$$\frac{dx}{dt} = v_{0x} = 80$$

### Vertical Direction ($y$):
Gravity acts downwards ($a_y = -g$).
$$\frac{d^2y}{dt^2} = -g$$
Integrating once for velocity ($v_y$):
$$v_y(t) = \frac{dy}{dt} = v_{0y} - gt = 60 - 10t$$

---

## 4. Calculations

### A. Time of Flight ($t_{flight}$)
The projectile hits the ground when the vertical displacement $y = 0$.
Integrating the velocity equation $v_y$ to get position:
$$y(t) = v_{0y}t - \frac{1}{2}gt^2$$
$$0 = 60t - 5t^2 \implies t(60 - 5t) = 0$$
$$\mathbf{t_{flight} = 12 \, \text{seconds}}$$

### B. Maximum Height ($h_{max}$)
Maximum height occurs when the vertical velocity is zero ($v_y = 0$), which happens at $t = t_{flight} / 2 = 6 \, \text{s}$.
$$h_{max} = y(6) = 60(6) - 5(6^2) = 360 - 180$$
$$\mathbf{h_{max} = 180 \, \text{meters}}$$

### C. Range ($R$)
The range is the total horizontal distance traveled during the flight.
$$R = v_{0x} \cdot t_{flight} = 80 \cdot 12$$
$$\mathbf{R = 960 \, \text{meters}}$$

---

## 5. Summary Table
| Parameter | Value |
| :--- | :--- |
| Initial Velocity | $100 \, \text{m/s}$ |
| Horizontal Velocity | $80 \, \text{m/s}$ (Constant) |
| Time of Flight | $12 \, \text{s}$ |
| Max Height | $180 \, \text{m}$ |
| Total Range | $960 \, \text{m}$ |