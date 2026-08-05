---
layout: page
title: Research
permalink: /research/
nav: true
nav_order: 2
---

<div style="text-align: justify;">

<p>My research focuses on developing machine learning systems that remain reliable, interpretable, and useful beyond controlled benchmark settings. I am particularly interested in how models behave under domain shift, demographic imbalance, limited supervision, missing sensor modalities, and other constraints that arise during real-world deployment.</p>

<p>My work lies at the intersection of <strong>machine learning</strong>, <strong>computer vision</strong>, <strong>medical image analysis</strong>, <strong>multimodal learning</strong>, <strong>explainable AI</strong>, and <strong>trustworthy AI</strong>, with additional applications in cybersecurity and intelligent sensing.</p>

<p>A unifying question across my research is:</p>

<blockquote><em>How can we develop models that not only perform well, but also generalize reliably and support defensible decisions when the deployment environment differs from the training environment?</em></blockquote>

<p>This question influences how I design models, construct evaluation protocols, analyze failure modes, and interpret model behavior.</p>

<p>A full list of publications with citations, abstracts, and BibTeX entries is available on the <a href="/publications/">publications page</a>.</p>

<hr>

<h2>Medical Image Analysis</h2>

<h3>ED-Net: Generalizable Colorectal Polyp Segmentation</h3>

<p>My undergraduate thesis focused on colorectal polyp segmentation, an important component of computer-assisted colonoscopy. I developed <strong>ED-Net</strong>, a hybrid deep learning framework that combines a pretrained EfficientNetB0 encoder with a Double U-Net architecture.</p>

<p>The framework incorporates Atrous Spatial Pyramid Pooling for multiscale feature extraction, Squeeze-and-Excitation attention for adaptive channel recalibration, and test-time augmentation to improve prediction consistency during inference. I also used Grad-CAM and SE attention maps to examine which image regions and feature channels influenced the model's predictions.</p>

<p>A central goal of this work was to evaluate whether the model could generalize beyond the dataset used for training. ED-Net was therefore assessed on multiple external polyp segmentation datasets without retraining, along with reverse cross-dataset experiments and ablation studies. A dual-mode clinical deployment strategy was proposed — real-time screening without TTA (47.17 FPS) and offline diagnostic analysis with TTA (12.93 FPS) — to support practical endoscopic workflows.</p>

<p>This work was published in <em>Biomedical Signal Processing and Control</em>, vol. 123, Part A, p. 110566, Elsevier, 2026 (Q1, IF: 4.9). See the <a href="/publications/">publications page</a> for full citation and BibTeX.</p>

<hr>

<h2>Fairness in Medical Image Segmentation</h2>

<h3>MetaSeg: Demographic Fairness in Skin Lesion Segmentation</h3>

<p>My subsequent research examined demographic fairness in skin lesion segmentation on the HAM10000 dataset. The study investigates an apparent segmentation performance gap between younger and older patients.</p>

<p>Rather than assuming the observed difference represented direct model bias, I examined whether it could be explained by differences in lesion-type composition across age groups. The analysis included multiple segmentation architectures, demographic-targeted interventions, regression adjustment, matching, standardization, bootstrap analysis, continuous-age modelling, and other robustness checks.</p>

<p>The results showed that the apparent age-related disparity was largely explained by the higher prevalence of more difficult lesion types among older patients — a case of lesion-type confounding rather than genuine model bias. Five interventions directed specifically at age did not meaningfully remove the gap, while adjustment for lesion type substantially reduced it.</p>

<p>This work has shaped my interest in <strong>confound-aware fairness evaluation</strong>. The manuscript is currently under review at <em>IEEE Open Journal of the Computer Society</em>.</p>

<hr>

<h2>Reliability of Clinical Machine Learning</h2>

<h3>Data Leakage in ML on Medical Tabular Data</h3>

<p>I have also contributed to a systematic review and experimental investigation of <strong>data leakage in clinical machine learning</strong>, conducted with collaborators at RUET.</p>

<p>The study examines how information can unintentionally pass between training and evaluation stages through preprocessing, feature selection, imputation, normalization, resampling, cross-validation, or improper data partitioning. Such leakage can produce overly optimistic results and make unreliable models appear suitable for clinical use.</p>

<p>This research expanded my perspective from model architecture to the reliability of the entire machine learning pipeline — reinforcing that trustworthy clinical AI depends not only on the model, but also on data provenance, experimental design, validation methodology, and transparent reporting. The manuscript is currently under review at <em>Computer Methods and Programs in Biomedicine</em> (Elsevier, IF: 4.8).</p>

