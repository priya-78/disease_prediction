# 🌱 Crop Disease Detection using Deep Learning

## 📌 Project Overview
This project detects **plant leaf diseases** using a Convolutional Neural Network (CNN).  
It classifies images of leaves into their respective disease categories, helping farmers identify crop health early.

---

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
