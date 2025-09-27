# Explainable AI with Grad-CAM (Deep Learning Lab 2025)

This project was part of the **Deep Learning Lab Challenge 2025** at TU Braunschweig.  
The task: train an **image classifier** and provide **explainable predictions** using saliency maps.

---

## 🚀 Project Overview
- Trained **ResNet-50** on Pascal VOC dataset (20 object classes).
- Implemented **Grad-CAM** for class-specific saliency maps.
- Evaluated explanations with:
  - **iAUC** (Faithfulness)
  - **Mean IoU** (Alignment with segmentation masks)
  - **Pointing Game** (Localization accuracy)

---

## 📊 Results
| Metric              | Score  |
|----------------------|--------|
| Test Accuracy        | 97.8%  |
| AUROC                | 98.4%  |
| iAUC (Faithfulness)  | 0.73   |
| Mean IoU (Alignment) | 0.29   |
| Pointing Game        | 0.53   |

---

## 🔍 Example Saliency Maps
Grad-CAM highlights the most important regions used by the model:

![Example](results/sample_saliency.png)

---

## 📂 Repository Structure
- `slides/` → Final presentation slides  
- `notebooks/` → Small Grad-CAM demo (PyTorch)  
- `results/` → Sample saliency maps and metrics  

---

## 🛠 Requirements
```bash
pip install -r requirements.txt
