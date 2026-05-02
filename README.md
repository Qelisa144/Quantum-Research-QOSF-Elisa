# Automated Regime Identification for Silicon Quantum Dots

**QOSF Mentorship Program – Jan to Apr 2026**

## 🎯 Problem

Spin qubit calibration currently requires **manual identification of charge stability regions** (like triple points) in silicon quantum dot devices. This is time‑consuming and hard to scale.

This project explores whether a **hybrid quantum‑classical pipeline** can automate regime identification, starting with Single Quantum Dots (SQD) and with the potential to scale to double or triple dots.

---

## 🔧 Tools & Technologies

| Area | Tools |
|------|-------|
| Device Simulation | QTCAD (finite‑element), KLayout (GDSII layout) |
| Quantum ML | PennyLane, Quantum Kernel Embeddings |
| Classical ML baseline | Python (scikit‑learn, NumPy, Matplotlib, Pandas) |
| Environment | Jupyter Notebooks, VSCode |

---

## ⚙️ Pipeline Overview

1. **Simulate** FD‑SOI quantum dot devices using QTCAD → extract electrostatic potential data
2. **Translate** physical parameters into feature maps for quantum kernels
3. **Implement** Quantum Kernel Embeddings with PennyLane
4. **Compare** classification performance against classical baselines (SVM, random forest)
5. **Automate** regime labelling to reduce manual calibration time

---

## 📊 Key Results

- Quantum kernel method achieved `[100]%` accuracy vs classical `[100]%`

Preliminary results show competitive performance with classical methods, with potential advantages in feature space flexibility.

---

## 🚀 How to Run (optional)

```bash
git clone https://github.com/Qelisa144/qosf-silicon-dot-regime.git
cd qosf-silicon-dot-regime
pip install -r requirements.txt
jupyter notebook
