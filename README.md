<h1 align="center">🧠 Neurodegenerative Disease Detection using CNN</h1>

<p align="center">
  <b>🎓 Undergraduate Thesis Project (Completed)</b><br>
  <i>Alzheimer’s, Parkinson’s & FTD Detection from MRI using Deep Learning</i><br><br>
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/Data-ADNI,PPMI,FTD-orange?style=flat-square">
  <img src="https://img.shields.io/badge/Model-SadNetV1-green?style=flat-square">
</p>

---

## 🚀 Overview

This research focuses on the early diagnosis of Alzheimer’s, Parkinson’s, and Frontotemporal Dementia (FTD) using 2D sagittal MRI slices with a pseudo-3D deep learning approach. The architecture leverages a lightweight MobileNetV2 backbone enhanced with Squeeze-and-Excitation (SE) attention blocks for efficient and interpretable classification.

> 🧾 Status: Thesis successfully submitted and defended at BRAC University, CSE Department.

> ⚠️ Note: Code and datasets are kept private to uphold ethical and institutional regulations.

---

## 📂 Datasets Used

- **ADNI**: Alzheimer's Disease Neuroimaging Initiative — https://adni.loni.usc.edu  
- **PPMI**: Parkinson’s Progression Markers Initiative — https://www.ppmi-info.org/  
- **FTD**: Neuroimaging in Frontotemporal Dementia — https://ida.loni.usc.edu  

MRI slices were processed using:
- Intensity clipping to range 0–255
- Conditional CLAHE for contrast enhancement
- Resizing to 224×224 resolution
- Normalization
- Stored as .png files for CNN input

---

## 🧪 Data Preprocessing Pipeline

![Pre_Processing_flow_chart drawio](https://github.com/user-attachments/assets/626cc488-7ec5-486b-864a-592694cbefba)

---

## 🔧 Proposed Model Workflow

![Work_Flow_Diagramof_Custom_Model drawio](https://github.com/user-attachments/assets/31602497-0db4-4f0f-9d06-38f9df7dfa15)

---

## 🧠 Model Architecture

- Base Model: MobileNetV2
- Enhancement: Squeeze-and-Excitation (SE) Attention Blocks
- Input Type: Pseudo-3D (Stacked 2D sagittal MRI slices)
- Optimizer: Adam (Learning rate = 1×10⁻⁵)
- Loss Function: Categorical Crossentropy

```mermaid
graph LR
A[Input MRI Slice] --> B[Preprocessing]
B --> C[MobileNetV2 + SE]
C --> D[Classification Head]
D --> E[Predicted Disease]
```

---

## 📊 Performance Summary

Our Proposed SadnetV1 gave us a solid result to detect Alzheimer's, Parkinson's and Fronto Temporal Dementia like-
Test- 96.15%
Validate- 97.11%
train- 96.84%
---

## 📈 Results & Visualizations

<p>Accuracy graph</p>
<img width="718" alt="Screenshot 2025-06-27 at 6 07 22 PM" src="https://github.com/user-attachments/assets/3549ab69-192d-40a6-ad66-80da3b83bb07" />
<p>Loss graph</p>
<img width="719" alt="Screenshot 2025-06-27 at 6 07 37 PM" src="https://github.com/user-attachments/assets/dcf23989-f534-4ef9-9bc7-8474860c57e1" />
<p>Test confusion matrix</p>
<img width="439" alt="Screenshot 2025-06-27 at 6 07 56 PM" src="https://github.com/user-attachments/assets/93b569d5-bee3-4343-969d-6d9af9c745ea" />


---

## 🌍 Future Work

- Deploy as an interactive web app
- Incorporate multi-modal imaging (MRI + PET)


---

## 🛠️ Tools & Tech Used

- Python
- PyTorch
- OpenCV
- NumPy & Pandas
- Matplotlib & Seaborn
- DICOM & NiBabel for medical imaging
- Jupyter Notebook

---

## 📎 Author & Contact

Shadman Rahman Sameen  
Undergraduate Student, Dept. of CSE  
BRAC University, Dhaka, Bangladesh  
📧 shadman.rahman.sameen@g.bracu.ac.bd  
🔗 GitHub: https://github.com/ShadmanRahman786

---

<p align="center"><i>“Turning pixels into predictions, one scan at a time.”</i></p>
