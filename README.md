<h1 align="center">🧠 Neurodegenerative Disease Detection using CNN</h1>

<p align="center">
  <b>🎓 Undergraduate Thesis Project (Completed)</b><br>
  <i>Detection of Alzheimer’s, Parkinson’s & FTD from MRI using Deep Learning</i><br><br>
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/Data-ADNI,PPMI,FTD-orange?style=flat-square">
  <img src="https://img.shields.io/badge/Model-SadNetV1-green?style=flat-square">
</p>

---

## 🚀 Overview

This research focuses on the early diagnosis of **Alzheimer’s**, **Parkinson’s**, and **Frontotemporal Dementia (FTD)** using **2D sagittal MRI slices** with a **pseudo-3D deep learning pipeline**.

Our custom model, **SadNetV1**, builds on **MobileNetV2** and enhances feature learning with **Squeeze-and-Excitation (SE) attention blocks** for high-performance, lightweight disease classification.

> 🧾 Status: Successfully submitted and defended at **BRAC University, Dept. of CSE**  
> 🔐 Code & datasets are private due to ethical and academic regulations

---

## 📚 Datasets Used

- **ADNI** – Alzheimer’s MRI data  
- **PPMI** – Parkinson’s data  
- **FTD** – Neuroimaging data for Frontotemporal Dementia  

**Preprocessing includes:**
- 🎚️ Intensity clipping (0–255)
- 🎨 Conditional CLAHE
- 📏 Resizing (224×224)
- 🧼 Normalization
- 🧾 Saved as `.png` format

### 🧪 Sample MRI Slice
<img width="395" alt="Sample Slice" src="https://github.com/user-attachments/assets/99c39dec-581a-4882-bfbf-8ff2e7b9097a" />

---

## 🔄 Data Preprocessing Pipeline

<img width="438" alt="Preprocessing Flowchart" src="https://github.com/user-attachments/assets/374aa9c8-e204-496d-a6cb-b1b95e3cef39" />

---

## 📈 Data Augmentation Process

- 🔀 Dataset split into Train, Validation, Test sets
- 🔄 Applied rotation, zoom, flips, contrast shifts

### 📊 Split Summary
<img src="https://github.com/user-attachments/assets/d1160f6f-b775-4f2d-9283-992b45e8ef7f" style="width:50%; height:auto;" />

### 🧪 Augmentation Pipeline
<img src="https://github.com/user-attachments/assets/9e7cef07-9eaa-4517-abcc-d84917fe8b81" width="70%"/>

---

## 🔧 Model Workflow Diagram

<img src="https://github.com/user-attachments/assets/31602497-0db4-4f0f-9d06-38f9df7dfa15" width="75%" />

---

## 🧠 Model Architecture – SadNetV1

- 🧩 **Base**: MobileNetV2  
- 🔁 **Attention**: Squeeze-and-Excitation (SE) Blocks  
- 🎯 **Input**: Stacked 2D sagittal MRI (Pseudo-3D)  
- ⚙️ **Optimizer**: Adam (`lr=1e-5`)  
- 📉 **Loss**: Categorical Crossentropy  

```mermaid
graph LR
A[Input MRI Slice] --> B[Preprocessing]
B --> C[MobileNetV2 + SE]
C --> D[Classification Head]
D --> E[Predicted Disease]
```

---

## 📊 Performance Summary

SadNetV1 achieved strong results across all diseases:

- ✅ **Train Accuracy**: 96.84%  
- ✅ **Validation Accuracy**: 97.11%  
- ✅ **Test Accuracy**: 96.15%

---

## 📈 Results & Visualizations

<table>
  <tr>
    <td align="center"><b>📊 Accuracy Graph</b></td>
    <td align="center"><b>📉 Loss Graph</b></td>
  </tr>
  <tr>
    <td><img width="100%" src="https://github.com/user-attachments/assets/3549ab69-192d-40a6-ad66-80da3b83bb07" /></td>
    <td><img width="100%" src="https://github.com/user-attachments/assets/dcf23989-f534-4ef9-9bc7-8474860c57e1" /></td>
  </tr>
</table>

---

## 🧠 Prediction Results

<table>
  <tr>
    <td align="center"><b>Predicted: Alzheimer’s Disease (AD)</b></td>
    <td align="center"><b>Predicted: Parkinson’s Disease (PD)</b></td>
    <td align="center"><b>Predicted: Frontotemporal Dementia (FTD)</b></td>
  </tr>
  <tr>
    <td><img width="100%" src="https://github.com/user-attachments/assets/078dd72b-b226-4ba0-84e9-950e293652ba" /></td>
    <td><img width="100%" src="https://github.com/user-attachments/assets/d62e0406-77ab-4f43-970e-3f9585466056" /></td>
    <td><img width="100%" src="https://github.com/user-attachments/assets/f9b63741-7837-4679-ba9d-434bb281e9d4" /></td>
  </tr>
</table>

---

## 🌍 Future Work

- 🌐 Deploy as an interactive web app
- 🧬 Integrate multi-modal inputs (MRI + PET)
- 🧠 Add attention explainability with SHAP & Grad-CAM++

---

## 🛠️ Tech Stack

- 💻 Python
- 🔬 PyTorch
- 🖼 OpenCV
- 📊 NumPy, Pandas
- 📈 Matplotlib, Seaborn
- 🧠 NiBabel, pydicom
- 🧪 Jupyter Notebook

---

## 📎 Author & Contact

**👨‍💻 Shadman Rahman Sameen**  
🎓 Undergraduate Student, Dept. of CSE  
🏫 BRAC University, Dhaka, Bangladesh  
📧 [shadman.rahman.sameen@g.bracu.ac.bd](mailto:shadman.rahman.sameen@g.bracu.ac.bd)  
🔗 GitHub: [github.com/ShadmanRahman786](https://github.com/ShadmanRahman786)

---

<p align="center"><i>“Turning pixels into predictions, one scan at a time.”</i></p>
