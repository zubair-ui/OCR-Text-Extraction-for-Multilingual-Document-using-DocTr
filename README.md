# OCR-Text-Extraction-for-Multilingual-Document-using-DocTr

This project implements **Optical Character Recognition (OCR) for multilingual document text extraction** using the [DocTR (Document Text Recognition)](https://github.com/mindee/doctr) library. The goal is to detect and recognize text regions in scanned documents, forms, and multilingual datasets to build a foundation for intelligent document processing systems.

---

## Features

- Text detection using deep learning–based detection models.
- Text recognition for multilingual documents.
- Preprocessing of document images for better OCR results.
- Training pipeline for both detection and recognition tasks.
- Evaluation and performance tracking.

---

## Dataset

We trained and evaluated our models on the following datasets:

- [Xfund and FUNSD Dataset](https://www.kaggle.com/datasets/zubairalibhutto/xfund-and-funsd)
  - **FUNSD**: Form Understanding in Noisy Scanned Documents, a benchmark for document understanding on noisy scanned forms.
  - **XFUND**: A large-scale multilingual dataset designed for form understanding, covering multiple languages and document layouts.

### Languages Covered

This project focuses on OCR text extraction across **8 languages**:

- **English**
- **Chinese**
- **Japanese**
- **Portuguese**
- **Italian**
- **Spanish**
- **German**
- **French**

These languages make the dataset well-suited for multilingual document analysis, enabling the model to generalize better across diverse regions and scripts.

---

## Model Training

The training pipeline is divided into two stages:

1. **Text Detection Model**

   - Detects bounding boxes of text regions in document images.
   - Achieved an accuracy of **88.94%** on validation data.

2. **Text Recognition Model**
   - Recognizes and transcribes text from detected bounding boxes.
   - Performance was not as strong due to **time limitations on Kaggle** and **hardware resource constraints** during training.

---

## Tech Stack

- Python
- TensorFlow/Keras
- [DocTR](https://github.com/mindee/doctr)
- Jupyter Notebook

---

## Results

- **Detection Model Accuracy**: 88.94%
- **Recognition Model**: Performance lower due to limited compute resources and restricted Kaggle runtime.

---

---

## Future Improvements

- Train recognition model longer on high-performance GPUs for better accuracy.
- Experiment with transformer-based OCR models.
- Expand dataset with more multilingual documents.
- Optimize inference pipeline for deployment.

---

## ✨ Acknowledgements

- [Mindee - DocTR](https://github.com/mindee/doctr)
- [FUNSD & XFUND Dataset](https://www.kaggle.com/datasets/zubairalibhutto/xfund-and-funsd)
