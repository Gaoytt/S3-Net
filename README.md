# S³-Net: Spatial-Spectral-Statistical Learning for Fine-Grained UAV Maritime Rescue Detection


<p align="center">

<b>
A Spatial-Spectral-Statistical Learning Framework for Fine-Grained UAV Maritime Rescue Detection
</b>

<br><br>

<a href="">
<img src="https://img.shields.io/badge/Paper-Coming%20Soon-red">
</a>

<a href="">
<img src="https://img.shields.io/badge/Code-Coming%20Soon-blue">
</a>

</p>


---

# 📌 Overview


UAV-based maritime rescue detection remains challenging due to:

- extremely small object scales,
- complex maritime backgrounds,
- significant appearance variations,
- limited discriminative features.


To address these challenges, we propose **S³-Net**, a spatial-spectral-statistical learning framework for fine-grained UAV maritime rescue detection.


S³-Net introduces three key components:


### 🔹 SAM-S2D  
**Spatial Attention Modulated Space-to-Depth**

SAM-S2D enhances spatial representation while preserving detailed information of small-scale targets through spatial attention modulation.


### 🔹 DS-C3k2-FSAS  
**Depthwise Separable Frequency-Enhanced Bottleneck with Frequency-Spectral Adaptive Selection**

DS-C3k2-FSAS explores frequency-domain characteristics to improve feature discrimination under complex backgrounds.


### 🔹 SAGA  
**Statistically-Adaptive Gated Attention**

SAGA introduces statistical feature descriptors for adaptive feature refinement and improves target representation.


Together, these components enable S³-Net to achieve accurate detection of small maritime targets with a compact model size.


---

# 🏗️ Framework


<p align="center">

[View framework.pdf](assets/framework.pdf)

</p>


The overall architecture of S³-Net integrates spatial, spectral, and statistical feature learning components to improve the representation capability for fine-grained UAV maritime rescue detection.


---

# 📊 Performance


## SeaDronesSee v2


S³-Net is evaluated on the SeaDronesSee v2 validation set.


Compared with the baseline YOLOv13-S, S³-Net achieves:

- **+8.3 AP improvement**
- **+10.3 AR<sub>10</sub> improvement**
- reducing parameters from **9.0M to 2.5M**


| Method | AP | AP<sub>50</sub> | AP<sub>75</sub> | AR<sub>1</sub> | AR<sub>10</sub> | Params |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| YOLOv13-S | 36.5 | 63.2 | 36.4 | 28.6 | 42.8 | 9.0M |
| **S³-Net (Ours)** | **44.8** | **77.2** | **44.6** | **33.6** | **53.1** | **2.5M** |


---

## Cross-Dataset Generalization


The generalization capability of S³-Net is further evaluated on TinyPerson and AFO datasets.


| Dataset | Method | AP | AP<sub>50</sub> | AP<sub>75</sub> | AR<sub>1</sub> | AR<sub>10</sub> |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| TinyPerson | YOLOv13-S | 5.8 | 16.1 | 3.3 | 2.0 | 6.2 |
| | **S³-Net (Ours)** | **8.4** | **24.3** | **4.5** | **2.2** | **8.1** |
| AFO | YOLOv13-S | 25.0 | 53.0 | 17.6 | 17.0 | 33.3 |
| | **S³-Net (Ours)** | **26.6** | **55.0** | **21.5** | **18.0** | **34.8** |


---

# 📈 Comparison with Existing Methods


<p align="center">

[View comparison.pdf](assets/comparison.pdf)

</p>


Comparison results demonstrate that S³-Net achieves superior detection performance compared with representative object detectors.

S³-Net obtains an AP of **44.8%** on the SeaDronesSee v2 validation set while maintaining a compact model size of **2.5M parameters**.


---

# 🔍 Detection Visualization


<p align="center">

[View detection_visualization.pdf](assets/detection_visualization.pdf)

</p>


Qualitative detection results demonstrate that S³-Net maintains robust performance under challenging UAV maritime scenarios, including small objects, dense distributions, and complex backgrounds.


---

# 🔥 Feature Activation Visualization


<p align="center">

[View heatmap_visualization.pdf](assets/heatmap_visualization.pdf)

</p>


Feature activation visualization demonstrates that S³-Net produces more focused responses on target regions while suppressing irrelevant background information.


---

# 📂 Repository Status


The current repository provides:

- project overview,
- model architecture,
- quantitative results,
- visualization examples.


The complete implementation, including:

- source code,
- training scripts,
- inference tools,
- configuration files,
- pretrained models,

will be publicly released after the paper acceptance.
