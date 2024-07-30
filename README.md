Drowsiness-Detection
Introduction
Drowsiness-Detection is a machine learning project designed to detect driver drowsiness in real-time using computer vision techniques. This project aims to enhance road safety by alerting drivers when signs of drowsiness are detected.

Features
Real-time video processing
Eye aspect ratio (EAR) calculation for blink detection
Drowsiness detection based on blink frequency and duration
Alerts when drowsiness is detected
Installation
To get started with this project, clone the repository and install the required dependencies.

bash
Copy code
git clone https://github.com/Avadhesh2/Drowsiness-Detection.git
cd Drowsiness-Detection
pip install -r requirements.txt
Usage
After installing the dependencies, you can run the main script to start the drowsiness detection system.

bash
Copy code
python main.py
How It Works
Face Detection: The system uses a pre-trained model to detect faces in the video stream.
Eye Detection: It then locates the eyes within the detected face region.
EAR Calculation: The Eye Aspect Ratio (EAR) is calculated to determine the state of the eyes (open, partially open, or closed).
Drowsiness Detection: If the eyes remain closed for a certain duration, the system triggers an alert indicating potential drowsiness.
Project Structure
bash
Copy code
Drowsiness-Detection/
│
├── main.py                # Main script to run the detection system
├── blink_detector.py      # Module for blink detection logic
├── face_detector.py       # Module for face detection
├── requirements.txt       # List of required dependencies
├── README.md              # Project documentation
└── data/                  # Directory to store any data (e.g., images, videos)
Dependencies
OpenCV
dlib
imutils
numpy
scipy
Results
The system has been tested on various video samples and has shown promising results in detecting drowsiness. Further improvements can be made by incorporating more advanced machine learning models and techniques.
Screenshots
Here are some screenshots demonstrating the functionality of the Drowsiness-Detection system:

Active Face
![image](https://github.com/user-attachments/assets/93f0a85b-9263-4817-af7c-d10b48b29985)

Drowsy Face
![image](https://github.com/user-attachments/assets/db7d5365-ad2a-4294-93ef-566f068fd1ea)

Sleeping Face
![image](https://github.com/user-attachments/assets/f38d179e-2f7f-484b-96f7-d9c038cc3106)
