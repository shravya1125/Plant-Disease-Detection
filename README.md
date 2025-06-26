# Plant Disease Detection using Deep Learning

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.12-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Deployed-brightgreen?logo=streamlit)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

## Overview

This project focuses on detecting diseases in plants using **Convolutional Neural Networks (CNN)** trained on leaf images. It helps farmers and agricultural experts identify diseases early, ensuring timely intervention and improved crop health.

> Built with deep learning + image classification  
> Accessible via a simple **Streamlit web app**  
> Achieved **over 95% accuracy** on validation set

---

**Accuracy/Loss Graphs**

![image](https://github.com/user-attachments/assets/57d9e0ed-21e5-4643-9ae4-cde06276290d)

![image](https://github.com/user-attachments/assets/bc0215dd-32ad-490c-ae28-f23e5c31bb8f)


## 📂 Dataset

- **Dataset Used**: [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)
- **Classes**: 5 disease types (incl. healthy leaves)
- **Format**: RGB JPEG images organized by class folders

---

## Tech Stack

| Component         | Description                                 |
|------------------|---------------------------------------------|
| **Python**        | Core language for development               |
| **TensorFlow / Keras** | Model building and training            |
| **OpenCV**        | Image preprocessing                         |
| **Streamlit**     | Frontend UI for model prediction            |
| **Matplotlib**    | Visualizations during model evaluation      |

---

## Model Architecture

- **Base Model**: Custom CNN with 3 Conv layers + Dense layers  
- **Input Shape**: 128x128x3  
- **Activation**: ReLU, Softmax  
- **Loss Function**: Categorical Crossentropy  
- **Optimizer**: Adam

> Trained for 50 epochs on GPU with early stopping  
> Achieved ~97% training accuracy and ~95% validation accuracy

---

## Preview with gradio
![Screenshot (8)](https://github.com/user-attachments/assets/117d8f14-d2d2-48f5-bfd2-8efc1ddfc99f)

## How to Run Locally

1. **Clone the Repo**
   ```bash
   git clone https://github.com/shravya1125/Plant-Disease-Detection.git
   cd Plant-Disease-Detection

2. **Install Requirements**
   ```bash
   pip install -r requirements.txt

3. **Launch Streamlit App**
   ```bash
   streamlit run app.py

4. **Upload Leaf Image**

   Upload any leaf image (.jpg/.png)
   Get instant disease prediction with confidence score


