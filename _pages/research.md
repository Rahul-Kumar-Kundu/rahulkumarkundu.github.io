---
layout: page
title: Research
permalink: /research/
nav: true
nav_order: 2
---


<div style="text-align: justify;">
My research focuses on developing machine learning systems that remain reliable, interpretable, and useful beyond controlled benchmark settings. I am particularly interested in how models behave under domain shift, demographic imbalance, limited supervision, missing sensor modalities, and other constraints that arise during real-world deployment.

My work lies at the intersection of **machine learning**, **computer vision**, **medical image analysis**, **multimodal learning**, **explainable AI**, and **trustworthy AI**, with additional applications in cybersecurity and intelligent sensing.

A unifying question across my research is:

> How can we develop models that not only perform well, but also generalize reliably and support defensible decisions when the deployment environment differs from the training environment?

This question influences how I design models, construct evaluation protocols, analyze failure modes, and interpret model behavior.

A full list of publications with citations, abstracts, and BibTeX entries is available on the [publications page](/publications/).

---

## Medical Image Analysis

### ED-Net: Generalizable Colorectal Polyp Segmentation

My undergraduate thesis focused on colorectal polyp segmentation, an important component of computer-assisted colonoscopy. I developed **ED-Net**, a hybrid deep learning framework that combines a pretrained EfficientNetB0 encoder with a Double U-Net architecture.

The framework incorporates Atrous Spatial Pyramid Pooling for multiscale feature extraction, Squeeze-and-Excitation attention for adaptive channel recalibration, and test-time augmentation to improve prediction consistency during inference. I also used Grad-CAM and SE attention maps to examine which image regions and feature channels influenced the model's predictions.

A central goal of this work was to evaluate whether the model could generalize beyond the dataset used for training. ED-Net was therefore assessed on multiple external polyp segmentation datasets without retraining, along with reverse cross-dataset experiments and ablation studies. A dual-mode clinical deployment strategy was proposed — real-time screening without TTA (47.17 FPS) and offline diagnostic analysis with TTA (12.93 FPS) — to support practical endoscopic workflows.

This work was published in *Biomedical Signal Processing and Control*, vol. 123, Part A, p. 110566, Elsevier, 2026 (Q1, IF: 4.9). See the [publications page](/publications/) for full citation and BibTeX.

---

## Fairness in Medical Image Segmentation

### MetaSeg: Demographic Fairness in Skin Lesion Segmentation

My subsequent research examined demographic fairness in skin lesion segmentation on the HAM10000 dataset. The study investigates an apparent segmentation performance gap between younger and older patients.

Rather than assuming the observed difference represented direct model bias, I examined whether it could be explained by differences in lesion-type composition across age groups. The analysis included multiple segmentation architectures, demographic-targeted interventions, regression adjustment, matching, standardization, bootstrap analysis, continuous-age modelling, and other robustness checks.

The results showed that the apparent age-related disparity was largely explained by the higher prevalence of more difficult lesion types among older patients — a case of lesion-type confounding rather than genuine model bias. Five interventions directed specifically at age did not meaningfully remove the gap, while adjustment for lesion type substantially reduced it.

This work has shaped my interest in **confound-aware fairness evaluation**. The manuscript has been submitted to a Q1 journal.

---

## Reliability of Clinical Machine Learning

### Data Leakage in ML on Medical Tabular Data

I have also contributed to a systematic review and experimental investigation of **data leakage in clinical machine learning**, conducted with Hafsa Binte Kibria at RUET.

The study examines how information can unintentionally pass between training and evaluation stages through preprocessing, feature selection, imputation, normalization, resampling, cross-validation, or improper data partitioning. Such leakage can produce overly optimistic results and make unreliable models appear suitable for clinical use.

This research expanded my perspective from model architecture to the reliability of the entire machine learning pipeline — reinforcing that trustworthy clinical AI depends not only on the model, but also on data provenance, experimental design, validation methodology, and transparent reporting. The manuscript is targeting *Computer Methods and Programs in Biomedicine* (Elsevier, IF: 4.8).

