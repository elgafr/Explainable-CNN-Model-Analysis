# Explainable CNN Model Analysis for Skin Cancer Detection

## 🩺 Real Medical Dataset Integration + Explainable AI

A comprehensive framework for **explainable AI analysis** of skin cancer detection using **real medical datasets**. This project demonstrates how to apply Grad-CAM and SHAP techniques to authentic dermatological images from clinical sources.

## ✨ Key Features

- **HAM10000 Dataset Support**: Full support for Harvard's dermatoscopic dataset
- **Grad-CAM & SHAP Analysis**: Visual and feature-level explanations for clinical predictions
- **Medical Visualization**: Specialized heatmaps and comparative analysis
- **Robust Data Handling**: Preprocessing and metadata integration for clinical images
- **Comprehensive Results**: Visualizations and evaluation metrics for real data

## 🚀 Quick Start

### 1. Setup Environment
```bash
git clone <repository>
cd Explainable_CNN_Analysis
pip install -r requirements.txt
```

### 2. Prepare the HAM10000 Dataset
- Download from: https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000/data
- Extract all images and metadata to: `data/datasets/HAM10000/`
  - Images should be in `data/datasets/HAM10000/images/`
  - Metadata: `data/datasets/HAM10000/HAM10000_metadata.csv`

### 3. Run Analysis
```bash
jupyter notebook notebooks/train_model.ipynb
```
- The notebook will:
  - Load HAM10000 images and metadata
  - Train and evaluate a CNN model
  - Generate Grad-CAM and SHAP explanations
  - Save results to the `results/` directory

## 📁 Project Structure

```
Explainable_CNN_Analysis/
├── config/
│   └── config.yaml                # Configuration settings
├── data/
│   └── datasets/
│       └── HAM10000/              # HAM10000 dataset (images, metadata)
├── models/
│   ├── skin_cancer_classifier.h5  # Trained model
│   └── training_history.png       # Training history plot
├── notebooks/
│   └── train_model.ipynb          # Main analysis notebook
├── results/
│   ├── real_data/                 # Real dataset visualizations
│   ├── gradcam/                   # Grad-CAM results
│   ├── shap/                      # SHAP analysis
│   ├── analysis/                  # Comparative analysis
│   └── evaluation/                # Evaluation metrics (ROC, confusion matrix)
├── requirements.txt               # Python dependencies
└── README.md                      # This file
```

## 🔬 Analysis Features

- **Authentic Data Loading**: Direct processing of HAM10000 clinical dataset
- **Medical Preprocessing**: Specialized image processing for dermatological images
- **Grad-CAM & SHAP**: Visual and feature-level explanations for model predictions
- **Comprehensive Results**: Visualizations, evaluation metrics, and comparative analysis

## 📊 Results

- Grad-CAM and SHAP visualizations: `results/gradcam/`, `results/shap/`
- Real data analysis: `results/real_data/`
- Comparative and summary analysis: `results/analysis/`
- Evaluation metrics: `results/evaluation/` (ROC curve, confusion matrix)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This framework is designed for **research and educational purposes**. For clinical use:
- Ensure proper medical validation
- Obtain regulatory approval (FDA/CE)
- Follow institutional protocols
- Maintain medical oversight

**Not intended for direct patient diagnosis without qualified medical professional review.**


---

**🩺 Real Medical Data + 🤖 Explainable AI = 🔬 Clinical Innovation** 