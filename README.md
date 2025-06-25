# 🍐 Pear Leaf Disease Detection using Siamese CNN & VAE

This project presents a hybrid deep learning approach for automated detection and classification of pear leaf diseases using a combination of **Siamese Convolutional Neural Networks (SCNN)**, **Variational Autoencoders (VAE)**, and an **SVM classifier**. The goal is to enable early detection of plant diseases in data-scarce agricultural settings.

---

## 🚀 Model Highlights

- **Siamese CNN:** Learns to compare pairs of leaf images for visual similarity.
- **Variational Autoencoder (VAE):** Encodes high-level latent features to aid classification and enhance generalization.
- **Feature Fusion:** Combines SCNN embeddings and VAE latent vectors into a joint 240-dimensional representation (`enhanced_z`).
- **Contrastive Learning:** Enables learning of disease-specific similarity under limited labeled data.
- **SVM Classifier:** Trained on the fused latent space for final classification.

---

## 🧠 Techniques Used

- Contrastive loss for similarity learning
- Latent space fusion (`z` + SCNN encodings)
- Reconstruction loss for VAE training
- PCA for latent space visualization
- Data augmentation: flips, rotation, noise, brightness jitter

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Libraries:** TensorFlow / Keras, NumPy, Matplotlib, scikit-learn  
- **Platform:** Google Colab  

---

## 📊 Dataset

- **DiaMOS Plant Dataset**
- Custom-labeled pear leaf disease images
- Multiple classes: fungal, curl, slug, etc.
- Highly imbalanced and small in size (challenging for standard CNNs)

---

## 📈 Results

- Achieved strong class-wise separation in fused latent space
- PCA plots showed high inter-class variance and low intra-class spread
- Significantly improved robustness and generalization via augmentation

---

## 📁 Folder Structure

