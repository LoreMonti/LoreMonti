## Lorenzo Monti

**Computational physicist — physics-informed machine learning for orbital dynamics
and physical systems.**

MSc in Physics (Theoretical Physics and Astrophysics), University of Turin —
110 cum laude. My thesis applied physics-informed neural networks to
multi-regime satellite orbit propagation, from LEO to GEO: trained on JPL
Horizons ephemerides, it kept the position error over one orbit below 1% and
generalised to spacecraft unseen in training (0.03%–0.67%); a paper on that
work is in preparation.

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
| **[Booster_Landing](https://github.com/LoreMonti/Booster_Landing)** | Powered descent of a reusable first stage in Simulink: 3-DOF plant, gimbal attitude loop, hoverslam guidance under a 40 % minimum throttle, PD versus LQR lateral control. 1000 of 1000 Monte Carlo landings meet the touchdown requirements; 99th-percentile miss 1.9 m. |
| **[Orbital_Rendezvous](https://github.com/LoreMonti/Orbital_Rendezvous)** | Docking a chaser spacecraft in the Clohessy–Wiltshire frame, held against LQR and the classical V-bar procedure on 200 unseen starts. A PPO agent docks 199 of 200; through a narrow docking port, a planner tracking exact manoeuvres docks 198 of 200 on 1.11 m/s. |
| **[MHD_Neural_Operator](https://github.com/LoreMonti/MHD_Neural_Operator)** | Fourier Neural Operator surrogate for a magnetized Kelvin–Helmholtz instability, trained on a from-scratch pseudo-spectral MHD solver. On a held-out band around the magnetic stabilization threshold, it gives the correct stability verdict for 97 % of runs. |
| **[Tokamak](https://github.com/LoreMonti/Tokamak)** | End-to-end fusion reactor simulator built from first principles: transport PDEs, Grad–Shafranov equilibrium, feedback control and ML surrogates, with a pybind11 C++ kernel. Validated against ITER parameters with 93 physics tests and CI. |
| **[Three_Body](https://github.com/LoreMonti/Three_Body)** | Sun–Earth–Jupiter system in C++, fixed-step RK4 against adaptive Runge–Kutta–Cash–Karp. Under strong perturbations only the adaptive step stays physical; the N-body extension to Pluto conserves energy to a few parts per million over 250 years. |
| **[Particle_EM](https://github.com/LoreMonti/Particle_EM)** | Charged-particle motion in prescribed electromagnetic fields in C++, RK4 against the Boris pusher, checked on gyration, E×B drift and a magnetic X-point. Over long runs the Boris energy error stays bounded near 1e-14, while RK4 drifts without bound. |
| **[Warp_Drive](https://github.com/LoreMonti/Warp_Drive)** | Numerical study of Alcubierre and Van Den Broeck warp-bubble spacetimes: exotic energy budget, horizons and null-geodesic ray tracing of the sky seen from inside the bubble, with quantum-inequality checks and an acoustic analogue in a Bose–Einstein condensate. |
| **[F1-strategy-engine](https://github.com/LoreMonti/F1-strategy-engine)** | Formula 1 lap-time simulator calibrated on real timing data (FastF1), with a Monte Carlo engine for safety cars and a strategy optimiser. It reproduces the real Monza tyre degradation (0.065 s/lap) and picks the one-stop strategy Leclerc won on. |
| **[Stellar_Radius_Estimation](https://github.com/LoreMonti/Stellar_Radius_Estimation)** | Radii of stars hosting transiting planets from multi-band photometry, with Monte Carlo propagation of the uncertainties in the J, H and K bands, formal consistency tests against reference radii and automatic detection of outliers. |
| **[DM_direct_detection](https://github.com/LoreMonti/DM_direct_detection)** | Direct-detection event rates for a 70 GeV WIMP under the Standard Halo Model, with the Helm nuclear form factor and the annual modulation from the Earth's orbit, comparing xenon and NaI targets. |
| **[Lane_Emden_Solver](https://github.com/LoreMonti/Lane_Emden_Solver)** | Lane–Emden equation for polytropic stars solved with RK4 for n = 0, 1, 3/2, 3 and 5, validated against the analytical solutions, with the Chandrasekhar mass of a relativistic white dwarf from the n = 3 polytrope. |

### Interests

Reinforcement learning and classical control for guidance and landing · orbit propagation and determination · space situational awareness and debris · thermospheric density and satellite drag · physics-informed neural networks and
neural operators · scientific machine learning

### Tools

Python (PyTorch, TensorFlow, Stable-Baselines3, Gymnasium, NumPy/SciPy) · MATLAB/Simulink · C++ · LaTeX · Git, GitHub Actions

---

Open to PhD and R&D positions in machine learning for astrodynamics and space systems, and to a six-month internship (April–September 2027) in GNC, flight dynamics or mission analysis.

[LinkedIn](https://www.linkedin.com/in/lorenzo-monti00) · monti.lorenzo00@gmail.com
