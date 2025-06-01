# Hand Gesture Recognition using MediaPipe & Machine Learning

This project detects and classifies 18 hand gestures from video input using MediaPipe and a trained machine learning model. It processes each frame to detect hand landmarks, extracts features, predicts the gesture, and overlays the result on the video.


## 🎯 Project Objective 
Build a real-time gesture recognition system that can identify hand gestures from video using MediaPipe for landmark detection and a machine learning classifier trained on gesture data.


## 📊 Model Performance
Multiple models were trained to identifiy hand gestures:
* **XGBoost** → 98.1% → Tuned to 98.3%
* **KNN** → 98.0% (best with default settings)
* **Random Forest** → 97.5%
* **SVM** → 97.1%
* **Decision Tree** → 95.1%
  
> **🏆 Final model:** XGBoost (optimized)
> 
> `{ 'subsample': 0.6, 'n_estimators': 500, 'max_depth': 3, 'learning_rate': 0.2 }`




## 📌 Notes
* Landmarks are normalized using the distance between the wrist and finger base (not fingertip). This showed better performance in experimentation.
* All preprocessing, training, and evaluation is included in the notebook.
