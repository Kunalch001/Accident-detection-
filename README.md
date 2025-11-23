🚗 Accident Detection System using ESP32, MPU6050 & Alert Messaging

A smart accident-detection prototype built using ESP32, MPU6050 accelerometer/gyroscope sensor, I2C LCD, buzzer, LED, and push button. This system detects unusual tilt/impact and sends an automatic emergency alert if the driver does not respond within 10 seconds.

📌 Project Overview

This project aims to provide a low-cost and efficient accident detection system for vehicles.
The system continuously monitors the tilt angle of the vehicle using the MPU6050.
When abnormal tilt exceeds a set threshold:

The buzzer alerts for 10 seconds.

The driver can press the push button to cancel the alert in case of a false alarm.

If not cancelled within the time limit, the ESP32 sends an emergency notification to a predefined contact number (via a cloud API / messaging service).

The LCD displays real-time status and warnings.

The LED acts as the engine indicator during operation.

🛠️ Components Used

ESP32 Development Board

MPU6050 (Accelerometer + Gyroscope)

I2C 16x2 LCD Display

Active Buzzer

LED (Engine Indicator)

Push Button

Jumper wires

Breadboard

🔧 Working Principle

Sensor Monitoring:

The MPU6050 continuously reads acceleration and gyro data.

Tilt angle or sudden impact is calculated.

Threshold Detection:

If tilt angle > predefined threshold → system enters Alert State.

Alert Mechanism:

Buzzer beeps for 10 seconds.

LCD shows "Possible Accident!".

Driver must press the button to stop it.

Emergency Messaging:

If driver fails to react within 10 seconds, the ESP32 automatically sends an alert message to the emergency contact.

Message includes vehicle status.

📟 LCD Display Messages

System Ready

Monitoring...

Accident Detected!

Sending Alert...

🚨 Features

Real-time tilt & impact monitoring

Automatic accident detection

False alert cancellation using a push button

Emergency SMS/notification system

Low-cost hardware design
