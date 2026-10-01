# Conventions ledger

Pinned source: Cheung, Liu and Remmen, arXiv:1801.08546v3.

`source-checked` means a collaborator supplied an exact page or equation from
the pinned version. It does not mean the project has independently rederived
the statement.

## Geometric and action conventions

| Item | Source convention | Status | Evidence |
| --- | --- | --- | --- |
| Metric signature | `(-,+,+,+)` | source-checked | p. 3, footnote 1; P1013-0003 |
| Riemann tensor | `R^mu_{nu rho sigma} = d_rho Gamma^mu_{nu sigma} - d_sigma Gamma^mu_{nu rho} + Gamma^mu_{rho alpha} Gamma^alpha_{nu sigma} - Gamma^mu_{sigma alpha} Gamma^alpha_{nu rho}` | source-checked | p. 3, footnote 1; P1013-0003 |
| Ricci tensor | `R_{mu nu}=R^rho_{mu rho nu}` | source-checked | p. 3, footnote 1; P1013-0003 |
| Gravitational coupling | `kappa^2=8 pi G` | source-checked | p. 3, footnote 1; P1013-0003 |
| Two-derivative Lagrangian | `L~=R/(2 kappa^2)-F_{mu nu}F^{mu nu}/4` | source-checked | p. 3, eq. (3); P1013-0003 |

## Coefficients and physical quantities

| Quantity | Source definition | Status | Evidence |
| --- | --- | --- | --- |
| Four-dimensional coefficient dimensions | `[c1,c2,c3]=0`, `[c4,c5,c6]=-2`, `[c7,c8]=-4` | source-checked | p. 3, eq. (4), and p. 15, footnote 7; P1013-0003 |
| Rescaled coefficients | `d1,2,3=kappa^2 c1,2,3`; `d4,5,6=c4,5,6`; `d7,8=kappa^-2 c7,8` | source-checked | p. 13, eq. (27); P1013-0004 |
| Dimension of every `d_i` | `-2` | source-checked | p. 13, eq. (27); P1013-0004 |
| Rescaled mass | `m=kappa^2 M/(8 pi)` | source-checked | p. 15, eqs. (34)-(35); P1013-0003 |
| Rescaled charge | `q=kappa Q/(4 sqrt(2) pi)` | source-checked | p. 15, eqs. (34)-(35); P1013-0003 |
| Non-extremality parameter | `xi=sqrt(1-q^2/m^2)` | source-checked | p. 15, eqs. (34)-(35); P1013-0003 |
| Zeroth-order metric functions | `f~=g~=1-2m/r+q^2/r^2` | source-checked | p. 16, eqs. (37), (39); P1013-0003 |
| Outer horizon | `r_+=m+sqrt(m^2-q^2)` | source-checked | p. 16, eqs. (37), (39); P1013-0003 |

## Reproducible checks

- Multiplying the zeroth-order horizon equation by `r^2` gives
  `r^2-2mr+q^2=0`. A double root therefore requires `m^2=q^2`; on the
  `m>0, q>=0` branch, `q/m=1` and `xi=0`.
- From the definitions above, `q/m=sqrt(2) Q/(kappa M)`.
- These are algebraic consistency checks, not a higher-derivative extremality
  result or a proof of the Weak Gravity Conjecture.

## Open checks

- [ ] Derive the eight-operator parity and reduction table.
- [ ] Independently derive every coefficient shift under the allowed field redefinitions.
- [ ] Verify complete invariant combinations, including all redefinition parameters.
- [ ] Confirm that equivalent bases give the same physical extremality correction.
- [ ] Separate quoted/source-checked results from independently reproduced results.
