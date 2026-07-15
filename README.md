# S3-Net
# S³-Net: Spatial-Spectral-Statistical Learning for Fine-Grained UAV Maritime Rescue Detection


<p align="center">

<b>
A Lightweight and Scale-Adaptive Detector for Small-Scale Maritime Rescue Targets in UAV Imagery
</b>

<br><br>

<a href="">
<img src="https://img.shields.io/badge/Paper-Coming%20Soon-red">
</a>

<a href="">
<img src="https://img.shields.io/badge/Code-Coming%20Soon-blue">
</a>

<a href="">
<img src="https://img.shields.io/badge/License-MIT-green">
</a>

</p>


<p align="center">
<img src="assets/teaser.png" width="95%">
</p>


---

## 📌 Overview

Unmanned Aerial Vehicle (UAV)-based maritime rescue detection faces significant challenges, including:

- extremely small object scales,
- complex background interference,
- severe appearance variations,
- limited computational resources for edge deployment.


To address these challenges, we propose **S³-Net**, a spatial-spectral-statistical learning framework designed for fine-grained UAV maritime rescue detection.


S³-Net introduces three key components:

- **SAM-S2D**  
  *Spatial Attention Modulated Space-to-Depth module*  
  Enhances spatial representation while preserving fine-grained target information.

- **DS-C3k2-FSAS**  
  *Depthwise Separable Frequency-Enhanced Bottleneck with Frequency-Spectral Adaptive Selection*  
  Explores frequency-domain characteristics to improve feature discrimination for small targets.

- **SAGA**  
  *Statistically-Adaptive Gated Attention module*  
  Utilizes statistical feature descriptors for adaptive feature recalibration.


Together, these components provide improved detection accuracy and deployment efficiency for UAV maritime rescue scenarios.


---

# 🔥 Highlights

✨ **Scale-Adaptive Architecture**

A redesigned multi-scale detection architecture focusing on high-resolution features for tiny maritime objects.


✨ **Spatial-Spectral Feature Enhancement**

Combines spatial attention and frequency-domain modeling to capture complementary target characteristics.


✨ **Statistical Adaptive Attention**

Introduces statistical descriptors to improve feature selection under complex backgrounds.


✨ **Edge Deployment Friendly**

Designed with lightweight components and validated on edge computing platforms.


---

# 🏗️ Network Architecture


<p align="center">
<img src="assets/framework.png" width="100%">
</p>


The overall framework consists of:

- backbone feature extraction,
- spatial-spectral enhancement,
- statistical adaptive attention,
- scale-adaptive detection heads.


---

# 📊 Qualitative Results


<p align="center">
<img src="assets/qualitative_results.png" width="95%">
</p>


S³-Net demonstrates robust detection performance under challenging UAV maritime environments, including:

- tiny targets,
- dense object distributions,
- complex ocean backgrounds.


---

# 🔍 Visualization Analysis


<p align="center">
<img src="assets/gradcam.png" width="95%">
</p>


Visualization results show that S³-Net focuses more effectively on target regions while suppressing irrelevant background responses.


---

# 📈 Performance


Detailed quantitative comparisons, ablation studies, and deployment benchmarks are provided in the paper.


| Model | Dataset | mAP | FPS |
|:---:|:---:|:---:|:---:|
| YOLO baseline | SeaDronesSee | - | - |
| S³-Net | SeaDronesSee | - | - |


*(Complete results will be updated after publication.)*


---

# 🚀 Code Availability


The source code is currently being organized.


The complete implementation, including:

- training scripts,
- inference code,
- model configuration,
- pretrained weights,
- evaluation tools,
- deployment files,

will be publicly released after the paper acceptance.


Stay tuned!


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


---

# 📅 Roadmap


- [x] Repository initialization
- [x] Framework visualization
- [x] Qualitative examples

Future:

- [ ] Source code release
- [ ] Pretrained models
- [ ] Training pipeline
- [ ] Inference toolkit
- [ ] ONNX/TensorRT deployment


---

# 📄 License


This project will be released under the MIT License after publication.


---

# 📬 Contact


For questions regarding this project, please contact:

```
Coming Soon
```
