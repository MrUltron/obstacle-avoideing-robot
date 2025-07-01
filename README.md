# 🚗 Object Detection Car using Arduino and Ultrasonic Sensor

This project demonstrates a simple autonomous obstacle-avoiding car using Arduino, an HC-SR04 ultrasonic sensor, and a motor driver. The car moves forward when no obstacle is detected and stops when it detects an obstacle within a certain range.

## 📦 Components Required
- Arduino Uno (or compatible)
- HC-SR04 Ultrasonic Sensor
- L298N Motor Driver Module
- 2 x DC Motors with Wheels
- Chassis for the car
- Jumper Wires
- Power Source (9V battery or LiPo pack)

## 🔌 Circuit Connections

### Ultrasonic Sensor (HC-SR04)
- VCC → 5V (Arduino)
- GND → GND (Arduino)
- TRIG → D9 (Arduino)
- ECHO → D10 (Arduino)

### Motor Driver (L298N)
- IN1 → D2
- IN2 → D3
- IN3 → D4
- IN4 → D5
- VCC → Battery +
- GND → Battery - and Arduino GND

### Motors
- Connect to OUT1, OUT2 (Motor A) and OUT3, OUT4 (Motor B) of the L298N

## 🧠 How It Works
1. The ultrasonic sensor continuously measures the distance to obstacles.
2. If an object is detected within 20 cm, the car stops.
3. If the path is clear, the car moves forward.

## 🖥️ Arduino Code
See the `object_detection_car.ino` file in this repository.

## 🧪 Testing
- Upload the code to your Arduino using the Arduino IDE.
- Place the car on a smooth surface.
- Power it using a battery.
- Observe the obstacle detection in real-time.

## 🛠️ Future Improvements
- Add reverse or turning logic when obstacle is detected
- Use servo motor for sensor rotation
- Integrate IR sensors or AI for smarter detection

## 📷 Preview
*(Add images or video links of the working project here)*

## 📄 License
This project is open-source and available under the MIT License.

---
Happy Building! 🚀
