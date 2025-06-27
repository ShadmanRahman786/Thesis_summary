<h1 align="center">🧠 Neurodegenerative Disease Detection using CNN</h1>

<p align="center">
  <b>Thesis Project</b> · <i>Detecting Alzheimer’s, Parkinson’s & FTD using Deep Learning</i><br>
  <img src="https://img.shields.io/badge/Status-Ongoing-blue?style=flat-square">
  <img src="https://img.shields.io/badge/Data-ADNI,PPMI,FTD-orange?style=flat-square">
</p>

---

## 🚀 Overview

This thesis proposes a deep learning approach for early-stage detection of **Alzheimer’s**, **Parkinson’s**, and **Frontotemporal Dementia (FTD)** from **2D sagittal MRI slices** using **pseudo-3D modeling**. A lightweight and efficient CNN architecture is built upon **MobileNetV2** with **SE attention blocks** to enhance feature representation.

> ⚠️ **Note:** Source code and raw datasets are kept private due to ethical and institutional policies.

---

## 📂 Datasets Used

| Dataset | Description | Source |
|--------|-------------|--------|
| ADNI | Alzheimer's Disease Neuroimaging Initiative | [adni.loni.usc.edu](https://adni.loni.usc.edu) |
| PPMI | Parkinson’s Progression Markers Initiative | [ppmi-info.org](https://www.ppmi-info.org/) |
| FTD | Custom pre-processed FTD dataset | Confidential |

MRI slices were extracted in **sagittal view**, preprocessed using:

- Intensity clipping to 0–255
- Conditional CLAHE for contrast
- Normalization & resizing to 224×224
- Stored in `PNG` format for CNN processing

---

## 🧠 Model Architecture

- ✅ Base: **MobileNetV2**
- ✅ Enhanced with: **Squeeze-and-Excitation (SE) Blocks**
- ✅ Input: Pseudo-3D MRI (2D slices stacked)
- ✅ Optimizer: `Adam` with LR = `1×10⁻⁵`
- ✅ Loss: `Categorical Crossentropy`

```mermaid
graph LR
A[Input MRI Slice] --> B[Preprocessing]
B --> C[MobileNetV2 + SE]
C --> D[Classification Head]
D --> E[Predicted Disease]
