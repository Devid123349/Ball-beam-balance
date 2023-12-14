# Ball-Beam-Balance

Here's simplified overview of the ball and beam balance system:

System Components:

Beam: A horizontal beam where the ball can roll.  
Ball: A small ball placed on the beam.  
Actuators: Devices that can manipulate the beam's angle, affecting the ball's position (Servo Gear).  
Sensors: Devices that measure the ball's position on the beam (Ultrasonic Distance Sensor).  

Control Objective:
The objective is to control the position of the ball on the beam to maintain it at a desired location. This is achieved by adjusting the angle of the beam using feedback control.

Control Steps:

Measurement: Sensors detect the current position of the ball.  
Comparison: The measured position is compared to the desired position.  
Control Action: A control algorithm calculates the necessary adjustment to the beam's angle based on the position error.  
Actuation: The actuators adjust the beam's angle according to the calculated control action.  
Feedback Loop: The process continues iteratively, with the control algorithm constantly adjusting the beam's angle based on the position feedback.  

Control Strategies:
Proportional-Integral-Derivative (PID) Control: A commonly used feedback control method that adjusts the control action based on the proportional, integral, and derivative terms of the error signal. Rectification of sensor noise using Exponential filter. 

Challenges and Considerations:

Stability: Ensuring that the ball remains at the desired position without oscillations.  
Nonlinearities: The ball and beam system exhibits nonlinear behavior due to factors like friction and inertia.  
Sensor Noise: Real-world sensors can have noise, affecting the accuracy of position measurement.   
Actuator Limitations: Actuators may have constraints on their range and speed.  

Technology Used: Arduino
