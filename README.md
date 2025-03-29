# SignAura: Accessible Learning Platform for Deaf and Mute Students

SignAura is a project aimed at breaking communication barriers for deaf and mute students by providing an innovative and accessible learning platform. It integrates cutting-edge technology to foster inclusivity in education, enabling students to learn effectively in environments that may lack resources, such as sign language proficiency among parents and educators.

---

## Features

### 1. **Learning Modules**
- **Sign Gesture Videos**: Tutorials for commonly used words, alphabets, and numbers.
- **Subject Tutorials**: Basic subjects like Mathematics, Science, and Grammar with sign-assisted explanations.
- **Interactive Dictionary**: A searchable collection of words and their corresponding hand gestures.
- **Supplementary Resources**: Additional learning aids to enhance understanding and engagement.

### 2. **SignaMate: AI-Powered Chatbot**
- **Speech/Text to Sign Translation**: Converts spoken or written language into corresponding sign language gestures.
- **Sign to Text/Speech Conversion**: Converts sign language gestures into text or speech for seamless two-way communication.

### 3. **Dashboard**
- A user-friendly dashboard to track the student’s learning progress and provide insights for educators and parents.

---

## Gesture Recognition Module
The gesture recognition system is a key component of SignAura, enabling the identification and interpretation of hand gestures in real-time.

### **Steps to Implement Gesture Recognition**

#### **1. Data Collection**
- Captures hand gesture landmarks using Mediapipe’s Hand module.
- Saves data as `.npy` files for training purposes.

#### **2. Model Training**
- Utilizes a **Support Vector Classifier (SVC)** with a linear kernel for gesture classification.
- Prepares training data by flattening hand landmark arrays and associating them with gesture labels.
- Achieves accurate recognition with robust generalization.

#### **3. Real-Time Gesture Recognition**
- Uses a webcam feed to detect hand gestures in real-time.
- Recognizes gestures and maps them to predefined labels (e.g., numbers 0-9).
- Displays the recognized gesture on-screen.

---

## Technologies Used

1. **Programming Language**: Python
2. **Machine Learning**: Scikit-learn (SVM for gesture classification)
3. **Computer Vision**: OpenCV and Mediapipe for hand tracking
4. **Data Handling**: NumPy for managing landmark data
5. **Model Persistence**: Pickle for saving and loading trained models

---

## Installation Guide

### **Prerequisites**
- Python 3.8 or above
- Libraries: Mediapipe, OpenCV, NumPy, Scikit-learn, Pickle

### **Setup**
1. Clone the repository:
   ```bash
   git clone https://github.com/username/SignAura.git
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Prepare the dataset for gesture recognition:
   - Run the `DataCollection.py` script to collect hand gesture data.
   - Organize data into labeled folders under the `Data` directory.

4. Train the model:
   - Execute the `ModelTraining.py` script to train and save the SVM model.

5. Test real-time gesture recognition:
   - Run the `GestureRecognition.py` script.

---

## Usage

1. Launch the SignAura platform to access learning modules and AI-powered chatbot.
2. Use the gesture recognition module for hands-on interaction and learning.
3. Monitor student progress using the dashboard.

---

## Project Goals
- Empower deaf and mute students by providing them with tools for self-paced and inclusive learning.
- Bridge the communication gap between students and their families or educators.
- Scale the solution to make it accessible across diverse communities globally.

---

## Team Member

- Krishna Moghe
- Zaid Md Saikh
- Jainil Patel
- Palak Patel
  
## Contribution
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and submit a pull request.

---

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

---

## Contact
For questions or suggestions, please contact:
- **Name**: Krishna Moghe
- **Email**: krishnamoghe74@gmail.com

---

Thank you for being part of this journey to make education more accessible and inclusive!

