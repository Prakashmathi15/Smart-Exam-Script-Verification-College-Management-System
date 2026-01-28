# 📝 Smart-Exam-Script-Verification-College-Management-System -TEAM 164🚀

![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-ee4c2c.svg)
![Transformers](https://img.shields.io/badge/Hugging%20Face-TrOCR-yellow.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-Image%20Processing-green.svg)

## 📌 Overview

Academic integrity is crucial, but traditional plagiarism checkers (like Turnitin) cannot read **handwritten** assignments. This project bridges that gap.

This is an **End-to-End Automated Pipeline** that ingests scanned PDF submissions, preprocesses them using Computer Vision, extracts text using the state-of-the-art **TrOCR (Transformer-based OCR)** model, and algorithmically compares every student's work against every other student to detect verbatim copying.

## 🚀 Key Features

* **📄 Batch Processing:** Automatically converts and processes folders full of PDF submissions.
* **🖼️ Advanced Preprocessing:** Uses OpenCV for Denoising and Adaptive Thresholding to clean noisy scans.
* **🤖 AI-Powered OCR:** Utilizes `microsoft/trocr-large-handwritten` for superior accuracy on diverse handwriting styles.
* **🔍 Pairwise Comparison:** Compares every document against every other document ($N^2$ complexity) to ensure no copy goes unnoticed.
* **📊 Visual Reports:** Generates a similarity matrix heatmap and a detailed text report flagging suspicious pairs (Threshold > 75%).

---
