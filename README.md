## Lorenzo Monti

**Computational physicist — physics-informed machine learning for orbital dynamics
and physical systems.**

MSc in Physics (Theoretical Physics and Astrophysics), University of Turin —
110 cum laude. My thesis applied physics-informed neural networks to
multi-regime satellite orbit propagation, reproducing a Cowell reference
propagator to within 1% and generalising to satellites unseen in training
(0.03%–0.67% relative error); a paper on that work is in preparation.

My research question is a sharper version of the same one: can a learned
model recover *physics* rather than interpolate data? In one project, a Fourier
Neural Operator trained on a band of parameter space that deliberately excludes
the magnetic stabilization threshold of a Kelvin–Helmholtz instability
reconstructs the growth-rate curve inside that unseen band and assigns the
correct stability verdict to 97% of held-out runs. In my latest ones, a PPO agent
learns an orbital rendezvous from scratch and is held against the classical
controllers on starting points it never saw, and a reusable booster is landed
in Simulink under thrust, wind and sensor errors the guidance does not know about.

I build simulators from first principles and validate them against reference
data — not notebooks, but tested packages with CI, C++ kernels where speed
matters, and physics-validation suites.

---

### Selected work

| Project | What it is |
|---|---|
| **[Orbital_Rendezvous](https://github.com/LoreMonti/Orbital_Rendezvous)** | Learning to dock a chaser spacecraft in the Clohessy–Wiltshire relative frame, with every result held against LQR and the classical V-bar procedure on 200 unseen starts. A PPO agent docks 199 of 200 in two minutes of training; through an oriented port, Go-Explore planning reaches 198 of 200, and a graph of exact manoeuvres tracked by a short-horizon planner reaches 198 of 200 on 1.11 m/s, also on a Kalman estimate with sensor and thrust errors. Four networks distilled from that pilot dock 197 of 200. Written up with the failures included. |
| **[MHD Neural Operator](https://github.com/LoreMonti/MHD_Neural_Operator)** | A Fourier Neural Operator emulating a magnetized Kelvin–Helmholtz instability, tested on a held-out band of parameter space around the magnetic stabilization threshold. Includes the from-scratch pseudo-spectral MHD solver that generates the ground truth — and a documented account of the two loss functions that failed first. |
| **[Booster_Landing](https://github.com/LoreMonti/Booster_Landing)** | Powered descent of a reusable first stage in Simulink: planar 3-DOF plant, gimbal attitude loop, hoverslam guidance that lights the engine as late as a 40 % minimum throttle allows, and PD versus LQR lateral control with a wind disturbance observer. Every model is checked against closed forms; 1000 of 1000 Monte Carlo landings meet the touchdown requirements, 99th-percentile miss 1.9 m. |
| **[Tokamak](https://github.com/LoreMonti/Tokamak)** | End-to-end fusion reactor simulator: transport PDEs, Grad–Shafranov equilibrium, feedback control, ML surrogates. Validated against ITER parameters with 93 physics tests, CI, a pybind11 C++ kernel and a Streamlit dashboard. |
| **[Warp_Drive](https://github.com/LoreMonti/Warp_Drive)** | Numerical study of Alcubierre and Van Den Broeck warp-bubble spacetimes: exotic energy budget, horizons, null-geodesic ray tracing of the sky seen from inside the bubble, the throat of the Van Den Broeck pocket with its energy floor and quantum-inequality checks, and an acoustic analogue in a Bose–Einstein condensate. |
| **[F1-strategy-engine](https://github.com/LoreMonti/F1-strategy-engine)** | Race strategy simulator: Monte Carlo analysis, ML tyre-degradation models, live safety-car re-optimisation. |
| **[Three_Body](https://github.com/LoreMonti/Three_Body)** | Sun–Earth–Jupiter system in C++ (RK4, RKCK), with energy-stability and chaotic-dynamics analysis. |
| **[Stellar_Radius_Estimation](https://github.com/LoreMonti/Stellar_Radius_Estimation)** | Stellar radii from multi-band photometry, with Monte Carlo uncertainty propagation and formal consistency tests against reference measurements. |
| **[Particle_EM](https://github.com/LoreMonti/Particle_EM)** | Charged-particle motion in prescribed EM fields — RK4 and Boris integrators, C++. |
| **[DM_direct_detection](https://github.com/LoreMonti/DM_direct_detection)** | WIMP direct-detection rates under the Standard Halo Model, annual modulation, Xenon vs NaI targets. |
| **[Lane_Emden_Solver](https://github.com/LoreMonti/Lane_Emden_Solver)** | Lane–Emden equation for polytropic stellar models, with Chandrasekhar mass estimation. |

### Interests

Orbit propagation and determination · reinforcement learning and classical control for guidance and landing · space situational awareness and debris ·
thermospheric density and satellite drag · physics-informed neural networks and
neural operators · scientific machine learning

### Tools

Python (PyTorch, TensorFlow, Stable-Baselines3, Gymnasium, NumPy/SciPy) · MATLAB/Simulink · C++ · LaTeX · Git, GitHub Actions

---

Open to PhD and R&D positions in machine learning for astrodynamics and space systems, and to a six-month internship (April–September 2027) in GNC, flight dynamics or mission analysis.

[LinkedIn](https://www.linkedin.com/in/lorenzo-monti00) · monti.lorenzo00@gmail.com
