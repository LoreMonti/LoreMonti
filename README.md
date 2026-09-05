## Lorenzo Monti

**Computational physicist — physics-informed machine learning for orbital dynamics
and physical systems.**

MSc in Physics (Theoretical Physics and Astrophysics), University of Turin —
110 cum laude. My thesis applied physics-informed neural networks to
multi-regime satellite orbit propagation, reproducing a Cowell reference
propagator to within 1% and generalising to satellites unseen in training
(0.03%–0.67% relative error); a paper on that work is in preparation.

My current project asks a sharper version of the same question: can a learned
operator recover *physics* rather than interpolate data? Trained on a band of
parameter space that deliberately excludes the magnetic stabilization threshold
of a Kelvin–Helmholtz instability, a Fourier Neural Operator reconstructs the
growth-rate curve inside that unseen band and assigns the correct stability
verdict to 97% of held-out runs.

I build simulators from first principles and validate them against reference
data — not notebooks, but tested packages with CI, C++ kernels where speed
matters, and physics-validation suites.

---

### Selected work

| Project | What it is |
|---|---|
| **[MHD Neural Operator](https://github.com/LoreMonti/MHD_Neural_Operator)** | A Fourier Neural Operator emulating a magnetized Kelvin–Helmholtz instability, tested on a held-out band of parameter space around the magnetic stabilization threshold. Includes the from-scratch pseudo-spectral MHD solver that generates the ground truth — and a documented account of the two loss functions that failed first. |
| **[Tokamak](https://github.com/LoreMonti/Tokamak)** | End-to-end fusion reactor simulator: transport PDEs, Grad–Shafranov equilibrium, feedback control, ML surrogates. Validated against ITER parameters with 93 physics tests, CI, a pybind11 C++ kernel and a Streamlit dashboard. |
| **[Three_Body](https://github.com/LoreMonti/Three_Body)** | Sun–Earth–Jupiter system in C++ (RK4, RKCK), with energy-stability and chaotic-dynamics analysis. |
| **[Stellar_Radius_Estimation](https://github.com/LoreMonti/Stellar_Radius_Estimation)** | Stellar radii from multi-band photometry, with Monte Carlo uncertainty propagation and formal consistency tests against reference measurements. |
| **[Warp_Drive](https://github.com/LoreMonti/Warp_Drive)** | Numerical study of Alcubierre warp-bubble spacetimes: geometry, exotic energy budget, causal structure. |
| **[F1-strategy-engine](https://github.com/LoreMonti/F1-strategy-engine)** | Race strategy simulator: Monte Carlo analysis, ML tyre-degradation models, live safety-car re-optimisation. |
| **[Particle_EM](https://github.com/LoreMonti/Particle_EM)** | Charged-particle motion in prescribed EM fields — RK4 and Boris integrators, C++. |
| **[DM_direct_detection](https://github.com/LoreMonti/DM_direct_detection)** | WIMP direct-detection rates under the Standard Halo Model, annual modulation, Xenon vs NaI targets. |
| **[Lane_Emden_Solver](https://github.com/LoreMonti/Lane_Emden_Solver)** | Lane–Emden equation for polytropic stellar models, with Chandrasekhar mass estimation. |

### Interests

Orbit propagation and determination · space situational awareness and debris ·
thermospheric density and satellite drag · physics-informed neural networks and
neural operators · scientific machine learning

### Tools

Python (PyTorch, TensorFlow, NumPy/SciPy) · C++ · LaTeX · Git, GitHub Actions

---

Open to PhD and R&D positions in machine learning for astrodynamics and space systems.

[LinkedIn](https://www.linkedin.com/in/lorenzo-monti00) · monti.lorenzo00@gmail.com
