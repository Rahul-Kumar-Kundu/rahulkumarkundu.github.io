---
layout: page
title: Multimodal Phishing Detection
description: Multimodal phishing detection using visual-semantic inconsistency scoring for robust brand impersonation detection.
importance: 3
category: Research
---

An ongoing research project developing a multimodal phishing detection framework that exploits explicit visual-semantic inconsistency between a website's visual appearance and its textual brand signals. Unlike URL-only or content-only approaches, this framework leverages joint visual-language understanding to detect brand impersonation — a core mechanism in modern phishing attacks.

**Core Research Challenge:**

Phishing detection faces a fundamentally adversarial distribution shift — attackers deliberately adapt their strategies to evade detection systems. URL-based and heuristic approaches are insufficient against zero-day phishing and adversarial manipulation. A multimodal approach that reasons about visual-semantic consistency offers a more robust signal that is harder for attackers to circumvent.

**Technical Approach:**
- Joint visual and textual feature extraction using frozen vision-language encoders
- Pairwise cosine similarity scoring between visual and textual brand signals
- Brand confidence scoring for known brand identification
- Lightweight classifier on top of similarity features
- Computationally efficient and generalizable design

**Evaluation Strategy:**
- Four-dataset progressive evaluation structure
- Cross-dataset generalization testing
- Adversarial robustness analysis

**Research Focus:**
- Multimodal learning for cybersecurity
- Visual-semantic consistency under adversarial conditions
- Robust and interpretable phishing detection
- Generalization across phishing campaign types

**Status:** In development
