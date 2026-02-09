# Oil-Quality-Classification-System

Overview:
This project is an AI powered oil quality detection system that classifies oil as either clean or dirty using a trained learning model and displays the result on an Arduino controlled LCD. A camera captures images of oil samples, a MobileNetV2 model performs classification, and the prediction is sent via serial communication to an Arduino Uno, which updates the LCD display.


Hardware Used:

- Arduino Uno
- 16x2 LCD (HD44780 compatible)
- USB Camera
- Jetson / Linux-based system
- 10kΩ potentiometer or resistor for LCD contrast


Software and Libraries:
- Python 3
- PyTorch
- Torchvision
- OpenCV
- PIL
- Arduino IDE
- LiquidCrystal library


How It Works:

A MobileNetV2 model was trained on labeled images of clean and dirty oil.
   →
Live Prediction:
The camera feed is processed in real time and classified every few frames to ensure stable predictions.
   →
Arduino Communication:
Predictions are sent over USB serial to the Arduino.
   →
LCD Output:
The Arduino updates the LCD to display the oil condition.


Future Work Planned:

- Display confidence percentage on LCD
- Add automatic image capture
- Expand dataset for better accuracy
- Deploy as a standalone embedded system



Marcos Paulino
Engineering Student
