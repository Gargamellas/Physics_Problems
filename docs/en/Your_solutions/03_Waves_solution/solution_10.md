# Wave Interference: 2D Superposition Simulation

## Mathematical Model
The height (amplitude) of a wave at any point on a 2D surface is given by:
$$u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_0}|^\alpha} \sin(k |\vec{r} - \vec{r_0}| - \omega t)$$

### Breaking down the parameters:
* **$\vec{r}$**: The coordinate of the point being measured (the pixel on screen).
* **$\vec{r_0}$**: The coordinate of the wave source (where the dot is placed).
* **$|\vec{r}-\vec{r_0}|$**: The straight-line distance ($d$) from the source to the point.
* **$\alpha$**: The attenuation parameter (0 to 2). 
  * $\alpha = 0$: No energy loss (ideal 2D wave).
  * $\alpha > 0$: The wave's amplitude decreases as it travels further from the source.
* **Superposition**: When multiple sources exist, the total wave height at any point is the algebraic sum of the waves from all individual sources: $U_{total} = \sum u_i$.

## Animation Logic (Implementation Steps)
1. **Grid Setup**: Create a 2D canvas representing the coordinate space.
2. **Input Handling**: Allow the user to click the canvas to store new source coordinates ($\vec{r_0}$) in an array.
3. **Render Loop**: Use a continuous animation loop (e.g., `requestAnimationFrame`) to increment time ($t$).
4. **Pixel Calculation**: For every pixel (or small block of pixels for performance), calculate the distance to all active sources, apply the wave equation, and sum the results.
5. **Color Mapping**: Map the resulting sum (positive for wave peaks, negative for wave troughs) to a color scale to visualize the interference pattern.