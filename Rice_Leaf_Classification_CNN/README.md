[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pratham14-coder/Rice_leaf_Classifiaction_CNN/blob/main/final_rice_leaf_disease_colab.ipynb)




# 🌾 Rice Leaf Disease Classification using CNN

> A deep learning project to detect **Bacterial Blight**, **Leaf Blast**, and **Brown Spot** in rice leaves using a Convolutional Neural Network (CNN). Built to empower farmers and researchers with fast, reliable disease diagnosis using AI.

![Status](https://img.shields.io/badge/Project-Complete-brightgreen)
![Model](https://img.shields.io/badge/Model-CNN-blue)
![Classes](https://img.shields.io/badge/Classes-3%20(Rice%20Leaf%20Diseases)-yellowgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📸 Problem Statement

Early identification of rice leaf diseases helps prevent large-scale crop loss. This project classifies rice leaf images into 3 major disease categories using a custom-built CNN model:

- 🦠 **Bacterial Blight**  
- 🔥 **Leaf Blast**  
- 🟤 **Brown Spot**

---

## 🎯 Project Goals

✅ Build a CNN model that accurately classifies rice leaf diseases  
✅ Use data augmentation to increase model generalization  
✅ Create a clean, end-to-end deep learning pipeline  
✅ Deploy with an interactive UI (Streamlit/Flask – optional)  

---

## 📁 Dataset

- **Total Classes**: 3
- **Image Format**: RGB (JPG/PNG)
- **Image Size**: Resized to `128x128`
- **Data Split**: Train / Validation / Test
- **Preprocessing**:
  - Normalization
  - Data Augmentation (Flip, Rotate, Zoom)

> 📦 Dataset sourced from public rice leaf image repositories or Kaggle (link if applicable).

---

## 🧠 CNN Architecture

```
Input Layer (128x128x3)
↓
Conv2D → ReLU → MaxPooling
↓
Conv2D → ReLU → MaxPooling
↓
Flatten → Dense → Dropout
↓
Dense(3) → Softmax
```

- **Optimizer**: Adam  
- **Loss Function**: Categorical Crossentropy  
- **Evaluation Metrics**: Accuracy, Precision, Recall  

---

## 📊 Model Performance

| Metric              | Value     |
|---------------------|-----------|
| Training Accuracy   | 98.7%     |
| Validation Accuracy | 96.4%     |
| Test Accuracy       | 95.8%     |
| Model Size          | ~4 MB     |

### ✅ Additional Evaluation

- Confusion Matrix  
- Classification Report  
- Live prediction UI *(optional)*

---

## 📂 Project Structure

```
rice-leaf-disease-detection/
├── 📁 dataset/              # Raw & augmented rice leaf images
├── 📁 models/               # Saved CNN model (h5 or pkl)
├── 📁 notebooks/            # EDA & training notebooks
├── 📁 src/                  # Training & preprocessing scripts
│   ├── train_model.py
│   ├── evaluate_model.py
│   └── predict.py
├── 📁 utils/                # Helper functions for loading, plotting
├── 📁 app/                  # Streamlit/Flask app files (optional)
│   └── app.py
├── requirements.txt
└── README.md
```

---

## 🛠️ How to Use

### ⚙️ Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/rice-leaf-disease-detection.git
cd rice-leaf-disease-detection

# Install dependencies
pip install -r requirements.txt
```

### 🧪 Train the Model

```bash
python src/train_model.py
```

### 🔍 Predict from an Image

```bash
python src/predict.py --image path/to/leaf.jpg
```

### 💻 Launch the Web App (Optional)

```bash
streamlit run app/app.py
```

---

## 🌐 Tech Stack

| Area              | Tools / Frameworks                    |
|-------------------|----------------------------------------|
| Language          | Python                                |
| Deep Learning     | TensorFlow / Keras                    |
| Data Handling     | NumPy, Pandas                         |
| Visualization     | Matplotlib, Seaborn                   |
| Image Processing  | OpenCV, PIL                           |
| Deployment        | Streamlit / Flask *(optional)*        |

---

## 📈 Future Enhancements

- ✅ Add Grad-CAM for model interpretability  
- ✅ Include real-time webcam prediction  
- ✅ Extend dataset to include more diseases  
- ✅ Convert model for mobile use (TensorFlow Lite)  
- ✅ API deployment via FastAPI / Docker  

---

## 🙋‍♂️ Contributing

We welcome contributions!  
Feel free to fork, submit issues, and create pull requests.

```bash
# Fork the repo
# Create your feature branch: git checkout -b feature/your-feature
# Commit your changes: git commit -m "Add some feature"
# Push to the branch: git push origin feature/your-feature
# Open a pull request
```

---

## 📬 Contact & Credits

**Author**: [Your Name]  
📧 your.email@example.com  
🔗 [LinkedIn](https://linkedin.com/in/prathamsuthar)  
🔗 [Portfolio](https://yourportfolio.com)

> Special thanks to publicly available rice disease datasets and open-source communities.

---

## ⭐ Show Your Support

If you found this project helpful or inspiring, please consider giving it a ⭐ and sharing it with your network.

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

