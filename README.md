# Probability Density Function Estimation - Assignment

## Objective

Estimate parameters of the probability density function:

p̂(z) = c · exp( -λ (z − μ)² )

using NO₂ values from the India Air Quality dataset.

------------------------------------------------------------------------

## Roll Number

102303007

Derived constants: a = 0.10\
b = 0.9

Transformation applied: z = x + 0.10 sin(0.9x)

------------------------------------------------------------------------

## Method

1.  Extract NO₂ numeric column from dataset
2.  Remove missing and invalid values
3.  Apply nonlinear transformation to obtain z
4.  Estimate Gaussian parameters using: μ = mean(z) σ² = variance(z)
5.  Convert: λ = 1 / (2σ²) c = 1 / (σ√(2π))

------------------------------------------------------------------------

## Final Parameters

λ = 0.0014851749
μ = 25.79786847
c = 0.02174271934

------------------------------------------------------------------------

## Notes

Population variance used (division by n). No machine learning models
were required.
