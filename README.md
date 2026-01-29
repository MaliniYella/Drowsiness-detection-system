
# Drowsiness Detection System

#Overview

The Drowsiness Detection System is a real-time computer vision application designed to monitor eye movements and detect signs of fatigue or drowsiness. Using the Eye Aspect Ratio (EAR) method with OpenCV and dlib, the system alerts users when signs of drowsiness are detected, making it suitable for applications like driver safety, workplace monitoring, or study environments.

#Features

* Real-time monitoring of eye movements.
* Detects drowsiness using Eye Aspect Ratio (EAR).
* Triggers alerts (visual or audio) when the user shows signs of fatigue.
* Lightweight and fast, suitable for webcam-based applications.

#Technology Stack

* Programming Language: Python
* Libraries & Tools:

  * OpenCV (Computer vision)
  * dlib (Facial landmark detection)
  * numpy (Numerical computations)
  * playsound or other audio library for alerts

---

#Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YourUsername/Drowsiness-Detection-System.git
   cd Drowsiness-Detection-System
   ```

2. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate   # For Linux/Mac
   venv\Scripts\activate      # For Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Download required models:
   Ensure `shape_predictor_68_face_landmarks.dat` is in the `assets/` folder (used by dlib).

---

#Usage

1. Run the main script:

   ```bash
   python drowsiness_detection.py
   ```
2. The webcam feed will open.
3. The system will monitor the eyes in real-time and trigger an alert if drowsiness is detected.

#How it Works

1. The face is detected using dlib’s pre-trained face detector.
2. Eye regions are identified using facial landmarks.
3. The Eye Aspect Ratio (EAR) is calculated to determine if eyes are closed.
4. If eyes remain closed for a predefined number of frames, the system triggers an alert.

---

#Future Improvements

* Integrate with a mobile or in-car device for real-world usage.
* Add yawning detection for better accuracy.
* Implement machine learning models for adaptive drowsiness prediction.

