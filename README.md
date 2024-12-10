This project is an Attendance Management System that uses Face Recognition powered by OpenCV. The system captures face data, trains a model, and uses the trained data to recognize and mark attendance automatically.
FEATURES:
Face Data Capture: Collect and save face data of employees/students.
Face Recognition: Detect and recognize faces in real time using OpenCV.
Attendance Recording: Automatically mark attendance in a database or a CSV file.
Simple User Interface: Easy-to-use interface for system administrators.
Secure: Prevents unauthorized users from being marked as present.

REQUIREMENTS:
Before running this project, ensure you have the following installed:
Python 3.x
OpenCV (cv2)
NumPy
pandas
dlib (optional for advanced face recognition)
SQLite3 (or any other database of choice)
Install the dependencies using:
pip install opencv-python numpy pandas dlib

HOW IT WORKS :
Face Data Collection:
The system captures face images and stores them in a dataset folder.
Each image is labeled with a unique identifier (e.g., employee ID or student ID).
Training the Model:
OpenCV's face_recognition module processes the images to create a recognition model.
Real-Time Recognition:
The webcam captures real-time video.
Faces are detected, matched against the trained model, and verified.
Attendance Recording:
If a face is recognized, the system logs the user's attendance in the database or CSV file with a timestamp.

Setup Instructions
Clone the Repository:
git clone https://github.com/yourusername/attendance-face-recognition.git
cd attendance-face-recognition
Prepare the Dataset:
Place all face images in the dataset/ folder.
Each person's images should be stored in a separate folder named after their unique ID.
Run the Training Script:
python train_model.py
Start the Attendance System:
python attendance_system.py