---

## Multimodal and Sensor-Based AI

### Cattle Behavior Recognition at Qatar University

I currently work as a Research Assistant under Dr. Amith Khandakar at Qatar University on multimodal cattle behavior recognition using wearable and farm-sensing modalities.

A major challenge is that real farms do not always provide the same sensors or complete observations. Sensors may fail, modalities may be unavailable, and models trained on one group of animals may not generalize to unseen animals. My current research therefore investigates how information from multiple sensors can be used during training while retaining the possibility of deployment with a more limited sensor configuration.

This work has expanded my interests toward multimodal representation learning, missing-modality robustness, cross-subject generalization, and deployable sensor-based intelligence.

---

## Explainable AI

Explainability is an important component of several of my projects.

In ED-Net, I used Grad-CAM and channel attention analysis to examine whether model predictions were associated with relevant polyp regions. In my skin lesion research, interpretability extended beyond visual explanations to include statistical analysis of demographic disparities, clinical confounding, and uncertainty.

I also applied SHAP-based feature attribution in an ensemble phishing detection system combining XGBoost, LightGBM, and CatBoost. The aim was to make security-related predictions more understandable by showing how lexical and structural website features contributed to classification decisions.

These experiences have led me to view explainability as more than the production of visual heatmaps. A useful explanation should help researchers identify failure modes, examine whether a model relies on defensible evidence, and understand how predictions change across populations or deployment conditions.

---

## Machine Learning for Cybersecurity

My cybersecurity research covers two directions. First, I contributed to an ensemble phishing detection framework based on XGBoost, LightGBM, and CatBoost with soft voting and SHAP-based interpretability, achieving 93.71% accuracy and 99% phishing recall. This work was accepted at ICCIT 2025 (IEEE). See the [publications page](/publications/) for full citation and BibTeX.

Second, I am developing a CLIP-based multimodal phishing detection framework using explicit visual-semantic inconsistency scoring with frozen CLIP encoders. The system computes pairwise cosine similarity features between visual and textual brand signals, combined with a lightweight MLP classifier, and is evaluated on a four-dataset progressive evaluation structure.

Cybersecurity presents a distinct form of distribution shift from medical imaging — the input distribution may change deliberately as attackers adapt their strategies. This makes robustness, transparent decision-making, and continuous evaluation particularly important.

---

## Natural Language Processing for Low-Resource Languages

### PAEG: Pragmatic-Aware Emotion Grounding for Bangla

I am also investigating pragmatic feature loss in machine-translated Bangla emotion datasets. Translation tools tend to preserve semantic content but lose pragmatic markers — culturally grounded expressions, honorifics, and discourse particles — that carry significant emotional signal in Bangla.

The **Pragmatic-Aware Emotion Grounding (PAEG)** framework combines lexicon retrieval with culturally grounded augmentation to recover these features and improve LLM-based emotion recognition for low-resource Bangla. This work is built on three self-constructed datasets and targets *Information Processing and Management* (Elsevier Q1).

---

## Research Vision

My long-term goal is to develop trustworthy and deployable AI methods for healthcare and intelligent sensing, particularly in environments where data, computational resources, sensor availability, and specialist expertise are limited.

I am especially interested in research involving:

- robustness under domain and population shift;
- multimodal learning with missing or incomplete modalities;
- uncertainty-aware prediction and selective decision-making;
- confound-aware fairness evaluation;
- interpretable model design;
- reliable validation of clinical and sensor-based AI systems.

I aim to pursue research that combines methodological rigor with practical deployment considerations. In the long term, I hope to contribute to the development of stronger AI research capacity in Bangladesh and support the creation of technologies designed for resource-constrained healthcare and sensing environments.

---

A full list of publications with citations, abstracts, and BibTeX entries is available on the [publications page](/publications/).

**Research Interests:** Machine Learning · Computer Vision · Multimodal Learning · Explainable AI · Trustworthy AI · Medical Image Analysis · Cybersecurity · Signal Processing · NLP for Low-Resource Languages.
</div>
