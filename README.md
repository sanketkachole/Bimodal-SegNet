# 🚀 **Bimodal SegNet: Instance Segmentation Fusing Events and RGB Frames for Robotic Grasping**

Bimodal SegNet is a dual-encoder deep learning architecture designed to fuse **event-based signals** and **RGB frame data** for robust instance segmentation in robotic grasping tasks under challenging visual conditions.

Object segmentation in dynamic environments is often degraded by **occlusion**, **low illumination**, **motion blur**, and **scale variation**.
Our architecture addresses these limitations using:

* **Two specialized encoders** (Event + RGB)
* **Spatial Pyramid Pooling with Atrous Convolutions**
* **Multi-scale context fusion**
* **A decoder producing sharp object boundaries**

Evaluations on the **Event-based Segmentation Dataset (ESD)** demonstrate **6–10% improvement** over state-of-the-art methods across five degradation conditions: occlusion, blur, brightness, trajectory variation, and scale variation.

---

## 📐 **Framework Overview**

<div align="center">
  <img width="600" alt="Overview Architecture" src="https://github.com/sanket0707/Bimodal-SegNet/assets/43345233/4337f390-d334-4b7c-9ec8-7a2f37b9ca1b">
</div>

---

## 📦 **Dataset**

The method is evaluated on the **Event-based Segmentation (ESD) Dataset**, publicly available on Figshare:

🔗 **[Download Full Dataset Collection](https://springernature.figshare.com/collections/A_Neuromorphic_Dataset_for_Object_Segmentation_in_Indoor_Cluttered_Environment/6432548/1)**

1. **[ESD1 Dataset](https://springernature.figshare.com/articles/dataset/ESD-2/22109120?backTo=%2Fcollections%2FA_Neuromorphic_Dataset_for_Object_Segmentation_in_Indoor_Cluttered_Environment%2F6432548&file=39281702)**
2. **[ESD2 Dataset](https://springernature.figshare.com/articles/dataset/ESD-1/22109117?backTo=%2Fcollections%2FA_Neuromorphic_Dataset_for_Object_Segmentation_in_Indoor_Cluttered_Environment%2F6432548&file=39281594)**

---

## 📚 **Cite This Article**

If you use this work in your research, please cite:

```bibtex
@misc{kachole2023bimodal,
    title     = {Bimodal SegNet: Instance Segmentation Fusing Events and RGB Frames for Robotic Grasping},
    author    = {Sanket Kachole and Xiaoqian Huang and Fariborz Baghaei Naeini and Rajkumar Muthusamy and Dimitrios Makris and Yahya Zweiri},
    year      = {2023},
    eprint    = {2303.11228},
    archivePrefix = {arXiv},
    primaryClass  = {cs.CV},
}
```

---

## 💻 **Code Implementation**

This repository contains the full implementation of **Bimodal SegNet**, including:

* Event encoder
* RGB encoder
* Spatial Pyramid Pooling + Atrous Convolutions
* Dual-stream fusion
* Segmentation decoder
* Training & evaluation scripts

---

## 🛠 **Requirements**

* Python **3.7**
* TensorFlow **2.11.0**
* NumPy
* SciPy
* OpenCV
* Matplotlib
  (Install instructions can be added if you want.)
