## Autonomous Bot for MIT Duckietown

**Project description:** This project was aimed at recreating the self driving car systems in a miniature town and explore the problems faced by the sensing components on the road. To have a standard design and testing environment, this project was implemented within the specifications of the Duckietown Project which was initiated by Massachusetts Institute of Technology. Due to this being a part of a faast paced course, least resistance methods to implement a working model were preferred. The basic elements that were used  

### 1. Implementing Odometry using IR sensors

Odometry is the use of data from motion sensors to estimate change in position over time. For this project we used IR sensors which can detect the reflectance of a surface that it faces. We then placed black and white quadrature circles in front of then near the wheel hub which will cause a change in current each time it switches colors. The counts of each switch were recorded using the Arduino and speed and distance were calculated.

### 2. Cruise control(obstruction detection) using ping sensors

To detect obstruction directly ahead of the vehicle, we used a ping sensor which works on the principle of ultrasound. A Proportional deviative control was implmented to cntrol the motor drive based on the distance output from the ping sensor.

### 3. Lane Finding and PD control using PiCamera

<img src="images/dummy_thumbnail.jpg?raw=true"/>

### 4. Path Planning and navigation state machine

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

## Final Test Run



## Brownie points for being cool
