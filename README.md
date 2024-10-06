FaceTrack Smart Attendance System
Overview

FaceTrack Smart Attendance System is an advanced facial recognition-based attendance management system. It uses computer vision technology to capture, recognize, and record attendance automatically, offering an efficient and automated solution for tracking attendance in educational institutions and workplaces.
Features

    Face Detection: Detects faces in real-time using the webcam and OpenCV.
    Face Recognition: Identifies and recognizes individuals using pre-trained models.
    Automated Attendance Marking: Automatically marks attendance in a CSV file.
    Model Training: Easily train the system with new faces using LBPH (Local Binary Patterns Histogram).
    Live Tracking: Continuously tracks individuals and matches them with the trained model for real-time attendance.
    User-friendly GUI: Simple and easy-to-use graphical user interface (GUI) for users.

Installation

    Clone the repository:

    bash

git clone https://github.com/Ashwaninikhil/faceTrack-smart-attendence-system.git

Navigate to the project directory:

bash

cd faceTrack-smart-attendence-system

Install the required dependencies:

bash

pip install -r requirements.txt

Download the necessary face detection models (e.g., Haar Cascade):

    Haar Cascade Frontal Face XML

Run the project:

bash

    python faceTrack.py

Usage
Steps to Use the Application:

    Enter Details: Provide your College ID and Name in the respective fields.
    Capture Images: Click the IMAGE CAPTURE BUTTON to capture multiple images of your face.
    Train Model: Click the MODEL TRAINING BUTTON to train the facial recognition model.
    Track Attendance: Once the model is trained, click the ATTENDANCE MARKING BUTTON to start the real-time face recognition and attendance marking.
    Exit: Use the QUIT button to close the application.

Files Generated:

    Training Images: All captured images are stored in the TrainingImage folder.
    Trained Model: The trained LBPH face recognizer is saved as Trainner.yml in the TrainingImageLabel folder.
    Attendance Records: Attendance data is saved in a CSV file with a timestamp under the Attendance folder.

Requirements

    Python 3.x
    OpenCV
    NumPy
    Pandas
    Tkinter
    Pillow (PIL)

Install the dependencies via requirements.txt:

bash

pip install -r requirements.txt

Project Structure

bash

.
├── Attendance/              # Stores attendance records in CSV format
├── ImagesUnknown/           # Stores unrecognized faces
├── StudentDetails/          # CSV file with student details (ID and Name)
├── TrainingImage/           # Stores captured training images
├── TrainingImageLabel/      # Contains the trained face recognition model
├── haarcascade_frontalface_default.xml  # Haar cascade classifier for face detection
├── faceTrack.py             # Main application script
├── requirements.txt         # Project dependencies
└── README.md                # This README file

Future Enhancements

    Implementing email notifications for attendance reports.
    Adding multi-camera support for larger environments.
    Improving the UI/UX with more advanced design features.
    Integrating with other databases like SQL for scalable data storage.

Contributing

If you wish to contribute to this project, feel free to submit a pull request. We welcome any suggestions for improvements.
License

This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgements

    OpenCV for providing the robust face detection and recognition library.
    Python community for developing powerful libraries such as NumPy and Pandas.
    Special thanks to IKGPTU for inspiring this project.

