# PROJECT: BUILD MY WORLD

![alt text](https://user-images.githubusercontent.com/53105229/128580621-64c7c4dd-8ab1-471e-a8f9-99d654e52b8f.JPG)

## OBJECTIVE
To create a simulation world for all your projects in this [Robotics Software Engineer Nanodegree Program.](https://www.udacity.com/course/robotics-software-engineer--nd209)
1. Build a single floor wall structure using the Building Editor tool in Gazebo. Apply at least one feature, one color, and optionally one texture to your structure. Make sure there's enough space between the walls for a robot to navigate.
2. Model any object of your choice using the Model Editor tool in Gazebo. Your model links should be connected with joints.
3. Import your structure and two instances of your model inside an empty Gazebo World.
4. Import at least one model from the Gazebo online library and implement it in your existing Gazebo world.
5. Write a C++ World Plugin to interact with your world. Your code should display “Welcome to ’s World!” message as soon as you launch the Gazebo world file.

## PROJECT STEP OF WROKS
1. Complete learning Gazebo Basics
2. Run Gazebo in the Workspace and then update and upgrade the Workspace `sudo apt-get update && sudo apt-get upgrade -y`
3. Create directories for the world and model files
4. Run Gazebo
5. Create a building model by Building Editor
6. Create a robot model, link all component joints by Model Editor
7. Create world file
8. Create a script file for display “Welcome to Paoryoma’s World!” to terminal
9. Create a CMakeLists.txt file
10. Create a build directory and compile the code
11. Attatch the plugin into world file
12. Launch the world file in Gazebo
13. Visualize the output

## FILE DIRECTORY STRUCTURE
```
.buildMyWorld                      # Build My World Project 
├── model                          # Model files 
│   ├── myBuilding
│   │   ├── model.config
│   │   ├── model.sdf
│   ├── myModel
│   │   ├── model.config
│   │   ├── model.sdf
├── script                         # Gazebo World plugin C++ script      
│   ├── welcome.cpp
├── world                          # Gazebo main World containing models 
│   ├── myWorld.world
├── CMakeLists.txt                 # Link libraries 
```
* _myBuilding: A building model_
* _myModel: A robot model_
* _welcome.cpp: Gazebo world plugin C++ script._
* _myWorld.world: Gazebo world file that includes the models._
* _CMakeLists.txt: File to link the C++ code to libraries._

## PROJECT SUBMISSION CHECKLIST
- [x] I am confident all rubric items have been met and my project will pass as submitted.
- [x] Project builds correctly without errors and runs.
- [x] All required functionality exists and my project behaves as expected per the project's specifications.

## TIPS
* Add '\n' at the end of printf to display in terminal: printf("Welcome to Paoryoma\'s World!\n");
