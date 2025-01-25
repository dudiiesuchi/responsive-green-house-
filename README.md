
# Responsive Greenhouse Project Documentation
# Introduction
The Responsive Greenhouse is an automated system designed to monitor and control environmental factors for optimal plant growth. The system incorporates sensors, actuators, and an Arduino microcontroller to regulate temperature, humidity, and lighting conditions while providing real-time feedback on an LCD display.
![image](https://github.com/user-attachments/assets/ad93c558-5278-45e9-905c-048d9d170d48


# Components Used
Arduino Uno (U1):

Acts as the central microcontroller for processing inputs and controlling outputs.
LCD 16x2 Display (U2):

Displays real-time information like temperature, humidity, and system status.
Potentiometer (R_POT):

Used to adjust the contrast of the LCD.
DHT Sensor (SEN1):

Measures temperature and humidity in the greenhouse.
Servo Motor (SERVO1):

Controls ventilation flaps or shading mechanisms.
DC Motor (M1):

Operates a fan for air circulation or temperature control.
Ultrasonic Sensor (PING1):

Detects water levels in the reservoir or monitors plant growth.
Resistor (R1):

Provides the necessary resistance for proper operation of the circuit.
Circuit Overview
Power Supply:
The system operates on a 5V power source, with connections made to components via the Arduino's voltage and ground pins.
Connections:
LCD Display:

Connected to digital pins D2–D7 for data and control signals.
Contrast controlled via a potentiometer.
DHT Sensor:

Connected to a digital pin for temperature and humidity readings.
Servo Motor:

Signal pin connected to a digital output pin to control ventilation.
DC Motor:

Controlled via a driver circuit connected to a digital pin.
Ultrasonic Sensor:

Trigger and Echo pins connected to specific digital pins for distance measurement.
Functionality
# Monitoring:

The DHT sensor continuously monitors the temperature and humidity inside the greenhouse.
Ultrasonic sensor checks the water level or plant height.
Control Mechanisms:

If temperature exceeds a threshold, the servo motor opens ventilation flaps, and the DC motor activates a fan.
Humidity levels are adjusted through automated systems (e.g., misters or fans).
Feedback:

Real-time data is displayed on the LCD screen.
Alerts are triggered if parameters exceed safe thresholds.
# Code Logic
Initialize components and libraries.
Read sensor data periodically.
Compare readings against predefined thresholds.
Trigger actuators (e.g., motors) as needed.
Update the LCD display with real-time readings and system status.
# Advantages
1. Ensures optimal plant growth conditions.
2. Minimizes human intervention.
3. Energy-efficient operation.
4. Provides real-time feedback and alerting.
# Future Improvements
1. Integration with IoT for remote monitoring and control.
2. Addition of a pH sensor to monitor soil quality.
3. Solar power integration for energy independence.
4. Implementation of advanced AI algorithms for predictive analysis.
