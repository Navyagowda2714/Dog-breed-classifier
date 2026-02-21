<!-- ===================================================== -->
<!--        Dog Breed Classifier — README.md (Premium)      -->
<!--            Classy • Visual • Recruiter-Ready           -->
<!-- ===================================================== -->

<div align="center">

<!-- ✅ BRAND BANNER (same brand style as your SwiftChat README) -->
<img width="100%" alt="Dog Breed Classifier premium header"
src="https://capsule-render.vercel.app/api?type=waving&color=0:070A12,45:1E3A8A,75:4F46E5,100:06B6D4&height=230&section=header&text=Dog%20Breed%20Classifier&fontSize=64&fontColor=FFFFFF&fontAlignY=40&desc=Image%20Recognition%20%E2%80%A2%20CNNs%20%E2%80%A2%20Transfer%20Learning%20%E2%80%A2%20ResNet50%20%2F%20VGG16%20%E2%80%A2%20OpenCV&descAlignY=70&descSize=18&animation=fadeIn" />

<br/>

<img alt="Python" src="https://img.shields.io/badge/Python-111827?style=for-the-badge&logo=python&logoColor=ffd43b"/>
<img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow%2FKeras-111827?style=for-the-badge&logo=tensorflow&logoColor=ff6f00"/>
<img alt="Computer Vision" src="https://img.shields.io/badge/Computer%20Vision-111827?style=for-the-badge&logo=opencv&logoColor=5CFF73"/>
<img alt="Transfer Learning" src="https://img.shields.io/badge/Transfer%20Learning-111827?style=for-the-badge"/>
<img alt="CNN" src="https://img.shields.io/badge/CNN%20Classifier-111827?style=for-the-badge"/>

<br/><br/>

<a href="#-project-overview"><b>Overview</b></a> •
<a href="#-model-pipeline"><b>Pipeline</b></a> •
<a href="#-results"><b>Results</b></a> •
<a href="#-contact"><b>Contact</b></a>

</div>

---

## ✨ Project Overview

This project is an **end-to-end image recognition pipeline** that predicts the **dog breed** from an input image.  
It also handles real-world input by detecting whether the image contains:

- ✅ a **human face**
- ✅ a **dog**
- ✅ neither (invalid input)

**One-line product summary:**  
**Upload an image → detect (human/dog) → predict dog breed → present a clean final result.**

---

## 🧪 Model Pipeline

<details open>
<summary><b>🐾 Interactive Flow Diagram (click to collapse)</b></summary>
<br/>

<!-- ✅ FIXED Mermaid:
  - Removed "Yes/No" labels from the arrow itself
  - Used edge labels correctly with |label|
  - Avoided parentheses that can sometimes cause parsing issues in node text
-->
```mermaid
flowchart TD
  A["Input Image"] --> B{"Human face detected?"}
  B -->|Yes| C["Face detector — OpenCV"]
  C --> D["Breed classifier — Transfer learning"]
  B -->|No| E{"Dog detected?"}
  E -->|Yes| F["Dog detector — ResNet50"]
  F --> D
  E -->|No| G["Reject / ask for clearer image"]
  D --> H["Predicted breed output"]
```

</details>

### Why this pipeline is practical
- Handles messy user inputs (human photos / unclear images)
- Separates **detection** vs **classification** (clean responsibilities)
- Uses **transfer learning** for strong performance without massive training time

---

## 📊 Results

<!-- ✅ INFOGRAPHIC / CLASSY LOOK (GitHub-safe):
  Use a visual "scorecard" + progress-bar style rows built from badges
-->

<div align="center">

<table>
<tr>
<td width="33%" align="center" valign="top">

### 🏆 Best Model
<b>ResNet50</b><br/>
<sub>Transfer Learning</sub>

<br/>

<img src="https://img.shields.io/badge/Selected_Model-ResNet50-16A34A?style=for-the-badge"/>

</td>

<td width="33%" align="center" valign="top">

### 🎯 Test Accuracy
<b>82.8947%</b><br/>
<sub>Breed classification</sub>

<br/>

<img src="https://img.shields.io/badge/Accuracy-82.89%25-0EA5E9?style=for-the-badge"/>

</td>

<td width="33%" align="center" valign="top">

### 🧠 CV Decision Logic
<b>Human / Dog / Invalid</b><br/>
<sub>Before predicting</sub>

<br/>

<img src="https://img.shields.io/badge/Input_Gate-Enabled-7C3AED?style=for-the-badge"/>

</td>
</tr>
</table>

</div>

<br/>

<div align="center">

<!-- Infographic-style comparison -->
<table>
<tr>
<td width="60%" valign="top">

### 📈 Accuracy Progression (Model Evolution)

<b>Baseline CNN (from scratch)</b><br/>
<img src="https://img.shields.io/badge/14.23%25-111827?style=for-the-badge&label=Accuracy&labelColor=0B1220"/>

<br/><br/>

<b>VGG16 (transfer learning)</b><br/>
<img src="https://img.shields.io/badge/41.63%25-111827?style=for-the-badge&label=Accuracy&labelColor=0B1220"/>

<br/><br/>

<b>ResNet50 (transfer learning)</b><br/>
<img src="https://img.shields.io/badge/82.89%25-111827?style=for-the-badge&label=Accuracy&labelColor=0B1220"/>

</td>

<td width="40%" valign="top">

### 🔍 What Improved

- Better feature extraction (pretrained backbones)  
- Faster convergence than training from scratch  
- More stable generalization on unseen images  
- Cleaner separation: detect → classify  

<br/>

<img src="https://img.shields.io/badge/Outcome-Production--style%20Pipeline-16A34A?style=for-the-badge"/>

</td>
</tr>
</table>

</div>

---

## 💼 Why This Project Is Recruiter-Relevant

- Demonstrates **computer vision reasoning**, not just model training
- Shows measurable improvement from baseline → transfer learning
- Uses a clean decision pipeline (human/dog/invalid): product thinking
- Covers the complete workflow:
  - preprocessing
  - CNN training
  - transfer learning
  - evaluation
  - end-to-end inference logic

---

## 🤝 Contact

<div align="center">

<a href="https://www.linkedin.com/in/navyashree-byregowda-472821196/">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-1E40AF?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="https://github.com/Navyagowda2714">
  <img src="https://img.shields.io/badge/GitHub-Portfolio-111827?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<a href="mailto:navyashreebyregowda@gmail.com">
  <img src="https://img.shields.io/badge/Email-Let's%20Talk-DC2626?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<br/><br/>
<sub>Dog Breed Classifier — built as an end-to-end CV pipeline (not just a model).</sub>

</div>
