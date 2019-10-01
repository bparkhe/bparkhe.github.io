## Autonomous Bot for MIT Duckietown

**Project description:** This project was aimed at recreating the self driving car systems in a miniature town and explore the problems faced by the sensing components on the road. To have a standard design and testing environment, this project was implemented within the specifications of the Duckietown Project which was initiated by Massachusetts Institute of Technology. Due to this being a part of a fast paced course, least resistance methods to implement a working model were preferred. The basic elements that were used  

### 1. Implementing Odometry using IR sensors

Odometry is the use of data from motion sensors to estimate change in position over time. For this project we used IR sensors which can detect the reflectance of a surface that it faces. We then placed black and white quadrature circles in front of then near the wheel hub which will cause a change in current each time it switches colors. The counts of each switch were recorded using the Arduino and speed and distance were calculated.
<img src="images/auto_bot/wheel_section.jpg?raw=true"/>

<img src="images/auto_bot/quad_pulses.jpg?raw=true"/>

### 2. Cruise control(obstruction detection) using ping sensors

To detect obstruction directly ahead of the vehicle, we used a ping sensor which works on the principle of ultrasound. A Proportional deviative control was implmented to cntrol the motor drive based on the distance output from the ping sensor.
<img src="images/auto_bot/ping_circuit.png?raw=true"/>


### 3. Lane Finding and PD control using PiCamera

<img width="700" src="images/auto_bot/lane_detection.png?raw=true"/>

### Final Test Run
<video width="640" height="480" controls>
  <source src="images/auto_bot/OuterLoopVision_2.mp4" type="video/mp4">
</video>


### Brownie points for being cool
..and, no he is not crazy, we had him tested :)

<video width="640" height="480" controls>
  <source src="images/auto_bot/cool_bot.mp4" type="video/mp4">
</video>
