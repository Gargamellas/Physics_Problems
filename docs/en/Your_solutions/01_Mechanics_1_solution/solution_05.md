# Relative Velocity: River Crossing Problem

## Problem Statement
A river flows east at **2 m/s**. A boat that can travel at **5 m/s** in still water wants to go directly north across the river. 
* In what direction (angle) should it head? 
* How long will it take to cross the river if it is **200 meters** wide?

---

## Step-by-Step Solution

To go directly north, the boat must angle itself upstream (west) to cancel out the eastward flow of the river. This creates a right-angled velocity vector triangle where the boat's speed in still water is the hypotenuse.

### Step 1: Find the Heading Angle
Let $\theta$ be the angle west of north that the boat needs to aim for. 
* **Opposite side (River's velocity):** 2 m/s
* **Hypotenuse (Boat's engine speed):** 5 m/s

Using trigonometry to find the angle:
$$\sin(\theta) = \frac{v_{river}}{v_{boat}}$$
$$\sin(\theta) = \frac{2}{5} = 0.4$$
$$\theta = \arcsin(0.4)$$
$$\theta \approx 23.58^\circ$$

**Answer 1:** The boat should head approximately **23.6° West of North**.

### Step 2: Find the Resultant Northward Velocity
To find out how much time it takes to cross, we first need the actual speed the boat makes heading straight across the river ($v_{y}$). We can find this using the Pythagorean theorem:
$$v_{y}^2 + v_{river}^2 = v_{boat}^2$$
$$v_{y}^2 + 2^2 = 5^2$$
$$v_{y}^2 + 4 = 25$$
$$v_{y}^2 = 21$$
$$v_{y} = \sqrt{21} \approx 4.58 \text{ m/s}$$

### Step 3: Calculate the Time to Cross
Now we use the basic kinematics formula for time, using the river's width and the boat's actual straight-across velocity.
* **Distance ($d$):** 200 meters
* **Velocity ($v_y$):** $\sqrt{21}$ m/s (approx. **4.58 m/s**)

$$t = \frac{d}{v_y}$$
$$t = \frac{200}{\sqrt{21}}$$
$$t \approx \frac{200}{4.583}$$
$$t \approx 43.64 \text{ seconds}$$

**Answer 2:** It will take approximately **43.64 seconds** to completely cross the river.