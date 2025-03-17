# Drowsiness Detection System

## Introduction
This project is a **real-time drowsiness detection system** that uses **Dlib** for facial landmark detection and **Scipy** to compute the Eye Aspect Ratio (EAR). The system continuously monitors the user's eye state and triggers an alert if drowsiness is detected.

## Features
- **Real-time Face and Eye Detection** using Dlib
- **Drowsiness Detection** using the Eye Aspect Ratio (EAR)
- **Automatic Alert System** when drowsiness is detected
- Works with **webcam feed**

## Requirements
Before running the project, install the following dependencies:

```bash
pip install dlib opencv-python numpy scipy imutils
```

Also, download the **Dlib's pre-trained model** for facial landmark detection:
- [Download here](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2)
- Extract and place `shape_predictor_68_face_landmarks.dat` in the project folder

## How It Works
1. The webcam captures the video stream.
2. **Dlib's face detector** detects faces in the frame.
3. **Facial landmarks** are extracted to locate the eyes.
4. The **Eye Aspect Ratio (EAR)** is computed:
   - If EAR < 0.25 for **20 consecutive frames**, an alert is triggered.
5. Eye landmarks are drawn on the frame.
6. The user is notified of drowsiness if detected.

## Usage
To run the project, execute the following command:

```bash
python detect.py
```

Press `q` to exit the program.

## Future Enhancements
- Add **sound alerts** when drowsiness is detected
- Improve detection using **deep learning models**
- Implement **mobile compatibility**
- Enhance accuracy with **infrared cameras** for night detection

## Contributing
Feel free to contribute to this project by improving the detection system or adding new features.

## License
This project is open-source and available under the **MIT License**.

---

**Author:** Rudranarayan Sahu  
**GitHub:** [rudranarayan-01](https://github.com/rudranarayan-01)  
**LinkedIn:** [rudranarayan-sahu](https://www.linkedin.com/in/rudranarayan-sahu-b7b9a6244/)  

