# Facial Recognition Attendance Tracker

This project is a facial recognition system that automates attendance tracking by detecting and identifying faces in a group photo. Built using Python, InsightFace, OpenCV, and SQLite, the system matches detected faces against a student database and logs attendance automatically.

## 👩‍💻 Project Overview

This attendance tracker identifies individuals from a group image using facial embeddings. The prototype was built using fictional Harry Potter characters to simulate a student database and test recognition capabilities. Faces are detected, matched, and attendance is recorded in a local SQLite database.

## 🔧 Tools & Technologies
- **Python**
- **OpenCV (cv2)** – image processing
- **InsightFace** – face detection and embedding extraction
- **SQLite** – local student database management
- **Google Colab** – cloud-based execution environment

## 🧠 Key Features
- Constructed a student database (`attendance.db`) with ID, name, and photo path
- Extracted facial embeddings and stored unique vectors for each student
- Detected faces from a group image and matched them using cosine similarity
- Automated attendance logging and visually highlighted recognized faces with bounding boxes

## 📊 Challenges & Solutions
- **Face Detection Failures**: Resolved by adjusting face detection parameters and using better image normalization
- **False Matches**: Improved matching accuracy by fine-tuning the cosine similarity threshold
- **Database Integration**: Ensured smooth retrieval and insertion of records through tested SQL queries

## 📷 Visual Enhancements
Faces detected in the group image are shown with bounding boxes to allow for easier debugging and visual confirmation. Duplicate detections (e.g., multiple “Harry” appearances) were noted and highlighted during testing.

## ✅ Outcome
The system was able to:
- Successfully identify 5 unique individuals from a complex group image
- Handle duplicate appearances and partial occlusions
- Record attendance in a structured and automated format

## 📂 File Structure
AttendanceTracker/
├── hpgrouppic.jpg
├── images/
│ ├── harry.jpg
│ ├── hermione.jpg
│ ├── ron.jpg
│ ├── draco.jpg
│ └── neville.jpg
├── attendance.db
├── attendance_tracker.ipynb
└── README.md

## 🚀 Future Improvements
- Real-time video stream detection
- Integration with Google Sheets or cloud-based attendance records
- Multi-classroom scalability with user interface

## 🧵 Author
Sophia Duran  
[GitHub](https://github.com/sophia-duran) | [LinkedIn](https://www.linkedin.com/in/sophia-duran)

---

*This project was completed as part of the Advanced Business Analytics coursework at Syracuse University.*
