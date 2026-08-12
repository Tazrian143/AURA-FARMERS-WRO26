# AURA (Antiquity Universal Restoration Automation)

![AURA Project Image](images/car.jpg)

## Project Overview
AURA is an intelligent robotic cleaning system designed to protect delicate historical artifacts in museums and galleries. It uses a compact vacuum mounted on a robotic arm to remove dust without physically touching the object. The system is equipped with distance and dust sensors to ensure safe, precise, and energy-efficient operation.

## Team Information
**Team Name:** AURA FARMERS  
**Category:** Future Innovators  
**Group:** Junior  
**Country:** Bangladesh  

**Members:**
- Md. Mohafizur Rahman
- Md. Nabhan Nubaid
- Kazi Tasfia Alam

## Problem Statement
Artifacts in museums and galleries gradually accumulate dust, which can cause chemical degradation and physical damage. Traditional cleaning methods are often slow, labor-intensive, and risky for fragile objects.

## Solution
AURA provides a non-contact cleaning solution that detects dust and maintains a safe distance from artifacts. This reduces the risk of damage, lowers manual effort, and improves cleaning efficiency.

## Key Components
| Component | Function | How it Works | Price Range | Image |
|---|---|---|---|---|
| ESP32 microcontroller | Main control unit | Runs the robot firmware, reads sensors, and controls motors and actuators | ৳450 – ৳550 | ![ESP32](images/microcontroller.jpg) |
| VL5303X Time-of-Flight Sensor | Distance sensing | Measures distance to the artifact using infrared light and returns precise range data | ৳550 – ৳650 | ![VL5303X](images/arm.jpg) |
| GP2Y1014AU0F Dust Sensor | Dust detection | Detects airborne dust particles using infrared light scattering and triggers cleaning when dust is present | ৳700 – ৳850 | ![Dust Sensor](images/dust-sensor.jpg) |
| 5015 Blower Fan | Suction source | Creates airflow through the nozzle and filter path to remove dust from the artifact area | ৳180 – ৳220 | ![Blower Fan](images/fan.jpg) |
| L298N Motor Driver | Motor power control | Converts control signals from the ESP32 into higher-current motor drive outputs | ৳180 – ৳220 | ![L298N](images/motor-driver.jpg) |
| MG996R Servo Motor | Arm joint actuation | Provides torque for the shoulder, elbow, and wrist joints of the robotic arm | ৳650 – ৳750 | ![MG996R](images/servo-motor.jpg) |
| 12V DC Gear Motor | Mobile drive | Drives the wheels of the mobile chassis with speed and torque suited for the robot base | ৳350 – ৳550 | ![DC Gear Motor](images/car.jpg) |
| OLED Display (0.96" I2C) | Status display | Shows system status, sensor readings, and operational messages | ৳320 – ৳400 | ![OLED Display](images/display.jpg) |
| Acrylic Robot Arm Kit | Structural frame | Provides the physical arm structure and mounting points for sensors and servos | ৳1,200 – ৳1,600 | ![Acrylic Arm](images/arm.jpg) |

## Component Descriptions
### ESP32 Microcontroller
The ESP32 is the main controller of the AURA system. It executes the control logic, reads data from the sensors, and sends drive signals to the motors and servos.

### VL5303X Time-of-Flight Sensors
These sensors measure the distance to the artifact without contacting it. They use a light pulse and timing measurement to determine the exact range, enabling the arm to maintain a safe cleaning distance.

### GP2Y1014AU0F Dust Sensor
This optical dust sensor detects fine particles in the air near the artifact. When the sensor detects dust above a threshold, it signals the ESP32 to activate the vacuum system.

### 5015 Blower Fan
The blower fan provides the suction force needed to pull dust particles through the nozzle and into the filter chamber. It is sized to deliver enough airflow while remaining compact and quiet.

### L298N Motor Driver
The L298N driver modules allow the ESP32 to control DC motors and servos. They handle the current required by the motors, enabling safe and responsive movement of the robot and arm.

### MG996R Servo Motors
These high-torque servos power the three joints of the robotic arm. They enable precise positioning of the nozzle and allow the arm to move smoothly around artifacts.

### 12V DC Gear Motors
The gear motors drive the robot’s wheels and provide traction for mobility. Their geared design supplies stable torque and speed for navigation across museum floors.

### OLED Display
The OLED screen shows real-time information such as battery status, sensor readings, and operating mode. It helps operators monitor the robot during use.

### Acrylic Robot Arm Kit
The acrylic arm kit provides a lightweight, durable structure for the robot arm. It supports the mounted sensors, nozzle, and servos while keeping the overall system compact.

## Development Notes
The system is built on a lightweight mobile chassis with a three-joint robotic arm. It uses sensors to detect both the artifact and dust before activating suction. A filter chamber and load sensor are included to collect and monitor dust.

## Conclusion
AURA aims to support the preservation of cultural heritage through safe, automated, and efficient artifact cleaning.
