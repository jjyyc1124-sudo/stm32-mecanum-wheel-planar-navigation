# stm32-mecanum-wheel-planar-navigation
A high-precision planar navigation algorithm implementation for 4-wheel Mecanum wheel mobile robots, supporting real-time path planning, pose correction and motion control on flat surfaces.
This project focuses on the design and development of an energy-efficient intelligent handling robot that autonomously completes material handling tasks as assigned.
The robot was independently developed by a team of three members (including myself). It is capable of receiving handling tasks by scanning QR codes or via communication means, 
and can transport materials to designated locations in a specified industrial scenario, placing them accurately in accordance with task requirements (i.e., the color and number of color rings, 
or the color and position specified by QR codes/barcodes).
The software environment for this project includes the Ubuntu 18.04 operating system and Keil development tool.
I was primarily responsible for the low-level development of STM32F4 (ST series MCU) and software programming for the host computer, while also participating in the mechanical structure design of the robot.
I utilized CAN bus communication and complied with the CAN 2.0 protocol to control four stepper motors of the chassis and two joint motors on the robotic arm.
I obtained the robot's planar coordinates on the 2D map via RS232 communication with Action, and independently developed the entire planar navigation algorithm (conversion between the world coordinate system and the robot's own coordinate system).
I performed motion calculation for the Mecanum wheels of the chassis to achieve closed-loop speed and position control, and completed the robot's global map navigation as well as the overall handling control of the robot.
