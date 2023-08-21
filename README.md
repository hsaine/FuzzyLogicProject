<h1 align="center">Controlling a Differential-Drive Mobile Robot Using Fuzzy Logic.</h1>


<h1 align="center">Abstract</h1>

The objective of this project is to create a fuzzy controller for a differential drive robot. The aim is to familiarize ourselves with fuzzy logic and to explore the capabilities of Simulink.The project involves modeling the kinematics of the robot in a block and linking it to a block of fuzzy logic. The robot has two speeds, which are both the outputs of our fuzzy controller and the inputs for the robot model. Our system is looped : we initially provide the positions
that the robot should reach, these positions enter a subtract block along with the estimated model measurements to provide errors that are used as inputs for the fuzzy controller. According to the rules and inference used, the controller provides the necessary speeds for the robot to navigate towards the destination. The robot will reach its destination when the errors cancel each other out.

<h1 align="center">General Project Description</h1>

The project involves creating a fuzzy controller that commands a differential drive robot. The overall goal of this project is to construct two general blocks using Simulink: one to implement the file containing the fuzzy logic and one to model the robot. At the outset, the user must provide the destination coordinates (X, Y) and specify the orientation (Theta) of the robot. Each time, the system calculates the error between the arrival point and the estimated point. It calculates the error in both the x and y directions and then squares the sum of these errors. Simultaneously, it calculates the error in Theta. In the end, there are two inputs for the fuzzy logic block: one for Theta and the other for XY. Using the fuzzy controller rules and membership functions, the system provides two outputs: the left wheel speed and the right wheel speed of the robot. These speeds are also inputs for the modeling block. Finally, the system traces the robot's trajectory until the errors converge to zero.The figure below provides a general overview of how the system operates:

<h1 align="center">The fuzzy logic block (Project.fis)</h1>





