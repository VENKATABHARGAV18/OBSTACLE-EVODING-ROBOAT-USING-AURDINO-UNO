# OBSTACLE-EVODING-ROBOAT-USING-AURDINO-UNO
### OVERVIEW

The Obstacle Avoiding Robot is an autonomous robotic system designed to detect obstacles in its path and navigate safely without human intervention. The primary goal of this project is to develop a robot that can move forward automatically and avoid collisions by detecting objects in front of it.

This robot uses an HC-SR04 ultrasonic sensor to measure the distance between the robot and nearby objects. The sensor sends ultrasonic sound waves and measures the time taken for the echo to return after hitting an object. Using this time, the distance to the obstacle is calculated. Based on this information, the robot decides whether to move forward or change its direction to avoid the obstacle.

The system is controlled by an Arduino Uno microcontroller, which processes the sensor data and controls the movement of the motors through an L298N motor driver module. When an obstacle is detected within a certain range, the robot stops, moves backward for a short period, and then turns in another direction to continue its movement.

Obstacle avoiding robots are widely used in many fields such as robotics research, industrial automation, military operations, surveillance 
systems, and autonomous vehicles, where navigation without human control is required.

### OBJECTIVES OF THIS PROJECT

The main objectives of this project are:

1. To design and build a simple autonomous mobile robot.

2. To implement obstacle detection using an ultrasonic sensor.

3. To control motor movement using a motor driver module.

4. To demonstrate how sensors and microcontrollers can be integrated in robotics.

5. To understand basic embedded system programming using Arduino.


THE FOLLOWING HARDWARE COMPONENTS ARE USED FOR THIS PROJECT:

* Arduino Uno

* HC-SR04 Ultrasonic Sensor

* L298N Motor Driver Module

* DC Motors

* Robot Chassis

* Battery Pack or Power Supply

* Connecting Wires

Each component plays an important role in the functioning of the robot. The Arduino Uno acts as the main controller, the ultrasonic sensor detects obstacles, and the motor driver controls the motors that move the robot.

**SOFTWARE REQUIREMENTS**

The software tools required for this project are:

* Arduino IDE

* USB Cable for programming Arduino Uno

* Computer or Laptop


The Arduino IDE is used to write, compile, and upload the program to the Arduino Uno.

### PIN CONFIGURATION
Ultrasonic Sensor Connections

Trig Pin → Arduino Uno Pin 9

Echo Pin → Arduino Uno Pin 10

Motor Driver Connections (L298N)

Left Motor Forward → Arduino Uno Pin 5

Left Motor Reverse → Arduino Uno Pin 4

Right Motor Forward → Arduino Uno Pin 7

Right Motor Reverse → Arduino Uno Pin 6

These pins are configured in the Arduino program to control the ultrasonic sensor and motor driver module.

### WORKING PRINCIPLE

The obstacle avoiding robot works based on the principle of ultrasonic distance measurement.

The HC-SR04 ultrasonic sensor emits high-frequency sound waves that travel through the air. When these sound waves hit an object, they are reflected back to the sensor. The sensor measures the time taken for the sound waves to travel to the object and return.

Using this time value, the Arduino calculates the distance between the robot and the obstacle using the formula:

Distance = Time / 58.2

If the calculated distance is greater than a predefined threshold value, it means that no obstacle is present in front of the robot. Therefore, the robot continues moving forward.

If the distance becomes smaller than the threshold value, it indicates that an obstacle is detected. In this case, the robot stops moving forward, moves backward slightly, and then turns to another direction to avoid the obstacle before continuing its movement.

This process repeats continuously, allowing the robot to navigate through its environment without collisions.

### SYSTEM WORKFLOW

The working process of the robot can be described in the following steps:

1. The ultrasonic sensor continuously sends ultrasonic signals.

2. The sensor receives reflected signals from nearby objects.

3. Arduino calculates the distance between the robot and the obstacle.

4. If the distance is greater than the threshold value, the robot moves forward.

5. If the distance is smaller than the threshold value:

6. The robot stops
 
7. Moves backward for a short time

8. Turns to another direction

9. After turning, the robot continues moving forward.

10. This continuous loop allows the robot to avoid obstacles automatically.

### APPLICATIONS

Obstacle avoiding robots can be used in several real-world applications such as:

1. Military surveillance robots

2. Industrial automation systems

3. Autonomous vehicles

4. Warehouse robots

5. Educational robotics projects

6. Smart navigation systems

These robots can perform tasks in environments where human intervention may be difficult or dangerous.

### FUTURE IMPROVEMENTS

Although this project demonstrates basic obstacle avoidance, several improvements can be made to enhance its performance:

* Adding multiple ultrasonic sensors for better obstacle detection

* Implementing camera-based navigation using computer vision

* Integrating IoT technology for remote monitoring and control

* Using advanced algorithms for intelligent path planning

* Improving movement efficiency using better motor control

### CONCLUSION

The Obstacle Avoiding Robot project demonstrates the basic concept of autonomous navigation using sensors and microcontrollers. By integrating an ultrasonic sensor with an Arduino Uno and a motor driver module, the robot can detect obstacles and change its direction automatically.

This project helps in understanding important concepts such as sensor interfacing, embedded programming, and motor control. It also provides practical experience in designing and implementing a simple robotic system.

The system can serve as a foundation for developing more advanced robotic applications that involve intelligent navigation, automation, and real-world problem solving.
