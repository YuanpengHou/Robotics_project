# Deep Reinforcement Learning for Robot Manipulator Control

## CMSC 756/ENEE 769M · Final Project

In this course project, we aim at exploring the application of deep reinforcement learning (DRL) techniques for controlling a robot manipulators. Robot Deep Reinforcement Learning (DRL) for Arm Manipulation is an aera at the intersection of robotics and machine learning. Arm manipulation refers to the control and movement of robotic arms to perform various tasks in a given environment, such as pick-and-place operations, assembly, and other forms of manipulation. We can consider manipulator parameters as different actions and the objective as rewards. These arms can have multiple joints, allowing for a wide range of movements. Deep Reinforcement Learning involves using deep neural networks to approximate the policy or value function in reinforcement learning. Deep learning enables the model to handle complex and high-dimensional input spaces, making it suitable for tasks like robotic control.

Robot manipulator control is a critical aspect of robotics, and the integration of DRL has shown promising results in enhancing the adaptability and efficiency of robotic systems. The integration of DRL with robotic arm manipulation involves training an agent (the robotic arm) to perform specific tasks or achieve goals by learning from its interactions with the environment. The agent might learn to control the joints of the robotic arm to grasp objects, navigate through an environment, or carry out complex manipulation tasks.

To summarize, we aimed to

(1) Implement a robot manipulator simulation environment using ROS and Gazebo;

(2) Develop and train deep reinforcement learning models for robot manipulator control;

(3) Evaluate the performance of DRL algorithms in comparison to traditional control methods.

## Building the Project for Nvidia Jetson TX2 Platform

Built a project from source, specifically tailored for the Nvidia Jetson TX2 platform. The process involves using the terminal to execute a series of commands:

1. Install cmake:

   ```bash
   $ sudo apt-get install cmake
   ```

2. Clone the project repository:

   ```bash
   $ git clone http://github.com/udacity/RoboND-DeepRL-Project
   ```

3. Navigate to the project directory:

   ```bash
   $ cd RoboND-DeepRL-Project
   ```

4. Update submodules:

   ```bash
   $ git submodule update --init
   ```

5. Create a build directory:

   ```bash
   $ mkdir build
   $ cd build
   ```

6. Run cmake:

   ```bash
   $ cmake ../
   ```

7. Build the project:

   ```bash
   $ make
   ```

During the cmake step, Torch will be installed, so it may take a while. The process will involve downloading packages and may prompt you for your sudo password during the installation.
