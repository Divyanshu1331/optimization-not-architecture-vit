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
