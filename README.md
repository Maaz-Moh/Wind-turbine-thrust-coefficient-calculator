# Wind-turbine-thrust-coefficient-calculator
it’s a small physics-based toolkit that computes a wind turbine’s thrust coefficient (C_T) and the corresponding axial induction factor (a) using simple 1‑D actuator‑disk / momentum‑theory formulas.
```markdown
# Thrust Coefficient Utility

This small Python module provides functions to compute the wind-turbine thrust coefficient (C_T)
from simple momentum theory (actuator-disk) relations and to convert between thrust and
axial-induction factor `a`.

Quick reference:
 - C_T = 4 a (1 - a)
 - C_T = T / (0.5 * rho * A * U^2)
 - a = (1 - sqrt(1 - C_T)) / 2   (physical, low-induction branch)

Limitations:
 - The 1D momentum relations are valid for moderate axial induction (a typically < ~0.3).
 - For highly loaded rotors (large a) or when blade geometry matters, use Blade-Element Momentum (BEM)
   with tip-loss and empirical (Glauert) corrections. This tool does not implement full BEM.
 - If you want a BEM implementation, provide blade geometry (radius grid, chord, twist),
   the number of blades, rotational speed / tip-speed ratio, and airfoil lift/drag polars.
```
