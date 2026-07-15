# S³-Net: Spatial-Spectral-Statistical Learning for Fine-Grained UAV Maritime Rescue Detection


<p align="center">

<b>
A Lightweight and Scale-Adaptive Detector for Fine-Grained UAV Maritime Rescue Detection
</b>

<br><br>

<a href="">
<img src="https://img.shields.io/badge/Paper-Coming%20Soon-red">
</a>

<a href="">
<img src="https://img.shields.io/badge/Code-Coming%20Soon-blue">
</a>

</p>


<p align="center">
<img src="assets/teaser.png" width="95%">
</p>


---

# 📌 Overview

UAV-based maritime rescue detection is challenging due to:

- extremely small object scales,
- complex maritime backgrounds,
- significant appearance variations,
- limited discriminative features.

To address these challenges, we propose **S³-Net**, a spatial-spectral-statistical learning framework for fine-grained UAV maritime rescue detection.


S³-Net introduces three key components:


### 🔹 SAM-S2D
**Spatial Attention Modulated Space-to-Depth**

Enhances spatial representation while preserving detailed information of small-scale targets.


### 🔹 DS-C3k2-FSAS
**Depthwise Separable Frequency-Enhanced Bottleneck with Frequency-Spectral Adaptive Selection**

Explores frequency-domain characteristics to improve feature discrimination under complex backgrounds.


### 🔹 SAGA
**Statistically-Adaptive Gated Attention**

Introduces statistical feature descriptors for adaptive feature refinement.


Together, these components enable S³-Net to achieve improved detection accuracy with a compact model size.


---

# 🏗️ Framework


<p align="center">
<img src="assets/framework.png" width="100%">
</p>


The proposed framework adopts a scale-adaptive architecture with enhanced high-resolution feature representation for small maritime targets.


---

# 📊 Performance


## SeaDronesSee v2


S³-Net is evaluated on the SeaDronesSee v2 validation set.


Compared with the baseline YOLOv13-S, S³-Net achieves:

- **+8.3 AP improvement**
- **+10.3 AR$_{10}$ improvement**
- reducing parameters from **9.0M to 2.5M**


| Method | AP | AP$_{50}$ | AP$_{75}$ | AR$_1$ | AR$_{10}$ | Params |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| YOLOv13-S | 36.5 | 63.2 | 36.4 | 28.6 | 42.8 | 9.0M |
| **S³-Net (Ours)** | **44.8** | **77.2** | **44.6** | **33.6** | **53.1** | **2.5M** |


---

## Cross-Dataset Generalization


The generalization capability of S³-Net is further evaluated on TinyPerson and AFO datasets.


| Dataset | Method | AP | AP$_{50}$ | AP$_{75}$ | AR$_1$ | AR$_{10}$ |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| TinyPerson | YOLOv13-S | 5.8 | 16.1 | 3.3 | 2.0 | 6.2 |
| | **S³-Net** | **8.4** | **24.3** | **4.5** | **2.2** | **8.1** |
| AFO | YOLOv13-S | 25.0 | 53.0 | 17.6 | 17.0 | 33.3 |
| | **S³-Net** | **26.6** | **55.0** | **21.5** | **18.0** | **34.8** |


---

# 🔍 Visualization


<p align="center">
<img src="assets/visualization.png" width="95%">
</p>


Visualization results demonstrate that S³-Net produces more accurate detections and focuses more effectively on small targets under complex maritime backgrounds.


---

# 📂 Repository Status


The current repository provides:

- project overview,
- framework visualization,
- qualitative results.


The complete implementation, including:

- source code,
- training scripts,
- inference tools,
- configuration files,
- pretrained models,

will be publicly released after the paper acceptance.


---

# 📝 Citation


If you find this work useful, please consider citing:


```bibtex
@article{S3Net2026,
  title={S$^3$-Net: Spatial-Spectral-Statistical Learning for Fine-Grained UAV Maritime Rescue Detection},
  author={Coming Soon},
  journal={Coming Soon},
  year={2026}
}
```
