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
## 1.Create Environment first 
## 2.Requirements
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

## Supported Versions
To ensure compatibility with the project, use the following package versions. These are the only supported versions for this project:

```bash
absl-py==2.1.0
astunparse==1.6.3
attrs==24.2.0
cachetools==5.4.0
certifi==2024.7.4
charset-normalizer==3.3.2
contourpy==1.2.1
cvzone==1.5.6
cycler==0.12.1
dagrt==2021.1
exceptiongroup==1.2.2
flatbuffers==1.12
fonttools==4.53.1
gast==0.4.0
google-auth==2.33.0
google-auth-oauthlib==0.4.6
google-pasta==0.2.0
grpcio==1.65.4
h5py==3.11.0
idna==3.7
importlib_metadata==8.2.0
importlib_resources==6.4.0
iniconfig==2.0.0
keras==2.9.0
Keras-Preprocessing==1.1.2
kiwisolver==1.4.5
leap==2021.1
libclang==18.1.1
Mako==1.3.5
Markdown==3.6
MarkupSafe==2.1.5
matplotlib==3.9.1.post1
mediapipe==0.9.1.0
MouseInfo==0.1.3
numpy==1.23.5
oauthlib==3.2.2
opencv-contrib-python==4.10.0.84
opencv-python==4.10.0.84
opt-einsum==3.3.0
packaging==24.1
pillow==10.4.0
pip==24.1.2
platformdirs==4.3.6
pluggy==1.5.0
protobuf==3.19.6
pyasn1==0.6.0
pyasn1_modules==0.4.0
PyAutoGUI==0.9.54
PyGetWindow==0.0.9
pymbolic==2022.2
PyMsgBox==1.0.9
pyobjc-core==10.3.1
pyobjc-framework-Cocoa==10.3.1
pyobjc-framework-Quartz==10.3.1
pyparsing==3.1.2
pyperclip==1.9.0
PyRect==0.2.0
PyScreeze==1.0.1
pytest==8.3.3
python-dateutil==2.9.0.post0
pytools==2024.1.14
pytweening==1.2.0
requests==2.32.3
requests-oauthlib==2.0.0
rsa==4.9
rubicon-objc==0.4.9
setuptools==70.3.0
six==1.16.0
tensorboard==2.9.1
tensorboard-data-server==0.6.1
tensorboard-plugin-wit==1.8.1
tensorflow==2.9.1
tensorflow-estimator==2.9.0
tensorflow-io-gcs-filesystem==0.37.1
termcolor==2.4.0
tomli==2.0.1
typing_extensions==4.12.2
urllib3==2.2.2
Werkzeug==3.0.3
wheel==0.44.0
wrapt==1.16.0
zipp==3.20.0
```
## 🎥 Reference video  
🎥 [Watch the Video](https://youtu.be/wa2ARoUUdU8?si=gyHoOB04tL9rhA9n)
