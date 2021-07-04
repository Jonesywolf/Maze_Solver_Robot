# Maze Solver Robot
Source code for a stewart platform based robot that solves marble mazes using computer vision.

## Mechanical Design Inspiration
I plan to base the robot's mechanical design on the 3 DOF stewart platform described in this Instructable: https://www.instructables.com/3DOF-Ball-on-Plate-Using-Closed-Loop-Stepper-Motor/, albeit with some modifications, namely the design will replace metal parts with 3D printed parts and the encoders will be replaced by much cheaper alternatives or not used at all. Perhaps servo motors may be used instead, provided they can operate smoothly.

## Electronics
For now, development will primarily focus on software, which will be developed on my PC. However, the end goal is to deploy the python code on a Raspberry Pi 4 for portability. An Arduino of some 

## Software Design Philosophy
I plan to practice test driven development for software development, as reccommended by INSERT NAME HERE in his book *The Clean Coder*.

## Current project roadmap
- [ ] Dynamically generate a 2D maze, likely using a technique similar to that described in this article: https://scipython.com/blog/making-a-maze/
- [ ] Create an STL file from the 2D maze for 3D printing, come up with vision targets or another technique to distinguish walls from the base plate
- [ ] Try to recreate the 2D maze using computer vision
- [ ] Track the ball using computer vision
- [ ] Solve the 2D maze and determine a path for the ball to follow
- [ ] Create the stewart platform, mounting the camera above the maze, attached to the maze baseplate so that the camera is always looking straight down at the maze, regardless of the platform's orientation
- [ ] Use inverse kinematics to translate motor movements to a desired pitch roll and yaw of the platform on the Arduno
- [ ] Use PID to make the ball follow the path
- [ ] Add support for hole obstacles in the maze, adding the necessary computer vision and path alterations as necessary
