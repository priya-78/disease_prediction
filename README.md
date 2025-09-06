# 🌱 Crop Disease Detection using Deep Learning


### 📌 Major Project – Corizo Machine Learning Internship  
👨‍💻 Group Project (3 Members)  

---

## 📖 Project Overview  
This project was developed as part of the **Corizo Machine Learning Internship (Aug–Sept 2025)**.  
It focuses on detecting plant leaf diseases using **Deep Learning (CNNs)**. By classifying crop leaf images into disease categories, the system helps farmers identify plant health issues early and take preventive measures.  

---

## 👥 Team Members  
- **Member 1:** Ranga Priya A  
- **Member 2:** Nirjjalaa C R  
- **Member 3:** Sarathi

## 📂 Dataset
- **Source**: [PlantVillage Dataset (Kaggle)](https://www.kaggle.com/datasets/emmarex/plantdisease)  
- **Total Images used**: ~15,000
- **Dataset used**: [training dataset](https://drive.google.com/drive/folders/1Sh6L9A7qOJRSfOpn0D8Zji5vfueutPP4?usp=drive_link)
- **Classes used for training**: 16  
  - Apple (Scab, Black Rot, Healthy)  
  - Corn (Common Rust, Northern Leaf Blight, Healthy)  
  - Grape (Black Rot, Esca, Healthy)  
  - Potato (Early Blight, Late Blight, Healthy)  
  - Tomato (Early Blight, Late Blight, Leaf Mold, Mosaic Virus, etc.)  
- **Structure**: Each class stored in a separate folder.  

---

## 🧠 Model Architecture
- **Framework**: TensorFlow / Keras  
- **Preprocessing**: ImageDataGenerator (rescale, train/validation split)  
- **Layers**: Custom CNN with Conv2D, MaxPooling, Dense, Dropout  
- **Optimizer**: Adam  
- **Loss Function**: Categorical Crossentropy  

---

## 📊 Results
- ✅ **Training Accuracy**: 95.40%  
- ✅ **Validation Accuracy**: 95.73%  
- ✅ **Validation Loss**: 0.1134  
- ✅ **Training Loss**: 0.1192  

**Example Prediction:**  
Input: 🍅 Tomato Leaf
Predicted: Tomato___Late_blight
Confidence: 92%


---

## 🚀 How to Run
1. **Clone the repo**  
   git clone https://github.com/yourusername/crop-disease-detection.git
   cd crop-disease-detection
2. **Install requirements**
   pip install -r requirements.txt
3. **Run training (Google Colab recommended)**
   jupyter notebook disease_pred.ipynb


## 📌 Future Work
🌐 Build a Gradio/Streamlit dashboard for image upload & predictions

☁️ Deploy model as a web application

🌾 Expand dataset with more crops and diseases
