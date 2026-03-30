# Dual-View CNN for Skin Lesion Classification

## Overview

A lightweight **dual-branch CNN** for dermatological image classification that combines **lesion features + surrounding skin context** to improve performance without using pre-trained models or segmentation.

---

## Key Idea

* Traditional CNNs use only the lesion
* This model uses:

  * **Lesion view (224×224)**
  * **Context view (128×128)**
* Mimics how clinicians assess both lesion and surrounding skin

---

## Results

* **Accuracy:** 76.5%
* **Macro F1-score:** 76%
* **AUROC:** ~0.95

**Highlights:**

* High sensitivity for melanoma (**87.8% recall**)
* More balanced performance across classes than baseline CNN
* Interpretable via Grad-CAM

---

## Tech Stack

* Python
* TensorFlow / Keras
* Google Colab

---

## Dataset

* HAM10000 (public)
* Fitzpatrick17k (restricted)

⚠️ Fitzpatrick17k is **not included** due to licensing restrictions.
You must request access separately to reproduce full results.

---

## Ethical Considerations

* No restricted data redistributed
* Acknowledges dataset bias (especially skin tone representation)
* Model is **not for clinical use**

---

## Why It Matters

* No reliance on pre-trained models
* Lower computational cost than transfer learning models
* Better balance between **performance, interpretability, and efficiency**

---


