#Pan-Tilt Face Tracking Bot 🤖📷
This project integrates an ESP32-CAM module with Python to perform real-time face tracking. A pan-tilt mechanism moves the camera based on detected faces using computer vision techniques. The system also provides a Flask web interface for live video streaming and optional chatbot interaction.

🚀 Features
🎯 Real-time face detection using OpenCV

🔄 Servo-controlled camera movement (pan & tilt)

🌐 Flask-based web interface for live video feed & control

🔌 MicroPython on ESP32-CAM for servo control

💬 Optional AIML chatbot for real-time communication

🛠️ Tech Stack
Component	Technology Used
Face Detection	OpenCV (Python)
Microcontroller	ESP32-CAM + MicroPython
Servo Control	GPIO (MicroPython PWM)
Web Interface	Flask (Python)
Video Streaming	MJPEG (OpenCV + Flask)
Chatbot (optional)	AIML + Flask (chat endpoint)

🧰 Requirements
Python 3.8+

OpenCV

Flask

PySerial (for serial communication)

ESP32-CAM board

2x Servo motors (pan & tilt)

MicroPython flashed on ESP32-CAM

Modern web browser (for Flask interface)

📸 How It Works
ESP32-CAM captures live video.

Python script (OpenCV) detects faces in real-time.

Detected face coordinates control servo motors for pan & tilt movement.

Flask interface streams live video and provides basic control.

📂 Repository Structure
graphql
Copy
Edit
PanTilt-FaceTracking/
│
├── esp32/           # MicroPython scripts for ESP32-CAM
├── python/          # Python scripts for face detection & servo control
├── templates/       # Flask web interface HTML files
├── static/          # CSS/JS for Flask interface
├── README.md        # Project documentation
└── requirements.txt # Python dependencies
▶️ Usage
Flash MicroPython to your ESP32-CAM.

Upload the ESP32 servo control script to the board.

Install Python dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the face tracking script:

bash
Copy
Edit
python face_tracking.py
Open the Flask interface in your browser to view the live feed.
