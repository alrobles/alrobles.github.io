# Ángel Luis Robles Fernández

Postdoctoral Researcher  
Kansas Biological Survey & Center for Ecological Research  
University of Kansas, Lawrence, KS 66047  
a.l.robles.fernandez@gmail.com | https://alrobles.github.io  
ORCID: 0000-0002-4674-4270 | GitHub: github.com/alrobles

---

## Education

**2021 – 2025** — **PhD in Evolutionary Biology**, Arizona State University, School of Life Sciences  
Dissertation: *Predicting host–parasite interactions from different biodiversity dimensions through machine learning*  
Committee: Nathan Upham (Co-Chair), Nico Franz (Co-Chair), Beckett Sterner, Taichi Suzuki

**2020 – 2021** — **MSc in Physics**, Universidad Veracruzana, Faculty of Physics, Mexico

**2017** — **BSc in Physics**, Universidad Veracruzana, Faculty of Physics, Mexico

---

## Research Experience

**Sep 2024 – Present** — **Postdoctoral Researcher**, University of Kansas  
Kansas Biological Survey & Center for Ecological Research | Supervisor: Daniel C. Reuman  
- Development of XSDM: a demographic species distribution model coupling stochastic population dynamics with climate variability time series (Berti, Robles-Fernández et al., 2026, bioRxiv).  
- Creator and maintainer of the `xsdm` R package (C++ backend, RcppParallel, CRAN-ready).  
- Key result: climate variability reduces species' potential distributions by 22–45%, comparable to the effect of changes in climate means.  
- Modeling environment: Linux, HPC (SLURM), DuckDB for large spatial datasets, Stan for Bayesian calibration.

**Aug 2021 – Jul 2025** — **Research Assistant**, Arizona State University, School of Life Sciences  
- Machine learning frameworks for predicting host–parasite interactions from phylogenetic, environmental, and geographic distances. Published in PNAS (2022), Frontiers in Veterinary Science (2021), and Parasitology (2025).  
- Co-developed the Suitability Prevalence Area (SPA) method linking Quaternary environmental stability to present-day population genetic diversity (Hernández, Robles-Fernández & Upham, 2025, Ecography; co-first author).  
- Taxonomic harmonization of global mammal and parasite databases.

---

## Ecosystem Modeling Projects (Active)

**rsofuncpp** — C++17 port of the SOFUN terrestrial ecosystem model  
github.com/alrobles/rsofuncpp  
- Full C++17 rewrite of the Fortran codebase underlying the `rsofun` R package (stineb/rsofun on CRAN).  
- Preserves P-model (photosynthesis, Farquhar model) and BiomeE (vegetation demography) mathematical structure.  
- Architecture designed for modular integration of plant hydraulics (P-hydro).  
- Added OpenMP parallelism, Stan-based Bayesian calibration pipeline, CI/CD validation against Fortran outputs.  
- Target: CRAN submission as a standalone R package.

**ucminfcpp** — C++17 port of UCMINF numerical optimization library  
github.com/alrobles/ucminfcpp  
- Fortran-to-C++ translation of the UCMINF unconstrained minimization algorithm.  
- Preserves numerical accuracy and convergence properties of the original.

---

## Peer-Reviewed Publications

*First and co-first author publications marked with \**

1. **\*Hernández, N.A.H.\*, \*Robles-Fernández, Á.L.\*, & Upham, N.** (2025). Environmental suitability throughout the late Quaternary explains population genetic diversity. *Ecography*, 2025(3), e07202. \*Equal contribution.

2. **\*Robles-Fernández, Á.L., Santiago-Alarcon, D., & Lira-Noriega, A.** (2022). Wildlife susceptibility to infectious diseases at global scales. *Proceedings of the National Academy of Sciences*, 119(35), e2122851119.

3. **\*Robles-Fernández, Á.L., Santiago-Alarcon, D., & Lira-Noriega, A.** (2021). American mammals susceptibility to dengue according to geographical, environmental, and phylogenetic distances. *Frontiers in Veterinary Science*, 8, 604560.

4. **\*Robles-Fernández, Á.L. & Lira-Noriega, A.** (2017). Combining phylogenetic and occurrence information for risk assessment of pest and pathogen interactions with host plants. *Frontiers in Applied Mathematics and Statistics*, 3, 17.

5. **Krasnov, B.R., Grabovsky, V.I., Korallo-Vinarskaya, N., Vinarski, M.V., Robles-Fernandez, Á.L., & Khokhlova, I.** (2025). Geographic variation in the determinants of ectoparasite faunas' species richness. *Parasitology*, 152(7), 745–756.

6. **Tinoco-Domínguez, E., Amancio, G., Robles-Fernández, Á.L., & Lira-Noriega, A.** (2025). Interaction network of *Phoradendron* and its hosts. *American Journal of Botany*, 112(4), e70025.

