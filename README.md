# 🎯 Object Tracking System (Pan-Tilt) using Computer Vision

## 📌 Overview
This project presents a real-time object tracking system based on a **pan-tilt platform (2 DOF)**.  
The system uses a camera and a laser pointer mounted on a movable structure driven by stepper motors.

Object detection and tracking are implemented using computer vision methods (**OpenCV + YOLO**), while control is based on a predictive approach to reduce delay and improve tracking accuracy.

<img width="436" height="495" alt="image" src="https://github.com/user-attachments/assets/0d5542f8-10fc-4622-b5b3-cfccec90ea6a" />

---

## 🎯 Objectives
- Design and build the mechanical structure (2 DOF)
- Selection of electronics and microcontroller
- Implementation of object detection and tracking algorithms
- Development of a control system ensuring smooth and precise tracking

---

## 🛠️ Tools & Technologies
- **Python** (OpenCV, YOLO, NumPy)
- **MATLAB / Simulink**
- **STM32 (STM32CubeIDE)**
- **Arduino IDE (C++)**
- **Kalman Filter**
- Stepper motor control

---

## 🧠 My Contributions
- Developed a mathematical model of the system
- Designed and built the mechanical structure
- Implemented stepper motor control
- Developed the vision algorithm (detection + tracking)
- Implemented a Kalman filter for position estimation
- Designed and implemented a predictive controller

---

## ⚙️ System Architecture
Control system diagram:

<img width="1576" height="891" alt="image" src="https://github.com/user-attachments/assets/bf109700-8189-4302-a185-9b1dec36c438" />

---

## 📐 Predictive Controller Model (Simulink)
The controller estimates the future tracking error based on current object and platform position.  
This predicted error is then fed into a PID controller, which controls motor velocity.

More details available upon request.

<img width="1706" height="639" alt="image" src="https://github.com/user-attachments/assets/2ab24032-dfab-4c39-b323-b9f10e0baa82" />

---

## 📊 Results

### Simulation Results (Predictive Control, Simulink)
Validation of predictive controller performance under simulated disturbances.  
The controller performs effectively and maintains stable tracking.

<img width="1919" height="923" alt="image" src="https://github.com/user-attachments/assets/859c2298-bada-4fa8-af31-b4bce74b52ea" />

---

## 🎥 Video Demonstration

### Object Tracking (earlier predictive control version)
The system detects and tracks objects with satisfactory accuracy.  
Currently working on improving control performance by implementing an enhanced predictive controller.

[![Demo](https://img.youtube.com/vi/rupabkPK9xA/0.jpg)](https://youtu.be/rupabkPK9xA)

---

## 📉 Limitations
- Limited camera frame rate
- Mechanical imperfections affecting precision
- Delays caused by image processing

---

## 🚀 Future Improvements
- Use of a high-speed global shutter camera
- Improved mechanical rigidity and calibration
- Further tuning of the predictive control algorithm
- Optimization of vision code for performance
- Integration of absolute encoders

---

## 📬 Contact
Feel free to reach out if you have any questions or would like to discuss the project.
