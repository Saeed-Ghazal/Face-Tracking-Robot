# Face-Tracking Robot

A face-tracking robotic system built using **Arduino UNO**, **Pan–Tilt mechanism**, **LED indicators**, **solar-powered battery**, and a **webcam**.  
The robot uses **Computer Vision** to detect human faces and automatically move the camera to center the face in the frame.

---

## 📸 System Preview

<img 
  src="https://github.com/Saeed-Ghazal/Face-Tracking-Robot/blob/main/face_tracking_camera-master/Image%20Nov%2021,%202025,%2003_02_50%20PM.png?raw=true" 
  alt="Face Tracking Camera" 
  style="width: 350px; border-radius: 10px;" 
/>

---

## 🧠 How It Works

1. The webcam streams live video to a computer running a **Computer Vision face detection algorithm**.  
2. The software calculates the face position and sends control signals to the Arduino.  
3. Two servos control the **Pan** and **Tilt** angles to keep the face centered.  
4. LEDs indicate the detection status:
   - 🔴 **Red** → No face detected  
   - 🟡 **Yellow** → Face detected but not centered  
   - 🟢 **Green** → Face centered  
5. A laser pointer indicates the camera's exact aim direction.  
6. A solar panel charges the battery, which powers the entire robot.

---

## 📱 Manual & Automatic Modes

The system includes a simple control interface:

- **Automatic Mode:**  
  Camera moves automatically to track the detected face.

- **Manual Mode:**  
  User can control camera movement with a mouse or keyboard input.

---

## 🔧 Hardware Components

| Component | Description |
|----------|-------------|
| Arduino UNO | Main microcontroller handling servo + LED control |
| 2× Servo Motors (SG90/MG90S) | Pan (horizontal) and Tilt (vertical) movement |
| Webcam | Captures live video for face detection |
| Red, Yellow, Green LEDs | Detection status indicators |
| Laser Module | Shows the exact targeting direction of the camera |
| Solar Panel | Recharges the battery |
| Rechargeable Battery | Powers the Arduino and servos |
| Pan-Tilt Bracket | Mounts the camera and servos |

---

## 🖥️ Software Features

- Real-time face detection  
- Pan–Tilt automatic servo stabilization  
- LED feedback system
- Automatic Tracking Mode: The camera automatically tracks the detected face and aligns it to the center of the screen.
- Manual camera control via app  
- Adjustable sensitivity and tracking speed  
