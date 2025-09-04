---
layout: default
title: "PlutoNet: Efficient Polyp Segmentation"
permalink: /projects/plutonet/
description: "PlutoNet: An efficient polyp segmentation network with modified partial decoder and decoder consistency training."
---

# PlutoNet: An Efficient Polyp Segmentation Network

**Abstract:**  
PlutoNet is a lightweight polyp segmentation network designed to accurately detect and segment polyps while minimizing the number of parameters. It introduces a **decoder consistency training** strategy with a **modified partial decoder** and an **auxiliary decoder**, balancing low-level salient details and higher-level semantic features. This approach improves encoder representations, reduces uncertainty, and lowers false positive rates. PlutoNet requires only **2.6M parameters**, less than 10% of comparable models, while achieving state-of-the-art performance on multiple public datasets.

## Key Highlights
- Lightweight encoder-decoder structure using EfficientNet-B0 as backbone  
- Modified Partial Decoder: combines partial decoder and full-scale connections, skipping redundant low-level connections  
- Auxiliary Decoder: focuses on higher-level semantic features during training  
- Decoder Consistency Training: combines losses from both decoders to enforce consistent predictions  
- Asymmetric Convolutions & Squeeze-and-Excitation blocks to handle variation in polyp size, shape, and appearance  
- Extensive evaluation on Kvasir-SEG, ClinicDB, ETIS, EndoScene, and CVC-ColonDB datasets  
- Outperforms state-of-the-art models with fewer parameters, especially on unseen datasets  
- Ablation studies demonstrate effectiveness of consistency training  
 

## Contributions
1. Novel **decoder consistency training** between two specialized decoders to improve segmentation representations.  
2. PlutoNet architecture achieves high accuracy with far fewer parameters than existing models.  
3. Comprehensive evaluation shows superior generalization to unseen datasets.  
4. Ablation studies confirm the effectiveness of the proposed consistency training.

## Code & Repo
- GitHub: [TugberkErol/PlutoNet](https://github.com/TugberkErol/PlutoNet)  

## Publication
- arXiv: [2204.03652v4](https://arxiv.org/abs/2204.03652)
- Paper: (https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/htl2.12105) 
