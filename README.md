# 🎭 Age, Gender & Emotion Detection 🤖🧠

Welcome to my Deep Learning project! This repo contains a real-time system that detects a person's **age 👶🧓**, **gender 🚹🚺**, and **emotion 😄😢😡** from live webcam footage using CNNs.

---


## 🧩 Problem Statement

🎯 Build a system that can:
- Predict **Age** (as a continuous value) 🎂
- Classify **Gender** as Male 🚹 or Female 🚺
- Detect **Emotion** like Happy 😄, Sad 😢, Angry 😡, and more

All in **real-time** via a webcam! 📷

---

## 🗂️ Datasets Used

| Task              | 📁 Dataset     | 🔢 Size         |
|------------------|----------------|-----------------|
| Age & Gender     | UTKFace        | 1,523 images 🖼️ |
| Emotion Detection| Kaggle Emotion | 4,176 images 🎭 |

📊 Emotion Split: 75% Training, 25% Testing

---

## 🧱 Model Architectures

### 🧓 Age Detection Model
- 🧠 Regression output
- 🏗️ 4 convolutional layers: 128 → 128 → 256 → 512
- ⚙️ Activation: ReLU
- 🧮 Output: Age in years

### 🚻 Gender Detection Model
- 🧠 Binary Classification (Male/Female)
- 🏗️ 5 convolutional layers: 36 → 64 → 128 → 256 → 512
- ⚙️ Activation: ReLU & Sigmoid
- 🧮 Output: 0 (Male) or 1 (Female)

### 🎭 Emotion Detection Model
- 🧠 Multi-class Classification
- 🏗️ 4 convolutional layers: 32 → 64 → 128 → 256
- 🧪 Activation: ReLU & Softmax
- 🤹 Labels: Angry 😠, Disgust 🤢, Fear 😨, Happy 😄, Neutral 😐, Sad 😢, Surprise 😲

---

## 📈 Training Results

| Task              | 📊 Accuracy | 🏁 Epochs |
|-------------------|-------------|-----------|
| Age & Gender      | 79.52% ✅   | 50 ⏱️     |
| Emotion Detection | 78.12% 😊   | 50 ⏱️     |

🖼️ Input size: 200x200 (Age/Gender), 48x48 (Emotion)

---

## 🖥️ Real-Time Detection Pipeline

🎥 Webcam stream with:
- 👁️ Face detection via Haar Cascade
- 🧠 Face input to Age, Gender & Emotion models
- 🧾 Labels drawn with OpenCV `cv2.putText()`
- 📦 Combined prediction loop for all 3 models
- 👨‍👩‍👧‍👦 Multi-face detection supported!

✨ Output Example:
Age: 24 👦
Gender: Male 🚹
Emotion: Happy 😄


---

## 🏁 Final Results

✅ All three models work together in real-time  
🧪 Predictions visible directly on webcam feed  
📷 Detects multiple faces simultaneously  

---

## 🚀 Future Improvements

🔬 Improve under low-light conditions 🌙  
📏 Handle faces at various distances and angles  
🧠 Enhance dataset diversity  
📱 Deploy lightweight model on mobile and edge devices  

---

## 📚 References

📖 Ijjina et al., ICCCNT 2020  
📖 Rafique et al., ICIC 2019  
📖 Agbo-Ajala & Viriri, IEEE Access 2020  
📖 Tawhid & Dey, IJCA 2018  

---

## 🧠 Conclusion

This project demonstrates a successful application of CNNs in real-time facial analysis 🧠📷. It shows strong performance for:
- Age Estimation 🎂  
- Gender Classification 🚻  
- Emotion Recognition 🎭  

👨‍🔬 With further tuning and dataset expansion, the model can be scaled for production-ready applications such as:
- Surveillance 👮
- Retail analytics 🛍️
- Healthcare diagnostics 🏥

---


