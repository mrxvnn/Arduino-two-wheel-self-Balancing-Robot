# Arduino-two-wheel-self-Balancing-Robot
A two-wheeled self-balancing robot built using Arduino that maintains its balance using real-time sensor data and a PID control algorithm. This project demonstrates core concepts of control systems, embedded programming, and robotics.

**Components Required**
Arduino Uno
MPU6050 (Gyroscope + Accelerometer)
Motor Driver (L293D / L298N)
2 × DC Geared Motors
2 × Wheels
7.4V Li-ion Battery
Chassis / Frame
Jumper wires

**Working Principle**
The MPU6050 sensor detects tilt angle and angular velocity.
Arduino processes this data in real-time.
A PID algorithm calculates how much the robot is falling.
Motors rotate forward or backward to counter the fall.

**Circuit Connections**
MPU6050 → I2C (SDA, SCL)
Motor Driver → PWM pins
Motors → Motor driver outputs
Battery → Motor driver + Arduino

**PID Tuning (IMPORTANT)**
double Kp = 15;
double Kd = 0.9;
double Ki = 140;

Kp → controls reaction strength
Kd → reduces oscillations
Ki → stabilizes over time

If you don’t tune this properly, your robot WILL fall. This is the hardest part of the project.

**How to Run**
Assemble the robot properly
Upload the Arduino code
Open Serial Monitor
Adjust PID values
Test on a rough surface for better grip

**Applications**
Robotics learning
Control systems understanding
STEM/Engineering projects
Autonomous balancing systems

