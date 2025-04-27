## American Sign Language (ASL) Detection
This project is designed to detect American Sign Language (ASL) hand gestures for alphabets (A to Z) and common words such as "HELLO", "GOODJOB", "YES", "NO", "PLEASE", "THANKYOU", and "SORRY". It utilizes OpenCV and MediaPipe for hand tracking and a Keras model for gesture classification.

## 📸 Screenshots
![Screenshot 2025-04-27 at 2 19 20 PM](https://github.com/user-attachments/assets/ddee53b0-ac89-4fa7-ac96-c21eaa16ce00)

## 🎥 Project Explanation Video
🎥 [Watch the Video](https://www.linkedin.com/posts/sathiyapriya-s-22ucs048_signlanguage-ai-asl-activity-7237472839723859968-59QU?utm_source=share&utm_medium=member_desktop&rcm=ACoAAEKubiABTjioeFLfoGOrHXFNNCGvYJ6moX8)

## Features
Hand Tracking: Uses MediaPipe to detect hands and track the position of the hand in the camera feed.

ASL Gesture Recognition: Classifies gestures for the English alphabet (A-Z) and common words.

Real-Time Detection: Provides real-time feedback on hand gestures displayed in the video feed.

Custom Model: Uses a custom-trained Keras model to recognize gestures based on hand positioning.

## Requirements
Before running the project, ensure the following dependencies are installed:

OpenCV - For image processing and camera access.

```bash
pip install opencv-python
```
cvzone - For hand detection and classification.

```bash
pip install cvzone
```

NumPy - For numerical operations.

```bash
pip install numpy
```
Keras - For machine learning model.

```bash
pip install keras
```
## Setup
Clone the repository or download the project files.

## Make sure you have the following files in your project directory:

## Data folder containing labeled images for training.

Model folder containing the pre-trained model (keras_model.h5).

Labels file (labels.txt) that contains the labels for gestures (A-Z, common words).

datacollection.py (for collecting training data).

test.py (for testing the ASL detection).

## Set up a virtual environment and install the dependencies using the following command:

```bash
pip install -r requirements.txt
```
## Run the test script to start real-time ASL detection:

```bash
python test.py
```

## How It Works
Hand Detection: The HandDetector from the cvzone library is used to detect hands in the video feed.

Gesture Classification: A pre-trained Keras model (keras_model.h5) is used to classify the detected gestures.

Image Preprocessing: The detected hand is cropped and resized to a fixed size to match the input requirements of the model.

Real-Time Prediction: The model predicts the gesture and displays the corresponding label on the screen.

## Model Training
You can train your own model using the provided datacollection.py script:

Collect Data: Use the script to capture images of each gesture. Save the images in corresponding folders (Data/A, Data/B, etc.) for each class.

Train Model: Train a deep learning model using Keras and the collected data.

The model should be saved as keras_model.h5 in the Model folder.

Label File: The labels.txt file should contain a list of all the classes (A-Z, words like "HELLO", "YES", etc.).

## Key Features
Real-Time Detection: ASL gestures are detected and displayed in real-time.

Gesture-to-Text: The corresponding gesture is shown as text on the screen.

Custom Model Compatibility: Easily integrates with any Keras-based model for gesture recognition.

## Controls
Hand Gesture Recognition: Hold your hand in front of the camera, and the system will recognize your gesture.

Display: The recognized gesture is displayed in the top-left corner of the image feed.
