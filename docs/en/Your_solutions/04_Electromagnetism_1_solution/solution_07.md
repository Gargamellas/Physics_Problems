### Constant Values
* **Electron Charge ($q$):** $1.6 \times 10^{-19}\text{ C}$
* **Electron Mass ($m$):** $9.11 \times 10^{-31}\text{ kg}$
* **Given Voltage ($V$):** 5000 V
* **Given Magnetic Field ($B$):** 0.1 T

---

### Step 1: Calculating the Velocity ($v$)

The equation here is: **Electrical Energy = Kinetic Energy**
$$q \cdot V = \frac{1}{2} m v^2$$

**1. Substitute the values:**
$$(1.6 \times 10^{-19}) \cdot 5000 = 0.5 \cdot (9.11 \times 10^{-31}) \cdot v^2$$

**2. Multiply the left side (Electrical Energy):**
Multiply 1.6 by 5000:
$$8000 \times 10^{-19}$$
To make the calculation easier, we adjust the decimal (add the zeros to the exponent):
$$8 \times 10^{-16}$$

**3. Multiply the right side:**
Multiply 0.5 by 9.11:
$$4.555 \times 10^{-31}$$

**4. Final state of the equation and isolating $v^2$:**
$$8 \times 10^{-16} = 4.555 \times 10^{-31} \cdot v^2$$
$$v^2 = \frac{8 \times 10^{-16}}{4.555 \times 10^{-31}}$$

**5. Division operation:**
First, divide the regular numbers: $8 / 4.555 \approx 1.756$
Then, divide the powers of 10 (in division, the bottom exponent moves up as a negative and is added: $-16 - (-31) = 15$):
$$v^2 \approx 1.756 \times 10^{15}$$

**6. Taking the square root to find velocity ($v$):**
To make taking the square root easier, we convert the number to have an even exponent ($17.56 \times 10^{14}$).
$$v = \sqrt{17.56 \times 10^{14}}$$
$$v \approx 4.19 \times 10^7\text{ m/s}$$

---

### Step 2: Calculating the Radius ($r$)

The equation here is: **Magnetic Force = Centripetal Force**
$$q \cdot v \cdot B = \frac{m \cdot v^2}{r}$$

**1. Simplify the formula:**
Since velocity ($v$) is on both sides, we cancel one out.
$$q \cdot B = \frac{m \cdot v}{r}$$
Cross-multiply to isolate the radius ($r$):
$$r = \frac{m \cdot v}{q \cdot B}$$

**2. Substitute the values:**
$$r = \frac{(9.11 \times 10^{-31}) \cdot (4.19 \times 10^7)}{(1.6 \times 10^{-19}) \cdot 0.1}$$

**3. Multiply the numerator (top part):**
Multiply the numbers: $9.11 \cdot 4.19 \approx 38.17$
Add the exponents: $-31 + 7 = -24$
Numerator = $38.17 \times 10^{-24}$

**4. Multiply the denominator (bottom part):**
Multiply the numbers: $1.6 \cdot 0.1 = 0.16$
Denominator = $0.16 \times 10^{-19}$

**5. Final division operation:**
$$r = \frac{38.17 \times 10^{-24}}{0.16 \times 10^{-19}}$$
Divide the numbers: $38.17 / 0.16 \approx 238.56$
Subtract the exponents ($-24 - (-19) = -5$): $10^{-5}$
$$r = 238.56 \times 10^{-5}$$

**6. Convert to scientific notation:**
If we shift the decimal two places to the left, we increase the exponent by two ($-5 + 2 = -3$):
$$r = 2.38 \times 10^{-3}\text{ m}$$