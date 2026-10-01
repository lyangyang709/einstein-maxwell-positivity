# Field-redefinition checks

Pinned source: Cheung, Liu and Remmen, arXiv:1801.08546v3, Appendix B,
eqs. (92)-(96). Source locations and the coefficient table below were supplied
in YourScience Workspace message P1013-0004.

## Single-parameter `r1` check

Set `r2=r3=r4=0` and choose `r1=-2 d2`, with every `d_i` on the right-hand
side denoting its value before the redefinition. The reported transformation
table gives

| Coefficient | Transformation | Result for `r1=-2 d2` |
| --- | --- | --- |
| `d1` | `d1'=d1-r1/4` | `d1+d2/2` |
| `d2` | `d2'=d2+r1/2` | `0` |
| `d3` | `d3'=d3` | `d3` |
| `d4` | `d4'=d4+r1/8` | `d4-d2/4` |
| `d5` | `d5'=d5-r1/2` | `d5+d2` |
| `d6` | `d6'=d6` | `d6` |
| `d7` | `d7'=d7` | `d7` |
| `d8` | `d8'=d8` | `d8` |

The substitutions in the last column have been independently checked by
elementary algebra. The Appendix B transformation table itself has not yet
been independently derived from the action.

## Minimal test vector

Starting from `(d1,...,d8)=(0,a,0,0,0,0,0,0)` gives

`(d1',...,d8')=(a/2,0,0,-a/4,a,0,0,0)`.

Thus choosing variables with `d2'=0` is not equivalent to deleting the
original `d2` term: compensating shifts appear in `d1`, `d4`, and `d5`.

## Invariance checks limited to this transformation

Direct substitution verifies

- `d1'+d2'/2 = d1+d2/2`,
- `d2'+d5' = d2+d5`, and
- the candidate `d9=d2+d5+d8` is unchanged under this `r1` transformation.

These checks establish invariance only under the single `r1` direction. They
do not establish invariance under the complete field-redefinition family or
physical observability. The next concrete check is the `r3` direction and its
effect on `d9`.
