---
layout: default
title: "The Power of Certainty: How Confident Models Lead to Better Segmentation"
permalink: /projects/power-of-certainty/
description: "Dynamic Confidence-Based Self-Distillation (DCSD) for polyp segmentation in medical images. Outperforms state-of-the-art models using confidence-weighted self-distillation."
---

# The Power of Certainty: How Confident Models Lead to Better Segmentation

**Authors:** Tugberk Erol, Tuba Caglikantar, Duygu Sarikaya  
**Affiliations:**  
- Gazi University, Department of Computer Engineering, Turkey  
- Ankara Yildirim Beyazit University, Department of Software Engineering, Turkey  
- University of Leeds, School of Computer Science, United Kingdom  

**Abstract:**  
Deep learning models have shown strong performance in automatic polyp detection and segmentation during colonoscopy. However, large models are prone to overfitting and poor generalization across diverse datasets. Knowledge distillation and self-distillation address these limitations, but often require high memory and computational cost. We propose **Dynamic Confidence-Based Self-Distillation (DCSD)**, a novel approach that leverages only previous iteration data during training without extra computation at test time. By weighting the distillation loss with a dynamic confidence coefficient, DCSD improves model reliability, consistency, and generalization across multiple datasets.

---

## Highlights

- Introduces a confidence-weighted self-distillation method for segmentation.
- Reduces hypothesis space by focusing on confident predictions from previous iterations.
- Compatible with efficient architectures such as Pyramid Vision Transformer (PVT) backbone.
- Outperforms baseline and previous self-distillation methods on multiple datasets, including Kvasir-SEG, CVC-ClinicDB, EndoScene, ETIS, and BKAI-IGH.
- Applicable to real-time polyp segmentation without increasing inference cost.

---

## Methodology

### Architecture
- Encoder-decoder structure using three layers from PVT as the backbone.
- Receptive Field Block (RFB) captures multi-scale spatial features.
- Layer aggregation replaces skip connections for better information fusion.

### Dynamic Confidence-Based Self-Distillation (DCSD)
- Stores only the previous mini-batch predictions during training.
- Uses Dice coefficient as a confidence score to weight MSE loss between iterations.
- Encourages model to reinforce only confident past knowledge.


## Conclusion

DCSD is a simple yet effective confidence-weighted self-distillation approach that improves segmentation performance and generalization without extra inference cost. Future work aims to explore adaptive temperature scaling and confidence estimation for better robustness in clinical settings.

**Contact:** tugberk.erol@gazi.edu.tr  
**arXiv:** [arXiv:2507.10490v1](https://arxiv.org/abs/2507.10490)  
