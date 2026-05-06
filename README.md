# QLOTO

## Quantum Locality-Sensitive Hashing for EEG-based Brain-Computer Interfaces

**A quantum-classical hybrid framework for rapid similarity search in high-dimensional EEG feature spaces, targeting non-invasive BCI rehabilitation in chronic traumatic spinal cord injury.**

---

## 🇵🇹 Português

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

- **Walk Again 2016** (Nature): Nicolelis et al. — 8 SCI patients, 12 months BMI + exoskeleton, neurological recovery
- **QEEGNet** (arXiv 2503.00080, Mar 2026) — Quantum EEG classification for BCI
- **FastLSH** (OpenReview ICLR 2025) — Efficient locality-sensitive hashing

---

## 📂 Repository Structure
QLOTO/
├── README.md (this file)
├── notebooks/ (Jupyter notebooks — exploratory code)
├── src/ (Python modules — production code)
├── data/ (datasets — PhysioNet, BCI CompIV, etc)
├── results/ (output — figures, metrics, logs)
├── paper/ (manuscript — Overleaf, LaTeX)
└── wiki/ (documentation — methods, links, learning notes)
---

## 📄 License

MIT License — see LICENSE file for details.

---

## 📧 Author

Caio — Civil Engineer, Data Engineer, BI Analyst  
Dual registration: CREA-BR, OEP-PT

---

**Last updated:** May 6, 2026