<hr>

<h2>Multimodal and Sensor-Based AI</h2>

<h3>Cattle Behavior Recognition at Qatar University</h3>

<p>I currently work as a Research Assistant under Dr. Amith Khandakar at Qatar University on multimodal cattle behavior recognition using wearable and farm-sensing modalities.</p>

<p>A major challenge is that real farms do not always provide the same sensors or complete observations. Sensors may fail, modalities may be unavailable, and models trained on one group of animals may not generalize to unseen animals. My current research therefore investigates how information from multiple sensors can be used during training while retaining the possibility of deployment with a more limited sensor configuration.</p>

<p>This work has expanded my interests toward multimodal representation learning, missing-modality robustness, cross-subject generalization, and deployable sensor-based intelligence.</p>

<hr>

<h2>Explainable AI</h2>

<p>Explainability is an important component of several of my projects.</p>

<p>In ED-Net, I used Grad-CAM and channel attention analysis to examine whether model predictions were associated with relevant polyp regions. In my skin lesion research, interpretability extended beyond visual explanations to include statistical analysis of demographic disparities, clinical confounding, and uncertainty.</p>

<p>I also applied SHAP-based feature attribution in an ensemble phishing detection system combining XGBoost, LightGBM, and CatBoost. The aim was to make security-related predictions more understandable by showing how lexical and structural website features contributed to classification decisions.</p>

<p>These experiences have led me to view explainability as more than the production of visual heatmaps. A useful explanation should help researchers identify failure modes, examine whether a model relies on defensible evidence, and understand how predictions change across populations or deployment conditions.</p>

<hr>

<h2>Machine Learning for Cybersecurity</h2>

<p>My cybersecurity research covers two directions. First, I contributed to an ensemble phishing detection framework based on XGBoost, LightGBM, CatBoost, and TabPFN with soft voting and SHAP-based interpretability, achieving 93.3% accuracy and 0.99 recall. This work was published at ICCIT 2025 (IEEE). See the <a href="/publications/">publications page</a> for full citation and BibTeX.</p>

<p>Second, I am developing a multimodal phishing detection framework using explicit visual-semantic inconsistency scoring with frozen vision-language encoders, combined with a lightweight classifier and evaluated on a four-dataset progressive evaluation structure.</p>

<p>Cybersecurity presents a distinct form of distribution shift from medical imaging — the input distribution may change deliberately as attackers adapt their strategies. This makes robustness, transparent decision-making, and continuous evaluation particularly important.</p>

<hr>

<h2>Natural Language Processing for Low-Resource Languages</h2>

<h3>PAEG: Pragmatic-Aware Emotion Grounding for Bangla</h3>

<p>I am also investigating pragmatic feature loss in machine-translated Bangla emotion datasets. Translation tools tend to preserve semantic content but lose pragmatic markers — culturally grounded expressions, honorifics, and discourse particles — that carry significant emotional signal in Bangla.</p>

<p>The <strong>Pragmatic-Aware Emotion Grounding (PAEG)</strong> framework combines lexicon retrieval with culturally grounded augmentation to recover these features and improve LLM-based emotion recognition for low-resource Bangla. This work is built on three self-constructed datasets.</p>

<hr>

<h2>Research Vision</h2>

<p>My long-term goal is to develop trustworthy and deployable AI methods for healthcare and intelligent sensing, particularly in environments where data, computational resources, sensor availability, and specialist expertise are limited.</p>

<p>I am especially interested in research involving:</p>

<ul>
<li>robustness under domain and population shift;</li>
<li>multimodal learning with missing or incomplete modalities;</li>
<li>uncertainty-aware prediction and selective decision-making;</li>
<li>confound-aware fairness evaluation;</li>
<li>interpretable model design;</li>
<li>reliable validation of clinical and sensor-based AI systems.</li>
</ul>

<p>I aim to pursue research that combines methodological rigor with practical deployment considerations. In the long term, I hope to contribute to the development of stronger AI research capacity in Bangladesh and support the creation of technologies designed for resource-constrained healthcare and sensing environments.</p>

<hr>

<p>A full list of publications with citations, abstracts, and BibTeX entries is available on the <a href="/publications/">publications page</a>.</p>

<p><strong>Research Interests:</strong> Machine Learning · Computer Vision · Multimodal Learning · Explainable AI · Trustworthy AI · Medical Image Analysis · Cybersecurity · Signal Processing · NLP for Low-Resource Languages</p>

</div>
