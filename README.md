# Wilkinson Polynomial

In numerical analysis, the Wilkinson polynomial typically refers to a specific polynomial that serves as a well-known test case for polynomial root-finding algorithms. It was introduced by James H. Wilkinson, a prominent mathematician and computer scientist.

The Wilkinson polynomial is defined as follows:

p(x) = (x - 1)(x - 2)(x - 3)...(x - 19)(x - 20)

This polynomial is constructed with roots at the integers from 1 to 20. However, the polynomial is often presented in a slightly modified form to highlight its properties:

p(x) = (x - 1)(x - 2)(x - 3)...(x - 18)(x - 19)(x - 20) + e

where 'e' represents a small perturbation term. The purpose of adding this term is to introduce some numerical instability and make the problem more challenging for numerical methods.

The Wilkinson polynomial is primarily used to test the accuracy and stability of polynomial root-finding algorithms. Due to the close proximity of its roots, it can be difficult for some methods to accurately determine all the roots or to handle the polynomial's behavior near the double root at x = 20.


I calculates and perturbs the coefficients of the Wilkinson polynomial, then computes the roots for different perturbation levels (epsilon values). Finally, it extracts the real and imaginary parts of the roots and plots them on a scatter plot.

After perturbing the coefficients of the Wilkinson polynomial, i observe changes in the roots of the polynomial. The perturbation introduces small variations to the coefficients, which affects the locations of the roots.

By examining the output, we can observe how the roots change as the perturbation level (epsilon) varies. The roots are calculated for different epsilon values (10^-3, 10^-4, 10^-5, 10^-6, 10^-7, and 10^-8), and the resulting roots are printed.

Now let's look at what happens after the perturbations:

Sensitivity to perturbations: The Wilkinson polynomial is known to be highly sensitive to perturbations due to the proximity of its roots. As the epsilon values decrease, the perturbations become smaller, but they still cause noticeable changes in the roots. This sensitivity highlights the numerical challenges of accurately computing roots for ill-conditioned problems.

Deviation from original roots: The perturbations cause the roots to deviate from their original positions, especially for smaller epsilon values. The closer the roots are to each other, the more likely they are to be affected by even small perturbations in the coefficients.

Stability of root-finding algorithms: The changes in the roots demonstrate the stability (or lack thereof) of root-finding algorithms when applied to the Wilkinson polynomial. Some algorithms may struggle to accurately compute the roots due to the ill-conditioning and sensitivity of the problem.
