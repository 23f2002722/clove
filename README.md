# clove

A Flask-based face recognition web application that allows users to upload face images and identify people in real-time using webcam-based face recognition.

---

## Features

* Upload and store face images
* Multiple image upload support
* Real-time face detection using webcam
* Face recognition using stored images
* Dynamic image gallery display
* Secure file handling with Flask

---

## Tech Stack

* Python
* Flask
* OpenCV
* face_recognition
* dlib
* NumPy
* Pillow

---

## Project Structure

```bash
Clove/
│
├── app.py
├── server.py
├── gray.py
├── requirements.txt
│
├── static/
│   └── images/
│
└── templates/
    └── index.html
```

---

## Installation

```bash
git clone https://github.com/your-username/Clove.git
cd Clove
```

Create virtual environment:

```bash
python -m venv venv
```

Activate environment:

### Windows

```bash
venv\Scripts\activate
```

### Linux/macOS

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Run the Application

Start Flask app:

```bash
python app.py
```

Run face recognition server:

```bash
python server.py
```

---

## How It Works

1. Upload face images through the Flask web interface.
2. Images are stored inside `static/images/`.
3. `server.py` reads uploaded images and generates face encodings.
4. Webcam feed is processed in real-time.
5. Detected faces are matched against stored encodings.
6. Recognized faces are labeled with corresponding names.

---

## Supported Formats

* JPG
* JPEG
* PNG
* GIF

---

## License

Open-source project for educational and learning purposes.
