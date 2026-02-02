# Probability Density Functions Assignment – UCS654

This repository contains the solution for Assignment-1 of UCS654.
The objective of this assignment is to learn the parameters of a
probability density function using a roll-number-parameterized
non-linear transformation.

---

## Dataset

**India Air Quality Dataset**

- Feature used: **NO₂ concentration**
- Dataset file: `data.csv`

---

## Transformation

Each NO₂ value \(x\) is transformed into \(z\) using a non-linear function:

\[
z = x + a_r \sin(b_r x)
\]

where:

- \(a_r = 0.05 \times (r \bmod 7)\)
- \(b_r = 0.3 \times (r \bmod 5 + 1)\)
- \(r\) is the university roll number

For this submission:
- \(a_r = 0.25\)
- \(b_r = 1.5\)

---

## Probability Density Function

The transformed variable \(z\) is modeled using the following probability
density function:

\[
\hat{p}(z) = c \cdot \exp\left(-\lambda (z - \mu)^2\right)
\]

---

## Parameter Estimation

The parameters \(\mu\), \(\lambda\), and \(c\) are estimated using
sample statistics (Method of Moments) on the transformed data.

---

## Output Values

