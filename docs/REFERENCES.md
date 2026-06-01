# QLOTO: Quantum Locality-Sensitive Hashing for Orthotic Trajectory Optimization

**Full Name:** Quantum Locality-Sensitive Hashing for Orthotic Trajectory Optimization  
**Application Domain:** EEG-based Brain-Computer Interfaces for Chronic Traumatic Spinal Cord Injury Rehabilitation

## Complete Literature Review and References

---

## Foundational Research: EEG-based BCI for Lower-Limb Rehabilitation

### Denis Delisle Rodriguez Research (ISD-IINN-ELS, Natal, Brazil)

These papers form the **core inspiration** for QLOTO, demonstrating effective EEG decoding of motor intent for rehabilitation applications.

#### 1. Multi-Class Classification of Pedaling Velocities (2024)

**Full Citation:**
> Gonzalez-Cely, A. X., Blanco-Díaz, C. F., Delisle-Rodriguez, D., & Bastos-Filho, T. F. (2024). 
> "EEG-Based Multi-Class Classification for Recognizing Pedaling Velocities: A Promising Approach for 
> Brain-Computer Interface-Enhanced Lower-Limb Robotic Rehabilitation." 
> In *Proceedings of the 2024 10th IEEE RAS/EMBS International Conference for Biomedical Robotics and 
> Biomechatronics (BioRob)* (pp. 223–228). Heidelberg, Germany.

**DOI:** 10.1109/ICCAD60883.2024.10553756  
**IEEE Xplore:** https://ieeexplore.ieee.org/document/10719823/

**Key Findings:**
- Multi-class EEG classification of 3 pedaling speeds (30, 45, 60 rpm) + rest
- Feature extraction: Common Spatial Patterns (CSP) + Power Spectral Density (PSD)
- Classifier: Convolutional Neural Network (CNN)
- **Accuracy: 87–89%** across 4 classes
- Dataset: 10 healthy subjects, Motorized Mini-Exercise Bikes (MMEBs)

**Why Important for QLOTO:**
- Establishes **baseline CNN performance** (87–89% accuracy) in EEG→motor intent mapping
- Demonstrates practical protocol using robotic devices (MMEBs) that QLOTO can extend
- Shows that CSP + CNN is competitive for pedaling classification
- **QLOTO Research Question:** Can Quantum LSH match CNN accuracy while reducing **latency** for real-time exoskeleton control?

---

#### 2. Kinematic Reconstruction from EEG (2024)

**Full Citation:**
> Blanco-Díaz, C. F., Guerrero-Mendez, C. D., Delisle-Rodriguez, D., Souza, A. F., Badue, C., 
> & Bastos-Filho, T. F. (2024). 
> "Lower-Limb Kinematic Reconstruction During Pedaling Tasks from EEG Signals Using Unscented Kalman Filter." 
> *Computer Methods in Biomechanics and Biomedical Engineering*, 27(7), 867–877.

**DOI:** 10.1080/10255842.2023.2207705  
**Full Text:** https://doi.org/10.1080/10255842.2023.2207705

**Key Findings:**
- Reconstructs **continuous kinematics** (position, velocity) from EEG in real-time
- Focus on slow cortical potentials in **delta band (0.1–4 Hz)** for motor control
- Unscented Kalman Filter (UKF) for state estimation
- Tested on pedaling rehabilitation tasks
- **Maximum accuracy:** 0.33 Pearson's r-value; SNR = 8 dB (delta band)

**Why Important for QLOTO:**
- Demonstrates **closed-loop kinematic decoding** — essential for exoskeleton feedback
- Validates slow cortical potentials as reliable motor control signals
- Opens path for **real-time trajectory prediction** (not just classification)
- **QLOTO Extension:** Use LSH/QLSH for rapid nearest-neighbor search in kinematic feature space

---

#### 3. Motor Imagery + Passive Pedaling Priming (2025)

**Full Citation:**
> Blanco-Diaz, C. F., Gonzalez-Cely, A. X., Delisle-Rodriguez, D., & Bastos-Filho, T. F. (2025). 
> "EEG-Based Analysis of Motor Imagery and Multi-Speed Passive Pedaling: Implications for Brain–Computer Interfaces." 
> *Signals*, 6(4), Article 52.

**DOI:** 10.3390/signals6040052  
**Open Access:** https://www.mdpi.com/2624-6120/6/4/52

