# Oil-Quality-Classification-System


This project is an AI powered oil quality detection system that can classify oil as either clean or dirty using a trained learning model, and also displays the result on an LCD that's controlled with an Arduino. A camera captures images of oil samples, a MobileNetV2 model then does the classification, and the prediction is sent using serial communication to an Arduino Uno, which then updates on the LCD display.


Materials used - 

- Arduino Uno
- 16x2 LCD (HD44780 compatible)
- USB Camera
- Jetson / Linux-based system
- 10kΩ potentiometer or resistor for LCD contrast


Software/libraries I used -
- Python 3
- PyTorch
- Torchvision
- OpenCV
- PIL
- Arduino IDE
- LiquidCrystal library


Summary:

A MobileNetV2 model was trained on labeled images of clean and dirty oil using a Jetson Orin Nano
   →

The camera is processed and classified every few frames to keep stable predictions instead of jumping around in a couple of miliseconds
   →

The predictions are then sent over USB serial to the Arduino.
   →

The Arduino then updates the LCD to display the oil condition.


I plan to

- Display a confidence percentage of the AI on the LCD
- Expand dataset for better accuracy
- Deploy it as a standalone embedded system that can control a pump to flick on a skimmer



Marcos Paulino, 
Engineering Student
