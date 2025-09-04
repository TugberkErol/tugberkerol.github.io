---
layout: null
title: "The Power of Certainty"
permalink: /projects/power-of-certainty/
description: "Confidence-based self-distillation approach for improved polyp segmentation."
---

# The Power of Certainty

**Abstract:**  
This project introduces a confidence-based self-distillation approach for polyp segmentation. The method stores predictions from previous training iterations and uses them to guide the network toward more consistent and reliable predictions. Unlike many distillation methods, this approach does not require extra computation or memory during inference, making it efficient for deployment. By leveraging only previously stored outputs, the model achieves better segmentation performance compared to state-of-the-art methods while maintaining computational efficiency.

---

## Key Features
- Confidence-guided self-distillation  
- No extra computation or memory required at test time  
- Improves segmentation consistency and reliability  
- Compatible with standard CNN and Transformer architectures

---


## Code & Repository
- GitHub: [TugberkErol/DCSD](https://github.com/TugberkErol/DCSD)

---

## Publication
- arXiv: [2507.10490](https://arxiv.org/abs/2507.10490)


