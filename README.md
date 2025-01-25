
# 4 DC Motors Control with L293D Motor Driver and Arduino
https://www.tinkercad.com/things/dfGVtZceoNn/editel?sharecode=-ZBHOSFHUy30baYRF_avG9wUK9z2cV-m3_yN-5hZ8-I

### Project Description

This project demonstrates how to control four DC motors using an Arduino and the L293D motor driver. The code provides functionality to make the motors perform specific movements, such as moving forward, backward, and turning alternately to the right and left.

The program simulates the behavior of a robotic system with four wheels, allowing the user to:
1. Move all motors **forward** for 30 seconds.
2. Move all motors **backward** for 1 minute.
3. Alternate between turning **right** and **left** for 1 minute.

The project is designed to work with the following hardware:
- Arduino (e.g., Arduino Uno)
- L293D motor driver IC
- 4 DC motors
- Power supply (e.g., 9V battery or external power source for the motors)
- Connecting wires and a breadboard

### Features
- **Forward Movement:** All motors move forward simultaneously at maximum speed.
- **Backward Movement:** All motors move backward simultaneously at maximum speed.
- **Turning:** The robot alternates between turning right and left by stopping motors on one side while moving the others.

### Components Required
1. **Arduino Uno**
2. **L293D Motor Driver IC**
3. **4 DC Motors**
4. **Power Source** (e.g., 9V battery or external motor power supply)
5. **Breadboard and Jumper Wires**
6. (Optional) **Chassis and Wheels** for a physical robotic system

### How It Works
- The L293D motor driver is used to control the direction and speed of the motors. Each motor has:
  - Two digital pins for controlling the direction (IN1, IN2).
  - One PWM pin for controlling the speed (EN).
- The Arduino sends control signals to the L293D to set the desired motor speed and direction based on the program logic.
- The program executes the following sequence:
  1. Move forward for 30 seconds.
  2. Move backward for 1 minute.
  3. Alternate between turning right and left for 1 minute.

### Setup and Usage
1. Connect the DC motors to the L293D motor driver as per the pin configurations in the code.
2. Power the L293D and Arduino with an appropriate power source.
3. Upload the code to the Arduino using the Arduino IDE.
4. Start the system, and the motors will perform the specified movements.

### Code Overview
The main program contains three primary functions:
- `moveForward()`: Moves all motors forward.
- `moveBackward()`: Moves all motors backward.
- `alternateRightLeft()`: Alternates between turning right and left.
Additional helper functions, `turnRight()` and `turnLeft()`, define the motor behavior during turns.
