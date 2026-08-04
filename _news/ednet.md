---
layout: post
title: ED-Net Published in Biomedical Signal Processing and Control
date: 2026-05-04 00:00:00
inline: false
related_posts: false
---

Our paper **ED-Net: A Hybrid Deep Learning Framework for Precise Polyp Segmentation Integrating EfficientNetB0 with Double U-Net Architecture and Atrous Spatial Pyramid Pooling with Test-Time Augmentation** has been published in *Biomedical Signal Processing and Control*, Elsevier (Q1, IF: 4.9).

#### About the Paper

Colorectal cancer (CRC) is a major global health concern, and colorectal polyps are early indicators of CRC. ED-Net is a hybrid deep learning framework designed to address three core limitations in existing polyp segmentation models: failure to jointly optimize Dice and IoU, limited cross-dataset generalization, and poor balance between segmentation accuracy and computational efficiency for real-time clinical deployment.

#### Key Contributions

- Hybrid dual-encoder-decoder combining EfficientNetB0 and Double U-Net with ASPP and SE-block channel attention
- Test-Time Augmentation (TTA) applied at inference to improve boundary delineation without modifying the network architecture
- Dual-mode clinical deployment strategy — real-time screening without TTA (47.17 FPS) and offline diagnostic analysis with TTA (12.93 FPS)
- Cross-dataset validation on three external benchmarks demonstrating clinical robustness under domain shift
- Grad-CAM and SE block attention analysis confirming clinically interpretable decision-making

#### Results

| Dataset | Accuracy | Dice | IoU |
|---|---|---|---|
| Kvasir-SEG (with TTA) | 97.13% | 92.26% | 91.08% |
| CVC-ClinicDB | 96.39% | 80.62% | 79.79% |
| ETIS-LaribPolypDB | 97.57% | 77.15% | 80.14% |
| PolypGen2021 | 95.66% | 80.71% | 74.32% |

#### Citation

R. K. Kundu, H. B. Kibria, Md. F. Ahamed, and M. E. H. Chowdhury, "ED-Net: A Hybrid Deep Learning Framework for Precise Polyp Segmentation Integrating EfficientNetB0 with Double U-Net Architecture and Atrous Spatial Pyramid Pooling with Test-Time Augmentation," *Biomedical Signal Processing and Control*, vol. 123, Part A, p. 110566, Elsevier, 2026.

DOI: [10.1016/j.bspc.2026.110566](https://doi.org/10.1016/j.bspc.2026.110566)
