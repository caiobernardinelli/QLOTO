# QLOTO: Quantum Locality-Sensitive Hashing for Orthotic Trajectory Optimization

**Application Domain:** EEG-based Brain-Computer Interfaces for Chronic Traumatic Spinal Cord Injury Rehabilitation

## Complete Literature Review and References

**A quantum-classical hybrid framework for rapid similarity search in high-dimensional EEG feature spaces, targeting non-invasive BCI rehabilitation in chronic traumatic spinal cord injury.**

---

## 🇵🇹 Português

### Nome Completo
**QLOTO** = Quantum Locality-Sensitive Hashing for Orthotic Trajectory Optimization

### Objetivo
QLOTO é um projeto de pesquisa que aplica Quantum Locality-Sensitive Hashing (QLSH) a sinais de EEG para criar interfaces cérebro-computador (BCI) não-invasivas. O foco é reabilitação de lesão medular traumática crônica através de feedback sensório-motor via exoesqueleto ou prótese robótica.

### Escopo
- Lesão medular (SCI): foco em trauma crônico (meses-anos pós-lesão)
- Técnica: QLSH (quantum + clássico) para classificação rápida de padrões EEG
- Saída: predição de intenção motora (movimento imaginado) com latência baixa
- Aplicação: reabilitação via neuroplasticidade + feedback contínuo

### Fases do Projeto
1. **Fase 1 (Mai–Jul 2026):** Revisão sistemática + datasets EEG + baseline clássico
2. **Fase 2 (Ago–Out 2026):** LSH clássico em Python + comparação SVM/kNN
3. **Fase 3 (Nov 2026–Jan 2027):** QLSH em Qiskit Aer (simulated) + preprint bioRxiv
4. **Fase 4 (Fev–Jun 2027):** Disseminação + IIN-ELS candidacy + v1.0

---

## 🇬🇧 English

### Full Name
**QLOTO** = Quantum Locality-Sensitive Hashing for Orthotic Trajectory Optimization

### Objective
QLOTO is a research project applying Quantum Locality-Sensitive Hashing (QLSH) to EEG signals for developing non-invasive brain-computer interfaces (BCI). The focus is on rehabilitation of chronic traumatic spinal cord injury via sensorimotor feedback through exoskeleton or robotic prosthesis.

### Scope
- Spinal Cord Injury (SCI): focus on chronic trauma (months-years post-injury)
- Technique: QLSH (quantum + classical) for rapid EEG pattern classification
- Output: motor intention prediction (imagined movement) with low latency
- Application: rehabilitation via neuroplasticity + continuous feedback

### Project Phases
1. **Phase 1 (May–Jul 2026):** Systematic literature review + EEG datasets + classical baseline
2. **Phase 2 (Aug–Oct 2026):** Classical LSH in Python + SVM/kNN comparison
3. **Phase 3 (Nov 2026–Jan 2027):** QLSH in Qiskit Aer (simulated) + bioRxiv preprint
4. **Phase 4 (Feb–Jun 2027):** Dissemination + IIN-ELS candidacy + v1.0

---

## 📚 Key References

### Foundational BCI + EEG + Rehabilitation (Denis Delisle Rodriguez, ISD)

- **Gonzalez-Cely et al. (2024)** — "EEG-Based Multi-Class Classification for Recognizing Pedaling Velocities: A Promising Approach for Brain-Computer Interface-Enhanced Lower-Limb Robotic Rehabilitation." *BioRob 2024*, Heidelberg. DOI: 10.1109/ICCAD60883.2024.10553756
  - Multi-class classification of motor intent from EEG (87–89% accuracy)
  - Motorized Mini-Exercise Bikes (MMEBs) for passive/active pedaling
  - Common Spatial Patterns (CSP) + CNN architecture
  - **Relevance to QLOTO:** Demonstrates baseline CNN decoder for lower-limb motor intention; QLOTO extends with LSH acceleration

- **Blanco-Díaz et al. (2024)** — "Lower-Limb Kinematic Reconstruction During Pedaling Tasks from EEG Signals Using Unscented Kalman Filter." *Computer Methods in Biomechanics and Biomedical Engineering*, Vol. 27(7), pp. 867–877. DOI: 10.1080/10255842.2023.2207705
  - Kinematic decoding (position, velocity) directly from EEG in real-time
  - Slow cortical potentials (delta band, 0.1–4 Hz) for motor control
  - Unscented Kalman Filter for state estimation
  - **Relevance to QLOTO:** Validates closed-loop EEG→kinematics mapping; critical for exoskeleton feedback

- **Blanco-Diaz et al. (2025)** — "EEG-Based Analysis of Motor Imagery and Multi-Speed Passive Pedaling: Implications for Brain–Computer Interfaces." *Signals*, Vol. 6, Article 52. https://www.mdpi.com/2624-6120/6/4/52
  - Motor imagery (MI) priming via passive pedaling (PP) sensory input
  - CNN achieves 87–89% on 4-class pedaling speeds
  - Enhanced cortical engagement through sensorimotor priming
  - **Relevance to QLOTO:** Protocol design for SCI-appropriate BCI training; extends beyond healthy subjects


### Classical BCI Benchmarks

- **Walk Again 2016** (Nature): Nicolelis et al. — 8 SCI patients, 12 months BMI + exoskeleton, neurological recovery

### Full Reference List
See [docs/REFERENCES.md](docs/REFERENCES.md) for complete literature review and additional citations.

- Expand Key References section with 3 papers (2024-2025)
- Add description of each paper's relevance to QLOTO
- Include link to docs/REFERENCES.md for full literature review
   
   These papers demonstrate state-of-the-art EEG decoding for 
   lower-limb rehabilitation (87-89% CNN accuracy).

### Full Reference List
See [docs/REFERENCES.md](docs/REFERENCES.md) for complete literature review and additional citations.
---

## 📂 Repository Structure

- **README.md** — this file
- **notebooks/** — Jupyter notebooks (exploratory code)
- **src/** — Python modules (production code)
- **data/** — datasets (PhysioNet, BCI CompIV, etc)
- **results/** — output (figures, metrics, logs)
- **paper/** — manuscript (Overleaf, LaTeX)
- **wiki/** — documentation (methods, links, learning notes)
---

## 📄 License

MIT License — see LICENSE file for details.

---

## 📧 Author

Caio — Civil Engineer, Data Engineer, BI Analyst  
Dual registration: CREA-BR, OEP-PT

---

**Last updated:** May 6, 2026
