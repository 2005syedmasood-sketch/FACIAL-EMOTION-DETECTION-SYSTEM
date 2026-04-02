# 🎭 Facial Emotion Detection using CNN

## 📌 Project Description
This project detects human facial emotions in real-time using a Convolutional Neural Network (CNN). It captures video from a webcam, detects faces, and classifies emotions such as Happy, Sad, Angry, and Neutral.

This system can be useful in mental health monitoring, human-computer interaction, and behavior analysis.

---

## 🚀 Features
- Real-time emotion detection using webcam  
- Face detection using Haar Cascade (OpenCV)  
- CNN-based emotion classification  
- Supports multiple emotions  
- Simple and lightweight implementation  

---

## 🧠 Technologies Used
- Python  
- TensorFlow / Keras  
- OpenCV  
- NumPy  
- Pandas  

---

## 📂 Project Structure
project/
│── train/
│ ├── angry/
│ ├── disgust/
│ ├── fear/
│ ├── happy/
│ ├── neutral/
│ ├── sad/
│ └── surprise/
│
│── test/
│ ├── angry/
│ ├── disgust/
│ ├── fear/
│ ├── happy/
│ ├── neutral/
│ ├── sad/
│ └── surprise/
│
│── train.py
│── detect.py
│── emotion_model.h5
│── README.md


---

## 📊 Dataset Details
- Total images: ~27,000  
- Classes: 7 (angry, disgust, fear, happy, neutral, sad, surprise)  
- Images per class: ~2,700  
- Image size: 48 × 48 pixels  
- Color mode: Grayscale  

---

## ⚙️ Model Architecture
- Conv2D (32 filters, 3x3) + ReLU  
- MaxPooling (2x2)  
- Conv2D (64 filters, 3x3) + ReLU  
- MaxPooling (2x2)  
- Flatten  
- Dense (128) + ReLU  
- Dropout (0.5)  
- Dense (7) + Softmax  

---

## 🏋️ Training the Model

Run the following command:

```bash
python train.py
Training Configuration
Epochs: 5
Batch size: 64
Optimizer: Adam
Loss function: categorical_crossentropy

After training, the model will be saved as:

emotion_model.h5
🎥 Real-Time Emotion Detection

Run the webcam detection:

python detect.py
Controls
Press q to exit
🧪 Output Emotions

The model predicts the following emotions:

Angry
Disgust
Fear
Happy
Neutral
Sad
Surprise
Final Display Mapping
Happy → Happy
Sad → Sad
Angry → Angry
Others → Neutral
⚠️ Known Issues
"Romantic" emotion is not part of the dataset (bug in code)
Accuracy is limited due to fewer training epochs
Performance depends on lighting and camera quality
📌 Future Improvements
Increase training epochs for better accuracy
Apply data augmentation
Use deeper CNN or transfer learning (ResNet, VGG)
Add more emotion classes
Deploy as a web or mobile application
Add emotion history tracking
👨‍💻 Author

Syed Masood Ali, Mohammed Maaz Ashraf, Ayaan Khan

⭐ Acknowledgment

This project is built for learning and academic purposes in the field of Computer Vision and Machine Learning.
