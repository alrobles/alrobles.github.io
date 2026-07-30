# Motivation Letter — Postdoc: Terrestrial Ecosystem Modelling
## Universität Bern, Institute of Geography
### Reference: geco-004 — UP-SCALE Project

---

Dear Prof. Stocker,

I am applying for the Postdoctoral position in Terrestrial Ecosystem Modelling (geco-004) within the UP-SCALE project. I hold a PhD in Evolutionary Biology from Arizona State University (defended July 2025) and am currently a postdoctoral researcher at the University of Kansas, where I develop demographic species distribution models that integrate stochastic population dynamics with climate variability.

My interest in this position is specific and grounded in concrete technical preparation. Over the past weeks, I have been porting the SOFUN ecosystem model — the Fortran codebase underlying your group's rsofun R package — to modern C++17 under the project name **rsofuncpp** (github.com/alrobles/rsofuncpp-devel). This is not a superficial wrapper. The C++17 port preserves the full mathematical structure of the P-model and BiomeE while adding OpenMP parallelism, a Stan-based Bayesian calibration pipeline, and a CI/CD test suite that validates numerical parity against the original Fortran outputs. I undertook this work because I recognized that UP-SCALE's core challenge — integrating a hydraulics-explicit model (P-hydro) into a vegetation demography model (BiomeEP) — is fundamentally a software architecture problem. The Fortran codebase, while scientifically rigorous, presents barriers to the modular integration, collaborative development, and high-throughput calibration that modern ecosystem modeling demands.

My qualifications for the specific tasks outlined in the job description rest on three pillars.

**First, demographic modeling expertise.** My postdoctoral work at KU centers on XSDM (Berti, Robles-Fernández et al., 2026, bioRxiv), a demographic SDM that couples stochastic population dynamics with environmental time series. The mathematical structure of XSDM — cohort-based demography, vital rates as functions of environmental covariates, likelihood-based calibration — is identical to the structure of BiomeEP. I understand population dynamics models not as a user but as a developer. I am the creator and maintainer of the `xsdm` R package with a C++ backend using RcppParallel.

**Second, Fortran-to-C++ translation demonstrated.** I have previously ported the UCMINF numerical optimization library from Fortran to C++ in my `ucminfcpp` package (github.com/alrobles/ucminfcpp). I read Fortran fluently and understand the numerical patterns common to legacy earth system model code. The rsofuncpp project is a direct extension of this capability to the specific codebase your group maintains.

**Third, model-data integration and high-performance computing.** My PhD work (PNAS, 2022; Frontiers in Veterinary Science, 2021) developed machine learning frameworks that integrate phylogenetic, environmental, and geographic data to predict species interactions at global scales. I have extensive experience with HPC environments (SLURM, DuckDB for large spatial data), Bayesian inference (Stan, GenSA), and reproducible research practices. I maintain 19 open-source R and C++ packages, all with documentation and test suites.

I am transparent about what I do not yet know. I do not have a background in plant hydraulics — the physics of stomatal conductance, xylem cavitation, and water potential is new to me. However, I have already mapped the equations from your 2022 Nature Plants paper describing P-hydro onto the rsofuncpp architecture. The software is designed for this integration: P-hydro would slot into the existing C++ class hierarchy as an independent module, with the calibration pipeline already capable of accepting sap flow and ecosystem manipulation data as new observation targets. My estimate — based on having worked through both codebases — is that a functional P-hydro integration into rsofuncpp is achievable in 2–3 months of focused work, not years.

My commitment to open, collaborative software development aligns with the philosophy described on the GECO group website. My public GitHub portfolio (github.com/alrobles) includes packages for SDMs (`xsdm`, `maxentcpp`), phylogenetic methods, network analysis, and high-performance computing. I would welcome the opportunity to contribute to the GECO group's computational infrastructure.

I am a Mexican national and will require a work visa, which I understand Swiss research institutions routinely sponsor. My current position at KU is funded through August 2027, and I am available to start in Bern between September 2027 and the arranged start date.

My CV, degree certificates, and the names of two referees are enclosed. I would welcome the opportunity to discuss how my computational and software engineering skills can accelerate UP-SCALE's objectives.

Sincerely,
Ángel L. Robles-Fernández, PhD
a.l.robles.fernandez@gmail.com
https://alrobles.github.io
github.com/alrobles/rsofuncpp-devel
