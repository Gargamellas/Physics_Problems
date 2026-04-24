# Young's Double-Slit Experiment: Interference Animation

## The Mathematical Model
The displacement of the resultant wave is calculated using the Principle of Superposition. The total wave $u(\vec{r},t)$ is the sum of the waves from Slit 1 and Slit 2:

$$u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_1}|} \sin(k |\vec{r} - \vec{r_1}| - \omega t) + \frac{A}{|\vec{r}-\vec{r_2}|} \sin(k |\vec{r} - \vec{r_2}| - \omega t)$$

### Survival Guide to the Variables:
* **$\vec{r_1}$ and $\vec{r_2}$**: The fixed coordinates of Slit 1 and Slit 2.
* **$|\vec{r} - \vec{r_1}|$**: The straight-line distance from Slit 1 to the pixel on the screen.
* **$d = |\vec{r_1} - \vec{r_2}|$**: The distance between the two slits.
* **$\lambda$ (Wavelength)**: Controls the wave number $k$, where $k = \frac{2\pi}{\lambda}$. 
* **Interference Fringes**:
    * **Constructive (Bright/High)**: When peaks hit peaks.
    * **Destructive (Dark/Flat)**: When peaks hit troughs, canceling each other out (forming nodes/dead zones).

## Animation Logic
To simulate this in real-time:
1. Place two static source points separated by a dynamic distance $d$.
2. Allow the user to modify $d$ and $\lambda$.
3. Loop through a pixel grid. For each pixel, calculate its distance to both slits.
4. Plug distances into the equation, sum them up, and map the result to a color scale to reveal the interference pattern (the signature "striped" effect).