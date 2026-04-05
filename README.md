# 🌊 Flood Segmentation using NDWI-Guided Probabilistic Fusion

An AI-based approach for accurate flood segmentation from satellite imagery using NDWI as a continuous prior, combined with deep learning and post-processing refinement.

---

## 🚀 Project Overview

Flood mapping from satellite images is critical for disaster response and environmental monitoring. This project introduces a hybrid pipeline that integrates:

- Spectral water index (NDWI)
- Deep learning segmentation model
- Probabilistic fusion strategy
- Intelligent post-processing

Unlike traditional methods, NDWI is used as a **continuous guiding signal**, not a binary mask.

---

## 💡 Key Contributions

✅ **NDWI as Continuous Prior**  
Instead of thresholding NDWI into binary water masks, we use it as a *soft probabilistic guide* to improve model predictions.

✅ **Dual-Threshold Refinement**  
Applies two adaptive thresholds to refine segmentation outputs, improving boundary accuracy and reducing noise.

✅ **Water-Flood Conflict Resolution**  
Handles ambiguous regions where model predictions and NDWI disagree, ensuring more consistent segmentation.

---

## 📊 Best Score

- **Validation IoU:** `0.1752`
- Target: **0.18+ (ongoing improvements)**

---

## 🧠 Methodology

### 🔁 Pipeline

1. Input satellite image
2. Compute NDWI
3. Model prediction (segmentation network)
4. Probabilistic fusion of NDWI + model output
5. Dual-threshold refinement
6. Conflict-aware post-processing
7. Final flood mask

---

## 🗂️ Repository Structure
