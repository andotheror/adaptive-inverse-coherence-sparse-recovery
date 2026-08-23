# Adaptive Inverse Coherence for Sparse Recovery

## Abstract

Let $X\in\mathbb R^{n\times d}$ have independent $N(0,1/n)$ entries. After observing
$X$, an adversary chooses a $k$-sparse signal $\theta^\star$ and noise $\xi$,
then the learner observes $y=X\theta^\star+\xi$. Recent work proved that
$n\gtrsim k^2\log(d/k)$ measurements suffice for
$\\|\widehat\theta-\theta^\star\\|_\infty=O(\\|X^\top\xi\\|_\infty)$, but its lower
bound was $n\gtrsim k^2$. We close the logarithmic gap.

The main ingredient is a sharp random-matrix law. If
$L=\log(ed/s)$ and $n\gtrsim sL$, then with high probability

$$\max_{|S|\leq s}\\\\\\|(X_S^\top X_S)^{-1}\\\\\\|_{\infty\to\infty}
 \asymp 1+s\sqrt{L/n}.$$

For the lower bound, one anchor column selects the columns having the largest
absolute correlations with it. Gaussian orthogonal decomposition leaves the
selected residual columns independent. An exact Schur complement then exposes
an inverse row with no perturbation remainder. The same decomposition controls
all unselected correlations even though the support depends on the full design.

For every constant approximation factor, no estimator succeeds with probability
$3/4$ when $n$ is below a sufficiently small constant times
$k^2\log(ed/k)$. The result also yields the same lower threshold for exact
variable selection. Together with the known upper bound, the adaptive Gaussian
measurement complexity is $\Theta(k^2\log(ed/k))$ at constant confidence.

## Keywords

sparse recovery, compressed sensing, random matrix theory, adversarial noise, inverse coherence, sample complexity, minimax lower bounds

## Files

- `main_2026-08-13.pdf`, the paper as first published, with its OpenTimestamps proof `main_2026-08-13.pdf.ots`.
- source: `aistats2027.sty`, `main_2026-08-13.tex`, `references.bib`.
- also: `main_2026-08-13.bbl`.
