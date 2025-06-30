# 🤖 Hand Gesture Controlled Servo Motor

This project lets you control a **servo motor** using your **hand gestures** detected in real-time via your webcam. It combines **computer vision (Python + MediaPipe)** with **Arduino-based motor control**, allowing touchless operation using just your hand movements.

---

## 🧠 Project Description

The system detects whether your hand is **open or closed** using the webcam. Based on the gesture:

* 🖐️ **Open Hand** → A signal `'1'` is sent to Arduino → Servo rotates to **90°**
* ✊ **Closed Hand** → A signal `'0'` is sent to Arduino → Servo rotates to **0°**

This interaction happens through **serial communication** between your PC and Arduino, enabling gesture-based control of physical hardware.

---

## 🚀 Quick Start

### 📥 Clone the Repository

```bash
git clone https://github.com/Asish-SGeorge/hand-gesture-servo-control.git
cd hand-gesture-servo-control
```


---

## 🖥️ What You Need

### Hardware

* Arduino UNO (or compatible)
* Servo motor (e.g., SG90)
* Jumper wires
* USB cable
* Computer with webcam
* (Optional) External power for servo (recommended)

### Software

* Python 3.10
* Arduino IDE

### Python Libraries

Install required libraries with:

```bash
pip install opencv-python mediapipe pyserial
```

---

## ⚙️ How It Works

1. **Python script** uses your webcam and MediaPipe to detect your hand in real-time.
2. It checks if fingers are extended or folded to classify the gesture.
3. Sends `'1'` for open hand and `'0'` for closed hand to Arduino via USB.
4. **Arduino** reads the incoming value and adjusts the servo angle accordingly.

---

## 🎯 Applications

* Gesture-based switch
* Smart home control
* Robotics education
* Touchless control systems
* Assistive technology interfaces

---

## 🎥 Demo

> *Insert a GIF or YouTube video link here showing the working project.*

---

## 💡 Future Improvements

* Detect more complex gestures (e.g., thumbs-up, peace sign).
* Control multiple servo motors.
* Wireless communication using Bluetooth or Wi-Fi.
* Display feedback on an LCD or in a GUI.
* Integrate with IoT platforms (like Blynk or Firebase).

---

## 📜 License

This project is licensed under the **MIT License**. Feel free to use, modify, and share it.

---

Let me know if you'd like a downloadable `.md` file version or help preparing visuals for the demo section!