7. **Velásquez-Roa, T., Hurtado-Materon, M.A., Robles-Fernández, Á.L., & Castro-Arellano, I.** (2026). Rosario: An algorithm to analyse cyclical data in ecology. *Biodiversity Data Journal*, 14, e176358.

### Preprint

8. **Berti, E., Robles-Fernández, Á.L., Rosenbaum, B., Peterson, T.A., Soberón, J., & Reuman, D.C.** (2026). The impacts of climate variability on the niche concept and distributions of species. *bioRxiv*. https://doi.org/10.1101/2024.10.30.621023

---

## Software & R Packages (19 packages, creator & maintainer)

### Ecosystem & Species Distribution Modeling
| Package | Description | Language |
|---------|-------------|----------|
| **rsofuncpp** | C++17 port of SOFUN terrestrial ecosystem model | C++ / R |
| **xsdm** | Demographic SDM with stochastic demography + climate variability | R / C++ (RcppParallel) |
| **maxentcpp** | Maxent SDM re-implemented in C++ | C++ |
| **kuenm** | Ecological niche modeling toolkit | R |
| **nicher** | Niche modeling utilities | R |
| **nicherbayes** | Bayesian niche modeling | R |

### Interaction Modeling & Phylogenetics
| Package | Description | Language |
|---------|-------------|----------|
| **ecointeraction** | Predict biotic interactions from phylogeny, environment, geography | R |
| **geotax** | Project interaction probability to geographic space | R |
| **fastJaccard** | Parallel Jaccard similarity (RcppParallel) | R / C++ |

### Data Infrastructure
| Package | Description | Language |
|---------|-------------|----------|
| **mdd** | Mammal Diversity Database range maps | R |
| **cofid** | Copepod–fish interaction database | R |
| **gbifliterature** | GBIF Literature API client | R |
| **ecoseek-bioclim** | ERA5-Land bioclimatic variables (BIO01–BIO19) | Python |
| **ecoseek-hpc-orchestrator** | Reusable SLURM templates for SDM pipelines | Shell |

### Optimization & Utilities
| Package | Description | Language |
|---------|-------------|----------|
| **ucminfcpp** | Fortran→C++ numerical optimization | C++ |
| **xplus** | Extended Positive and Unlabeled Learning | R |
| **pam** | Presence–absence matrices from shapefiles | R |
| **sobol** | Sobol sequence generation | C++ |
| **fastEukaryotyping** | Eukaryotic genotyping pipeline | R |

---

## Honors and Awards

| Date | Award | Amount |
|------|-------|--------|
| 10/2022 | **GBIF Ebbe Nielsen Challenge** — 2nd Prize | $5,000 |
| 05/2023 | Grant-in-Aid of Research, American Society of Mammalogists | $1,750 |
| 03/2022 | Leo S. Rowe Fund, Organization of American States | $15,000 |
| 10/2020 | **GBIF Young Researcher Award** | $5,000 |
| 05/2016 | 5th Young Talent Award, COVEICYDET, Mexico | $1,500 |

---

## International Conferences — Oral Presentations

- **2024** — International Biogeography Society (IBS), Prague, Czech Republic
- **2022** — American Society of Mammalogists, 101st Annual Meeting
- **2022** — International Biogeography Society (IBS), Vancouver, Canada
- **2020** — International Conference on Complex Systems, NECSI
- **2017** — International Biogeography Society (IBS), Tucson, AZ

---

## Teaching & Mentoring

- **Instructor**: Introduction to R (2017), Faculty of Physics, Universidad Veracruzana
- **Teaching Assistant**: Quantitative Ecology (2024), Statistical Models for Biology (2024), Arizona State University
- **Certification**: RStudio Certified Trainer — Tidyverse

---

## Technical Skills

**Programming:** R (expert), C++17 (advanced), Fortran (reading/modification), Python (intermediate), SQL (intermediate)  
**HPC & Data:** SLURM, DuckDB, Apache Spark, Linux (CentOS, Debian, Ubuntu)  
**Methods:** Machine learning (random forest, PU learning, gradient boosting), ecological niche modeling (Maxent, BIOCLIM, XSDM), Bayesian inference (Stan), phylogenetic comparative methods, network analysis  
**Languages:** Spanish (native), English (professional fluency)

---

*Last updated: July 2026*

---

## References

1. **Daniel C. Reuman** — Postdoctoral Supervisor  
   Professor, Department of Ecology and Evolutionary Biology  
   University of Kansas  
   reuman@ku.edu

2. **Andrés Lira-Noriega**  
   SECIHTI Research Fellow, Red de Estudios Moleculares Avanzados  
   Instituto de Ecología, A.C., Xalapa, Mexico  
   aliranoriega@gmail.com
