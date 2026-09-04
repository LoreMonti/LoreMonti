## Lorenzo Monti

**Computational physicist — physics-informed machine learning for orbital dynamics
and the space environment.**

MSc in Physics (Theoretical Physics and Astrophysics), University of Turin —
110 cum laude. My thesis applied physics-informed neural networks to
multi-regime satellite orbit propagation. I am currently working on learned
models of **thermospheric density**, the dominant source of uncertainty in
low-Earth-orbit prediction, and preparing a paper on machine learning for
satellite orbit propagation.

I build simulators from first principles and validate them against reference
data — not notebooks, but tested packages with CI, C++ kernels where speed
matters, and physics-validation suites.

---

### Selected work

| Project | What it is |
|---|---|
| **[MHD_Neural_Operator](https://github.com/LoreMonti/MHD_Neural_Operator)** | Fourier Neural Operator surrogate for the magnetized Kelvin–Helmholtz instability, trained on a from-scratch pseudo-spectral MHD solver. Recovers the magnetic stabilization threshold in a band of parameter space held out from training (correlation 0.92 with the true growth rate), with resolution-independent rollout. |
| **[Tokamak](https://github.com/LoreMonti/Tokamak)** | End-to-end fusion reactor simulator: transport PDEs, Grad–Shafranov equilibrium, feedback control, ML surrogates. Validated against ITER parameters with 93 physics tests, CI, a pybind11 C++ kernel and a Streamlit dashboard. |
| **[Warp_Drive](https://github.com/LoreMonti/Warp_Drive)** | Numerical study of Alcubierre warp-bubble spacetimes: geometry, exotic energy budget, causal structure. |
| **[F1-strategy-engine](https://github.com/LoreMonti/F1-strategy-engine)** | Race strategy simulator: Monte Carlo analysis, ML tyre-degradation models, live safety-car re-optimisation. |
| **[Three_Body](https://github.com/LoreMonti/Three_Body)** | Sun–Earth–Jupiter system in C++ (RK4, RKCK), with energy-stability and chaotic-dynamics analysis. |
| **[Particle_EM](https://github.com/LoreMonti/Particle_EM)** | Charged-particle motion in prescribed EM fields — RK4 and Boris integrators, C++. |
| **[DM_direct_detection](https://github.com/LoreMonti/DM_direct_detection)** | WIMP direct-detection rates under the Standard Halo Model, annual modulation, Xenon vs NaI targets. |
| **[Stellar_Radius_Estimation](https://github.com/LoreMonti/Stellar_Radius_Estimation)** | Stellar radii from multi-band photometry, with Monte Carlo uncertainty propagation in JHK. |
| **[Lane_Emden_Solver](https://github.com/LoreMonti/Lane_Emden_Solver)** | Lane–Emden equation for polytropic stellar models, with Chandrasekhar mass estimation. |

### Interests

Orbit propagation and determination · thermospheric density and satellite drag ·
space situational awareness and debris · physics-informed neural networks and
neural operators · scientific machine learning

### Tools

Python (PyTorch, TensorFlow, NumPy/SciPy) · C++ · LaTeX · Git, GitHub Actions

---

Open to PhD and R&D positions in machine learning for astrodynamics and space systems.

[LinkedIn](https://www.linkedin.com/in/lorenzo-monti00) · monti.lorenzo00@gmail.com
