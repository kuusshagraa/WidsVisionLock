# Final Project: Face Verification with Siamese Neural Networks

## 🎓 Project Overview
This project is the final submission for a 6-week Neural Network course. The goal is to build a high-accuracy Face Verification system using a **Siamese Neural Network (SNN)**.

### Key Requirements Met:
* **One-Shot Learning:** The model recognizes a face from just one reference image.
* **Personalized Data:** As per the instructions, the base images (anchors) are of my own face.
* **Clean Code:** The implementation is modular, commented, and organized for readability.

## 🏗️ Model Architecture
The model uses a "Twin" architecture where two identical CNNs share the same weights to extract feature vectors.
* **Feature Extractor:** CNN layers reducing images to 4,096-dimensional embeddings.
* **Distance Layer:** A custom L1 Distance layer to calculate similarity between faces.
* **Final Layer:** Sigmoid activation to output a "Match" probability (0 to 1).


## 📂 Repository Structure
* `face_verification_final.ipynb`: Main code notebook with training and results.
* `siamese_model.h5`: The final trained model weights.
* `requirements.txt`: List of required Python libraries.
* `data/`: Contains `anchor`, `positive`, and `negative` image folders.

## 🚀 How to Run
1. Clone this repo.
2. Install dependencies: `pip install -r requirements.txt`.
3. Open the notebook and run the final cell to see the **Match vs No-Match** visualization.

## ✅ Results
The model was trained using **Binary Cross-Entropy Loss** and the **Adam Optimizer**, achieving clear distinction between my face and others.
