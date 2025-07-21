# 🧠 NMF Robustness Evaluation on Face Datasets
## 🧾 Project Description

This group project implements and compares the robustness of two Non-negative Matrix Factorization (NMF) algorithms on face image datasets (ORL and Extended YaleB). The focus is on performance under Gaussian noise corruption.  

Implemented Algorithms  
L2-Norm Multiplicative Update Rule (MUR) NMF  

L2,1-Norm Robust NMF  

We evaluate both on:  

Reconstruction ability  

Clustering accuracy  

Robustness under noise  

### ✅ Implemented Algorithms

- **L2,1-Norm Robust NMF**  
  Adds L2,1-norm regularization to improve robustness against outliers and noise.

- **L2-Norm MUR NMF**  
  Traditional multiplicative update rule with Frobenius norm minimization.

### 🧠 Goals

- Analyze NMF robustness under Gaussian noise
- Evaluate effectiveness via clustering metrics
- Visualize noisy vs. reconstructed face images

---

## 📊 Dataset Overview

| Dataset         | Samples | Subjects | Description                             |
|----------------|---------|----------|-----------------------------------------|
| ORL            | 400     | 40       | 10 images per subject, small-scale      |
| Extended YaleB | 2414    | 38       | Various poses & lighting, large-scale   |

> ⚠️ **Note**: Datasets are **not included**. Please download from official links and place into `code/data/` manually.

---

## 🧪 Experiments

- Images are **corrupted with Gaussian noise** (mean = 0, std = 0.2)
- Metrics:  
  - ✅ Accuracy (ACC)  
  - ✅ Normalized Mutual Information (NMI)

### 📈 Results

| Dataset        | Algorithm       | ACC    | NMI    |
|----------------|-----------------|--------|--------|
| ORL            | L2-Norm MUR     | 0.6200 | 0.7900 |
| ORL            | L2,1-Norm       | 0.2475 | 0.4182 |
| Extended YaleB | L2-Norm MUR     | 0.1396 | 0.1796 |
| Extended YaleB | L2,1-Norm       | 0.0861 | 0.0746 |

> 📌 See `results.md` and report for full visual comparisons.

---

## 🚀 How to Run

### 1. Clone and Enter Project

```bash
git clone https://github.com/YOUR_USERNAME/NMF-Robustness.git
cd NMF-Robustness/code  
```

---

## ⚠️ Academic Integrity Notice

This repository contains code written for educational purposes.  

Please **do not copy** or reuse this work for academic submission in any course, as this may violate university academic honesty policies.  
You are welcome to use it as reference for personal learning, but not for plagiarism.


