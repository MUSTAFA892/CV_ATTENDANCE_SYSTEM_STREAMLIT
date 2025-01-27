

---

# Face Recognition Attendance System (Streamlit)

This project facilitates attendance tracking using facial recognition with a simple interface built using Streamlit. The system works in two parts:

1. **Face Attendance Script**: Core logic for recognizing faces and marking attendance.
2. **Streamlit API**: A web-based interface where you can upload an image and pass the roll number to mark attendance.

## Folder Structure

```
/face-attendance
    ├── face_attendance.py       # Core script for face recognition attendance
    ├── utils.py                 # Helper functions for face recognition
    └── requirements.txt         # Required libraries for the project
/api
    ├── app.py                   # Streamlit application
    ├── requirements.txt         # Required libraries for the Streamlit app
    └── README.md                # Documentation for Streamlit app usage
```

---

## Prerequisites

Before running the system, make sure you have the following installed:

- Python 3.x
- Required libraries: `opencv-python`, `face_recognition`, `streamlit`, etc. (listed in the `requirements.txt` file)

To install the required dependencies, run the following command in your terminal:

```bash
pip install -r requirements.txt
```

---

## Face Attendance System (Script)

### How It Works:
The **face attendance script** recognizes faces from an uploaded image and matches them against a database of known faces to mark attendance.

### Running the Script:
To run the face recognition and attendance marking script, execute the following:

```bash
python face_attendance.py
```

This script will process the image of the student, recognize their face, and mark attendance accordingly.

---

## Streamlit Application

The **Streamlit app** provides a user-friendly web interface to upload an image, pass a roll number, and mark the student's attendance based on face recognition.

### How to Use the Streamlit App:

1. **Start the Streamlit app** by running the following command:

    ```bash
    streamlit run api/app.py
    ```

2. Once the app launches in your web browser, follow these steps:

   - **Enter Roll Number**: Type the roll number of the student.
   - **Upload Image**: Upload a clear image of the student for face recognition.
   - The app will process the image, recognize the face, and mark attendance.

---

## Streamlit UI Workflow:

1. **Enter Roll Number**: Input the roll number of the student.
2. **Upload Image**: Upload an image file containing the student's face. The app will process the image for facial recognition.
3. **Attendance Status**: Once the system recognizes the student’s face, the attendance will be marked, and the result will be displayed on the interface.

### Example:

- **Roll Number**: `101`
- **Uploaded Image**: Image of the student with roll number 101

The system will match the face in the uploaded image with the database and mark attendance for the student.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
