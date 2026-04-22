# Optimization, Not Architecture: ViT Generalization in Small-Data Regimes

This repository contains a controlled empirical study investigating why Vision Transformers (ViTs) underperform in small-data settings (CIFAR-10) and what factors truly govern their generalization.

---

## 🔍 Key Insight

Contrary to common assumptions, **architectural scaling and data augmentation alone provide limited gains**.  

Instead, **optimization strategies — specifically learning rate warmup combined with cosine decay — produce substantial improvements in generalization performance.**

---

## 📊 Results

- Baseline ViT: ~45–55% accuracy  
- + Augmentation & capacity: ~56–57%  
- + Optimized training: **~71% accuracy**

This demonstrates that **optimization dynamics dominate architectural choices in small-data regimes.**

---

## 🧪 Experiments

The repository includes:

- VGG16 baseline (CNN comparison)
- ViT baseline (no augmentation, no scheduling)
- ViT + Data Augmentation
- ViT + Increased Capacity & Regularization
- ViT + Optimized Training (Warmup + Cosine Decay)

---

## 📁 Repository Structure

- Notebook/ → All experiment notebooks
- Figures/ → Accuracy plots and results
- Paper/ → Research paper (PDF)


---

## 📄 Paper

[Read the paper](Paper/vit-small-data-optimization.pdf)
[OpenReview Version](https://openreview.net/forum?id=BnKObGDEr6)

---

## 🔗 Future Work

Ongoing work explores:
- Robustness under distribution shifts  
- Behavior under distorted or real-world imaging conditions  
- Extending optimization insights to detection and video tasks  

---

## ⚙️ Notes

All models are trained from scratch on CIFAR-10 under controlled experimental settings to isolate the effects of:
- Data diversity  
- Model capacity  
- Regularization  
- Optimization strategies
  
