# Explainable-AI-based-ECG-Heartbeat-Classification-Using-Deep-Learning-Models
Got it 👍 You uploaded your research paper (PDF) and the Jupyter notebook. Based on both, I’ll draft a **professional README.md** for your GitHub repository. This README will summarize your project, explain the methodology, provide setup instructions, and guide contributors. Here’s a first version:

---

# Explainable AI-Based ECG Heartbeat Classification Using Deep Learning

This repository contains code and resources for the project **"Explainable AI-Based ECG Heartbeat Classification Using Deep Learning Models"**, which leverages **CNN-LSTM-Attention architectures** along with **SHAP** and **LIME** for model interpretability.

The project aims to build **accurate and explainable deep learning models** for classifying ECG heartbeats from the MIT-BIH Arrhythmia Database and PTB Diagnostic ECG Database.

---

## 🚀 Features

* **Deep Learning Models**:

  * Convolutional Neural Networks (CNNs) for spatial feature extraction
  * Long Short-Term Memory (LSTM) networks for temporal dependencies
  * Attention mechanism for focusing on critical ECG segments
* **Explainable AI (XAI)**:

  * **SHAP values** to assess feature contributions
  * **LIME** for local, human-interpretable explanations
* **Performance**:

  * Achieved **98.25% accuracy** and high F1-scores across heartbeat classes

---

## 📊 Datasets

* **MIT-BIH Arrhythmia Database**

  * 109,446 annotated heartbeats
  * Five heartbeat categories: Normal (N), Supraventricular (S), Ventricular (V), Fusion (F), and Unclassifiable (Q)
* **PTB Diagnostic ECG Database**

  * 14,552 diagnostic-quality ECG samples
  * Two-class dataset (healthy vs diseased)

Both datasets are available on [PhysioNet](https://physionet.org/).

---

## 🛠️ Installation & Setup

Clone the repo:

```bash
git clone https://github.com/your-username/ecg-explainable-ai.git
cd ecg-explainable-ai
```

Create a virtual environment and install dependencies:

```bash
python -m venv venv
source venv/bin/activate   # (Linux/macOS)
venv\Scripts\activate      # (Windows)

pip install -r requirements.txt
```

---

## 📓 Usage

Run the Jupyter notebook:

```bash
jupyter notebook ecg-cnn.ipynb
```

The notebook includes:

1. **Data preprocessing** (noise reduction, normalization, augmentation)
2. **Model training** (CNN-LSTM-Attention)
3. **Evaluation** (Accuracy, Precision, Recall, F1-score)
4. **Interpretability analysis** (SHAP & LIME visualizations)

---

## 📈 Results

* Mean F1-score: **98.25%**
* SHAP analysis showed **QRS complex amplitude and duration** were most influential in classification
* LIME visualizations highlighted **P-wave** and **QRS complex** for specific heartbeat types

Example:

* **Supraventricular Premature Beats** → P-wave importance
* **Premature Ventricular Contractions** → QRS complex importance

---

## 📂 Repository Structure

```
.
├── ecg-cnn.ipynb          # Jupyter notebook with implementation
├── Explainable_AI-Based_ECG_Heartbeat_Classification_Using_Deep_Learning_Models.pdf
├── requirements.txt       # Dependencies
├── README.md              # Project documentation
└── /data                  # (Optional) Place datasets here
```

---

## 📌 Future Work

* Incorporate **GAN-based data augmentation**
* Extend model to **other physiological signals**
* Explore more **XAI techniques** (e.g., Grad-CAM, Integrated Gradients)

---

## 🧑‍🤝‍🧑 Authors

* **Rohit Moningi**, Shreya Mahakur, Shradha Mundada, Asis Kumar Tripathy
* School of Computer Science, VIT, Vellore, India

---

## 📜 Citation
https://ieeexplore.ieee.org/document/10870845

```
@inproceedings{moningi2024ecg,
  title={Explainable AI-Based ECG Heartbeat Classification Using Deep Learning Models},
  author={Moningi, Rohit and Mahakur, Shreya and Mundada, Shradha and Tripathy, Asis Kumar},
  booktitle={IEEE International Conference on Artificial Intelligence and Signal Processing (AISP)},
  year={2024}
}
```

---

👉 Do you want me to also create the **requirements.txt** file for dependencies (TensorFlow, PyTorch, SHAP, LIME, etc.) so the repo is ready to run?
