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
Each NO₂ value (x) is transformed into z using a non-linear function:
z = x + a_r sin(b_r x)
where:
- (a_r = 0.05 x (r mod 7))
- (b_r = 0.3 x (r mod 5 + 1)
- r is the university roll number
For this submission:
- (a_r = 0.25)
- (b_r = 1.5)

---

## Probability Density Function
The transformed variable (z) is modeled using the following probability
density function:

p̂(z) = c · exp(−λ (z − μ)²)

---

## Parameter Estimation
The parameters μ, λ, and c are estimated using
sample statistics (Method of Moments) on the transformed data.

---

## Output Values

![Output Values](output.png)

---

## Estimated PDF Plot

![Estimated PDF Plot](pdf_plot.png)

The figure illustrates the empirical probability density function of the transformed variable \(z\),
obtained using a normalized histogram, along with the estimated parametric probability density function.
The empirical distribution exhibits a prominent peak, while the smooth estimated curve closely follows
the main trend of the data.

The alignment between the empirical and estimated distributions indicates that the chosen probability
density model effectively captures the dominant characteristics of the transformed NO₂ data.


---

## Key Observations

- The empirical probability density of the transformed variable \(z\) shows a clear dominant peak, indicating a primary mode in the data.
- The estimated parametric PDF closely follows the shape of the empirical distribution near the peak region.
- Minor deviations in the tail region are expected due to the non-linear transformation applied to the original NO₂ values.
- Overall, the estimated PDF provides a reasonable approximation of the underlying data distribution.

---

## Conclusion

In this assignment, a roll-number-parameterized non-linear transformation was applied to NO₂ concentration values.
The transformed data was modeled using a parametric probability density function, and the parameters were estimated
using sample statistics.

The comparison between the empirical distribution and the estimated PDF demonstrates that the chosen model
adequately captures the main characteristics of the transformed data. This confirms the effectiveness of the
parameter estimation approach for learning probability density functions from real-world data.

