# The Lorentz-Capacity Sub-Programme (LC-Synthesis)

This repository contains the source of the synthesis paper
*The Lorentz-Capacity Sub-Programme: Projective Origin of the Lorentz Factor in
the Cosmochrony Programme* (`Beau2026lcsyn`).

## Overview

The Lorentz-capacity (LC) sub-programme answers one specific structural
question of the Cosmochrony framework: **where does the Lorentz factor
$\gamma = (1 - \beta^2)^{-1/2}$ come from, if Lorentzian geometry is not assumed
as fundamental?**

The answer is that $\gamma$ is read as the temporal residual of the bounded Born-Infeld capacity budget of
admissible projection, then placed in the observer-transform structure of special relativity through a
supplied Lorentzian co-metric of the conditional form of Q11,
$g^{\mu\nu} = \mathrm{diag}(-A_\tau, 2\lambda, 2\lambda, 2\lambda)$, whose two coefficients are independent and
fixed by no source. The link is one named hypothesis, **[H-cone]**: the light-cone speed of the co-metric
equals the Born-Infeld bound per ordering step, the coupling datum that Q11 leaves open. This paper
synthesises the six constituent papers and exhibits the conditional chain that links them.

## The Structural Chain

$$\text{BI budget} \;\to\; F^\tau = \tfrac{1}{\gamma} \;\to\;
g^{\mu\nu} \propto \eta^{\mu\nu}\ \text{and [H-cone]} \;\to\; \Lambda(\beta) \;\to\;
R(x)^2 = 1 - \epsilon(x) \;\to\; \text{finite-}q\text{ domain.}$$

A central organising distinction runs through the whole sub-programme:

- The **Born-Infeld capacity sphere** $(F^\tau)^2 + \beta^2 = 1$ is a Euclidean
  norm constraint in capacity space. It supplies the projective load $\beta$ and
  the residual clock factor $F^\tau = \sqrt{1 - \beta^2} = 1/\gamma$. It is
  **not** the Minkowski interval.
- The **effective Lorentzian metric** is supplied separately, in the conditional form of Q11; after a
  rescaling of $\tau$ it is proportional to $\eta$, and the normalisation $g^{\mu\nu} = 2\eta^{\mu\nu}$ is a
  choice of units. The Lorentz group is the isometry group of this metric, **not** the symmetry group of the
  capacity sphere.

## Constituent Papers

| Label | Key | Main result |
|-------|-----|-------------|
| LorCap | `Beau2026n` | Lorentz mobility from projective capacity; $F^\tau = 1/\gamma$ |
| TempProj | `Beau2026tp` | Temporal residual map $F^\tau_n = \sqrt{1 - B_n^2}$: values fixed by the BI sphere and the Weil filling law, identified as temporal by the splitting; time dilation under [H-cone] |
| LCII | `Beau2026lco2` | Fibrewise local lapse $R(x)^2 = 1 - \epsilon(x)$ |
| LC-O1 | `Beau2026lco1` | Lorentz boost $\Lambda(\beta)$; length contraction $\ell = \ell_0/\gamma$ |
| LC-O2-O1 | `Beau2026lco2o1` | **No-go**: the free-fraction law does not close the bridge, for any postulated $A_\tau^\infty$; LC-O2-O1 open |
| LC-O3 | `Beau2026lco3` | Finite-$q$ correction $\Delta_q(n) = 4m^2/q^2$ to the Carnot identification |

## Outputs

- **Special-relativistic kinematics**: time dilation (proper-time rate $1/\gamma$ under [H-cone]),
  the light cone ($B = 1 \Rightarrow F^\tau = 0$, reached by the exact torus load of LC-O3), Lorentz boosts, and length
  contraction, all reconstructed from projective capacity, a supplied co-metric and [H-cone].
- **Local gravitational capacity lapse**: LCII supplies the parallel structural
  definitions $R(x)^2 = 1 - \epsilon(x)$ and $R(x)^2 = g_{\tau\tau}(x)/g_{\tau\tau}^\infty$.
  Their equivalence gives a capacity-side reading of gravitational time dilation
  in the Einstein regime, but its derivation from admissibility remains open.
- **Finite-$q$ control**: the exact correction $\Delta_q(n) = 4m^2/q^2$ bounds
  the domain in which continuum Carnot estimates of the spatial load are valid.

## Status

The inertial kinematic chain is complete conditionally on a supplied co-metric and on [H-cone].
The non-homogeneous capacity-metric identification remains open.
The Lorentzian co-metric is supplied in the conditional form of Q11, while the Born-Infeld capacity
relation comes from the quadratic budget hypothesis.

| Label | Status |
|-------|--------|
| LorCap | conditional on the quadratic budget and the convergence lemma; kinematic reading under [H-cone] |
| TempProj | proved under a supplied co-metric, the identification of $B_n$ and the BI lift; time dilation under [H-cone] |
| LCII | structural; capacity-metric bridge **open** (declared postulate, Remark 3.2) |
| LC-O1 | proved for $\eta$; observer reading under a supplied co-metric and [H-cone] |
| LC-O2-O1 | proved no-go; bridge open |
| LC-O3 | proved |

## Upstream Dependencies

| Paper | Role |
|-------|------|
| Born-Infeld capacity bound (`Beau2026c`) | [A-cap]; the unit capacity form $(F^\tau)^2 + \beta^2 = 1$ is the quadratic budget hypothesis of LorCap |
| Projective temporal ordering (`Beau2026pto`) | Candidate trajectory proxy, numerically non-decreasing within tolerance; exact monotonicity conjectural; state order needs [H-acyc]; no step and no coefficient |
| Supplied co-metric (`Beau2026q5b`, `BeauQ8`, `Beau2026q11`) | Conditional form $\mathrm{diag}(-A_\tau, 2\lambda, 2\lambda, 2\lambda)$; coefficients free |
| [H-cone] | Light-cone speed equal to the Born-Infeld bound per ordering step (Q11-O1; assumed) |

## Repository Contents

```
lc-synthesis/
|-- out/              # Compiled PDF
|-- tex/
|   |-- lc-synthesis.tex
|   |-- cosmochrony-bibliography.bib
|-- compile.sh
|-- zenodo.json
|-- README.md
```

## Compilation

```bash
bash compile.sh
```

## Citation

> J. Beau, *The Lorentz-Capacity Sub-Programme: Projective Origin of the Lorentz
> Factor in the Cosmochrony Programme*, Preprint, 2026.

## Acknowledgements

Portions of the editorial refinement benefited from iterative interactions with
large language models used as analytical assistants.
All claims, interpretations, and final formulations remain the sole
responsibility of the author.
