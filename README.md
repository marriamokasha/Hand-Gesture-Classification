# Hand Gesture Recognition using MediaPipe & Machine Learning

This project detects and classifies 18 hand gestures from video input using MediaPipe and a trained machine learning model. It processes each frame to detect hand landmarks, extracts features, predicts the gesture, and overlays the result on the video.


## 🎯 Project Objective 
Build a real-time gesture recognition system that can identify hand gestures from video using MediaPipe for landmark detection and a machine learning classifier trained on gesture data.


## 📊 Model Performance
Multiple models were trained to identifiy hand gestures:
* **XGBoost** → 98.11% → Tuned to 98.27%
* **KNN** → 98.01% (best with default settings)
* **Random Forest** → 97.46%
* **SVM** → 97.07%
* **Decision Tree** → 95.13%
  
> **🏆 Final model:** XGBoost (optimized)
> 
> `{ 'subsample': 0.6, 'n_estimators': 500, 'max_depth': 3, 'learning_rate': 0.2 }`


## 📹 Output Sample
You can see a short demo of the final result here https://drive.google.com/drive/folders/1fGR_xOG9IPiV1bGYd8SFOKNYWlz2AKOq?usp=sharing 


## 📌 Notes
* Landmarks are normalized using the distance between the wrist and finger base (not fingertip). This showed better performance in experimentation.
* All preprocessing, training, and evaluation is included in the notebook.
