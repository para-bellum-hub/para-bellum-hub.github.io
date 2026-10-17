---
layout: page
title: Hydrogen orbital solver
description: Hydrogen-atom wavefunctions from the Schrödinger equation, with the special-function recursions written from scratch.
img: assets/img/projects/hydrogen_orbital_320.png
importance: 4
category: projects
github: https://github.com/para-bellum-hub/hydrogen_orbital_simulator
---

**December 2024 – February 2025.** Advisor: Prof. Abhiraj Sharma, Department of Civil Engineering, IIT Roorkee. Code: [para-bellum-hub/hydrogen_orbital_simulator](https://github.com/para-bellum-hub/hydrogen_orbital_simulator).

The solver computes hydrogen-atom wavefunctions from the Schrödinger equation. The Legendre, associated Legendre and Laguerre polynomials that make up the angular and radial parts are implemented from scratch with their recurrence relations, rather than taken from a library. Three interactive Matplotlib simulators then render the results in 3D: the orbital for user-chosen quantum numbers (n, l, m), the same orbital with positive and negative lobes of the wavefunction coloured separately, and the spherical harmonics on their own.

<div class="row justify-content-sm-center">
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/hydrogen_orbital_320.png" title="3d orbital, n=3, l=2, m=0" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The n = 3, l = 2, m = 0 orbital, rendered by the signed-wavefunction simulator.
</div>
