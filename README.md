# Verto

An interactive, gesture-controlled 3D hologram. Built with [OpenCV](https://opencv.org/), [Mediapipe](https://developers.google.com/mediapipe), [Websockets](https://socket.io/), [Flask](https://flask.palletsprojects.com/en/3.0.x/), [Next.js](https://nextjs.org/), and various [Poimandres](https://github.com/pmndrs) React packages for Three.js. 

![jarvisgif](https://github.com/ishaan1013/jarvis/assets/69771365/e2c0a4f3-3458-4a7c-8be5-e5847a60743e)



# 🚀 Verto — Gesture-Controlled 3D Hologram Interface
An interactive **real-time gesture-controlled 3D hologram system** built with **OpenCV, MediaPipe, Flask, WebSockets, Next.js, and Three.js**.  
Verto captures hand gestures from a live webcam feed and manipulates 3D models in a hologram-style UI using Pepper’s Ghost effect.

---

## ⭐ Features
- ✋ **Hand-gesture control** using OpenCV + MediaPipe  
- 🧠 Real-time gesture → action mapping  
- 🌐 **Flask WebSocket backend** for low-latency streaming  
- 🎨 **Next.js + Three.js** frontend for interactive 3D rendering  
- 🎤 Optional **voice commands** using WebSpeech API  
- 📱 Works on any screen (with or without hologram prism)  
- 🧊 Supports loading & rotating 3D models  
- ⚡ Smooth, low-latency communication between backend & frontend  

---

## 🛠️ Tech Stack

### Backend
- Python  
- Flask  
- OpenCV  
- MediaPipe  
- WebSockets  

### Frontend
- Next.js  
- React  
- Three.js  
- WebSpeech API  

---

## 📦 Project Structure
```
Verto/
│
├── backend/             # Python backend with CV + gesture-tracking
│   ├── camera.py
│   ├── gestures.py
│   ├── server.py
│   └── ...
│
├── frontend/            # Next.js 3D UI
│   ├── components/
│   ├── pages/
│   ├── public/
│   └── ...
│
├── utils/               # Shared utilities
│
├── calibrate-camera/    # Calibration tools for gesture accuracy
│
└── README.md
```

---

# 🚀 Getting Started

## 1️⃣ Clone the Repository
```bash
git clone https://github.com/Jyothireddy-pula/Verto
cd Verto
```

---

# 🔧 Backend Setup

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Set Up Camera
Position the webcam **facing upward**, slightly below your screen.

### 4️⃣ Run Backend Server
```bash
cd backend
flask run
```
Runs at:
```
http://localhost:8000
```

---

# 🎨 Frontend Setup

### 5️⃣ Install Dependencies
```bash
cd frontend
npm install
```

### 6️⃣ Start Development Server
```bash
npm run dev
```

Runs at:
```
http://localhost:3000
```

---

# 🧪 How It Works

### 1. Gesture Capture  
OpenCV + MediaPipe detect:  
- swipe left/right  
- open palm  
- fist  
- pinch  

### 2. Real-Time Communication  
Flask WebSockets → push gesture events instantly.

### 3. 3D Rendering  
Next.js + Three.js update the model based on gestures.

---

# 🪩 Optional: Build a Pepper’s Ghost Hologram
Use transparent acrylic sheets placed at **45°**, enabling a pseudo-hologram effect.

---

# 🎤 Voice Commands (Optional)
Supports commands like:
- “Rotate left”
- “Zoom in”
- “Change object”

---

# 🧩 Future Improvements
- Custom ML gesture training  
- Multi-gesture sequences  
- Model library switcher  
- Mobile-browser support  

---

# 📸 Demo
![jarvisgif](https://github.com/ishaan1013/jarvis/assets/69771365/e2c0a4f3-3458-4a7c-8be5-e5847a60743e)

---

# 🤝 Contributing
Pull requests welcome. Open an issue to discuss major changes.

---

# 📄 License
MIT License.

## Running Locally.

It works just fine on any regular screen (without the hologram effect, of course). But feel free to build a Pepper's Ghost hologram if you'd like. 

### Cloning the repository the local machine.

```bash
git clone https://github.com/Jyothireddy-pula/Verto
```

### Backend setup

- Set up a webcam facing upwards, in front of your screen and a little bit below.
- Ensure OpenCV recognizes your webcam in `backend/camera.py`
- 🐍 Run the flask app, which will be available at `http://localhost:8000`.

```bash
flask run
```

### Running the frontend app
```bash
npm install
```

Then, run the application in the command line and it will be available at `http://localhost:3000`.

```bash
npm run dev
```

#### Notes.
- Viewing and manipulating 3D models can be resource-intensive.
- Voice control uses the WebSpeechAPI which currently works best on Chrome, Microsoft Edge, or Safari 14.1