**Key Findings:**
- **Novel protocol:** Passive Pedaling (PP) as sensory priming before Motor Imagery (MI)
- PP enhances cortical engagement during MI (spectral power increase around Cz)
- CNN architecture: **87–89% accuracy** on 4-class MI at different speeds (30, 45, 60 rpm)
- Comparison vs. baseline CSP+LDA: 67–70% accuracy (CNN wins decisively)
- Tested on 10 healthy subjects

**Why Important for QLOTO:**
- **Most recent work** — reflects current best practices in BCI protocol design
- Demonstrates that **sensorimotor priming improves EEG signal quality** for motor decoding
- Protocol is appropriate for **SCI patients** (passive pedaling used in clinical settings)
- **QLOTO Application:** Can PP-primed EEG benefit from LSH acceleration? Does it improve latency without sacrificing accuracy?

---

## Walk Again Protocol and Clinical Translation

### Miguel Nicolelis et al. (Duke University, IINN-ELS)

**Walk Again Project (2016–Present):**
> Nicolelis, M. A. L., Shokur, S., Donati, A. R. C., Campos, D. S. F., Almeida, S., Braga, V. A. S., ... & Seo, J. (2016). 
> "Training with brain-machine interfaces, visuotactile feedback, and assisted locomotion improves sensorimotor, visceral, 
> and psychological signs in chronic paraplegic patients." 
> *Nature*, 533(7601), 66–72.

**DOI:** 10.1038/nature17435  
**Nature Link:** https://www.nature.com/articles/nature17435

**Key Milestones:**
- First non-invasive brain-controlled exoskeleton for SCI patients
- 8 patients, 12 months of training
- Combined protocol: BMI + Exoskeleton + Virtual Reality + Sensory Substitution
- **Clinical outcomes:** Walking restoration, autonomic nervous system recovery, psychological improvement

**Relevance to QLOTO:**
- **Gold standard** for BCI-based SCI rehabilitation
- Establishes that multi-modal feedback (motor + sensory) is critical
- Identifies latency as a key engineering challenge (real-time exoskeleton control requires <100ms feedback)
- QLOTO targets this latency bottleneck via quantum-accelerated similarity search

---

## Quantum Computing + Machine Learning Acceleration

### Recent Quantum ML Papers (Supporting QLOTO's Technical Approach)

**QEEGNet (2026):**
> [Authors TBD]. "Quantum-Enhanced EEG Classification for Brain-Computer Interfaces." 
> *arXiv:2503.00080* (Mar 2026).

**FastLSH (2025):**
> [Authors TBD]. "Efficient Locality-Sensitive Hashing via Quantum Sampling." 
> *OpenReview ICLR 2025*.

---

## Datasets and Benchmarks

### Public EEG Datasets for BCI Research

- **BCI Competition IV (Dataset 2b):** Left/Right hand motor imagery (278 channels, 250 Hz)
  - Link: http://bnci-horizon-2020.eu/database/data-sets
  
- **PhysioNet Motor Movement/Imagery Dataset:** Large public EEG database
  - Link: https://physionet.org/content/eegmmidb/1.0.0/
  
- **Walk Again Dataset (IINN-ELS):** SCI patients + non-invasive BCI (contact IINN-ELS for access)

---

## QLOTO Research Gaps

### What Denis et al. Do Well:
✓ Accurate EEG-to-motor decoding (87–89%)  
✓ Practical protocol design (passive + active MI)  
✓ Real-time closed-loop kinematic mapping  

### What QLOTO Addresses:
✗ **Latency optimization** for embedded/edge hardware  
✗ **Quantum acceleration** of similarity search in high-dim EEG space  
✗ **Scalability** to large patient cohorts without cloud infrastructure  

---

## How to Cite QLOTO

**If you use this repository in your work, please cite:**

```bibtex
@software{bernardinelli_qloto_2026,
  title={QLOTO: Quantum Locality-Sensitive Hashing for Orthotic Trajectory Optimization},
  author={Bernardinelli, Caio},
  year={2026},
  url={https://github.com/caiobernardinelli/QLOTO},
  note={GitHub repository}
}
```

---

## Contact

**Inspired by and building on work of:**

**Prof. Denis Delisle Rodriguez**  
Institute for International Neuroscience of Natal (IINN-ELS)  
Instituto Santos Dumont, Natal, RN, Brazil  
Email: denis.rodriguez@isd.org.br  
Lattes: http://lattes.cnpq.br/7140331839822423  
Google Scholar: https://scholar.google.com.br/citations?user=axdSb0MAAAAJ

---

**Last Updated:** December 2026
