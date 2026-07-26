# The Lorentz-Capacity Sub-Programme (LC-Synthesis)

This repository contains the source of the synthesis paper
*The Lorentz-Capacity Sub-Programme: Projective Origin of the Lorentz Factor in
the Cosmochrony Programme* (`Beau2026lcsyn`).

## Overview

The Lorentz-capacity (LC) sub-programme answers one specific structural
question of the Cosmochrony framework: **where does the Lorentz factor
$\gamma = (1 - \beta^2)^{-1/2}$ come from, if Lorentzian geometry is not assumed
as fundamental?**

The answer is that $\gamma$ is not a kinematic postulate. It is reconstructed
from the bounded Born-Infeld capacity budget of admissible projection, then
lifted to the observer-transform structure of special relativity through the
effective Lorentzian co-metric established in the geometric branch of the
programme. This paper synthesises the six constituent papers and exhibits the
single completed chain that links them.

## The Structural Chain

$$\text{BI budget} \;\to\; F^\tau = \tfrac{1}{\gamma} \;\to\;
g^{\mu\nu} = 2\eta^{\mu\nu} \;\to\; \Lambda(\beta) \;\to\;
R(x)^2 = 1 - \epsilon(x) \;\to\; \text{finite-}q\text{ domain.}$$

A central organising distinction runs through the whole sub-programme:

- The **Born-Infeld capacity sphere** $(F^\tau)^2 + \beta^2 = 1$ is a Euclidean
  norm constraint in capacity space. It supplies the projective load $\beta$ and
  the residual clock factor $F^\tau = \sqrt{1 - \beta^2} = 1/\gamma$. It is
  **not** the Minkowski interval.
- The **effective Lorentzian metric** $g^{\mu\nu} = 2\eta^{\mu\nu}$ is supplied
  separately by the Q5b-Q11 geometric closure. The Lorentz group is the isometry
  group of this metric, **not** the symmetry group of the capacity sphere.

## Constituent Papers

| Label | Key | Main result |
|-------|-----|-------------|
| LorCap | `Beau2026n` | Lorentz mobility from projective capacity; $F^\tau = 1/\gamma$ |
| TempProj | `Beau2026tp` | Temporal residual map $F^\tau_n = \sqrt{1 - B_n^2}$; time dilation, light cone |
| LCII | `Beau2026lco2` | Fibrewise local lapse $R(x)^2 = 1 - \epsilon(x)$ |
| LC-O1 | `Beau2026lco1` | Lorentz boost $\Lambda(\beta)$; length contraction $\ell = \ell_0/\gamma$ |
| LC-O2-O1 | `Beau2026lco2o1` | **No-go**: the free-fraction law does not close the bridge; LC-O2-O1 reopened |
| LC-O3 | `Beau2026lco3` | Finite-$q$ correction $\Delta_q(n) = 4m^2/q^2$ to the Carnot identification |

## Outputs

- **Special-relativistic kinematics**: time dilation ($d\tau/dn = 1/\gamma$),
  the light cone ($B = 1 \Rightarrow F^\tau = 0$), Lorentz boosts, and length
  contraction, all reconstructed from projective capacity and the effective
  metric closure.
- **Local gravitational capacity lapse**: LCII supplies the parallel structural
  definitions $R(x)^2 = 1 - \epsilon(x)$ and $R(x)^2 = -2g_{\tau\tau}(x)$.
  Their equivalence gives a capacity-side reading of gravitational time dilation
  in the Einstein regime, but its derivation from admissibility remains open.
- **Finite-$q$ control**: the exact correction $\Delta_q(n) = 4m^2/q^2$ bounds
  the domain in which continuum Carnot estimates of the spatial load are valid.

## Status

The inertial kinematic chain is complete.
The non-homogeneous capacity-metric identification remains open.
The Lorentzian metric is inherited from Q5b-Q11, while the Born-Infeld capacity
relation comes from the admissibility budget.

| Label | Status |
|-------|--------|
| LorCap | proved (conditional on $[U]$) |
| TempProj | proved (conditional on $[U]$) |
| LCII | structural; capacity-metric bridge **open** (declared postulate, Remark 3.2) |
| LC-O1 | proved |
| LC-O2-O1 | proved no-go; bridge reopened |
| LC-O3 | proved |

## Upstream Dependencies

| Paper | Role |
|-------|------|
| Born-Infeld admissibility (`Beau2026c`, `Beau2026m`) | Unit capacity form $(F^\tau)^2 + \beta^2 = 1$ |
| Projective temporal ordering (`Beau2026pto`) | Non-decreasing temporal proxy $d\tau/dn = F^\tau$ |
| Q5b-Q11 metric closure (`Beau2026q5b`, `Beau2026q11`) | Effective co-metric $g^{\mu\nu} = 2\eta^{\mu\nu}$ |

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
