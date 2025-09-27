# Explainable AI with Grad-CAM (Deep Learning Lab 2025)

This project was part of the **Deep Learning Lab Challenge 2025** at TU Braunschweig.  
The task: train an **image classifier** and provide **explainable predictions** using saliency maps.

---

##📂 Repository Contents
Due to cluster restrictions, the full training code cannot be shared here.
Instead, this repository contains:

✅ Final presentation slides

✅ Evaluation results (Classification & Explainability metrics)

✅ A Grad-CAM demo notebook using pretrained ResNet

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

<p align="center">
  <img src="results/sample1_class14_saliency.png" alt="Grad-CAM Example" width="400"/>
</p>  

*Example: Grad-CAM saliency map for Class 14.*  

Bright **yellow regions** show where the model focused most strongly when making its prediction,  
while **darker areas** indicate less influence.  
This visualization clearly illustrates **which parts of the image drive the decision**.  


---

## 📂 Repository Structure
- `slides/` → Final presentation slides  
- `notebooks/` → Small Grad-CAM demo (PyTorch)  
- `results/` → Sample saliency maps and metrics  

---

## 🛠 Requirements
```bash
pip install -r requirements.txt
