# Real-Time-Sign-Language-Tranlation
A comprehensive web-based application that translates sign language gestures into text in real-time using computer vision and deep learning techniques.
✨ Features

Real-time Translation: Live webcam feed processing for instant sign language recognition
Web Interface: User-friendly Flask-based web application
User Management: Complete authentication system with signup, login, and profile management
Multiple Recognition: Supports 20+ common sign language phrases and words
High Accuracy: Custom YOLOv5 model trained for sign language detection
Responsive Design: Modern web interface with real-time video streaming
Virtual Camera Support: Integration with virtual camera for enhanced functionality

🎯 Supported Signs
The system currently recognizes the following sign language expressions:
- Hello          • Thank you      • I love you     • Yes
- Please         • Sorry          • Bye            • No
- How are you    • I am fine      • Help           • Bathroom
- What           • Stop           • Friend         • Which
- Who            • Me             • You            • Live Long
🛠️ Technology Stack

Backend: Flask (Python)
Computer Vision: OpenCV, MediaPipe
Machine Learning: PyTorch, YOLOv5
Database: MongoDB
Frontend: HTML, CSS, JavaScript
Authentication: Custom user management system
Email Service: SMTP integration for password recovery

🚀 Getting Started
Prerequisites

Python 3.8 or higher
Webcam/Camera device
MongoDB (for user management)
Git

Installation

Clone the repository
bashgit clone https://github.com/Jayadeep2004/Real-Time-Sign-Language-Translation.git
cd Real-Time-Sign-Language-Translation

Create a virtual environment
bashpython -m venv sign_lang_env
source sign_lang_env/bin/activate  # On Windows: sign_lang_env\Scripts\activate

Install dependencies
bashpip install -r requirements.txt

Download the trained model

Place your trained YOLOv5 model weights in signLang/weights/best.pt
Or train your own model using the provided configuration


Set up MongoDB

Install MongoDB and ensure it's running
Update database connection settings in backend/mongo.py


Run the application
bashpython app.py

Access the application

Open your web browser and navigate to http://localhost:5000

📱 Usage
For Users

Sign Up: Create a new account with your details
Login: Access your personalized dashboard
Start Translation: Navigate to the translation page
Perform Signs: Make sign language gestures in front of your webcam
View Results: See real-time translation results on screen

For Developers

Training New Models: Use the configuration in config.py to train custom models
Adding New Signs: Extend the dataset list in config.py
Virtual Camera: Use SignCam.py for virtual camera integration

🏗️ Project Structure
Real-Time-Sign-Language-Translation/
├── app.py                 # Main Flask application
├── body.py               # Core computer vision processing
├── SignCam.py            # Virtual camera integration
├── config.py             # Configuration and dataset settings
├── requirements.txt      # Python dependencies
├── backend/
│   ├── mongo.py          # Database operations
│   └── fpwd.py           # Password recovery functionality
├── templates/            # HTML templates
├── static/               # CSS, JS, and static assets
├── signLang/
│   └── weights/          # Trained model weights
└── Data/
    └── images/           # Training dataset
