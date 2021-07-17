# Robot State Publisher Problem Solution

This repository will solve the robot state publisher problem

Because I am using the ROS system melodic version, I’m going to use this site [The Construct](https://www.theconstructsim.com/) to work on the ROS Noetic version online.

---

At first, we open the Terminal and write this command: `$ cd ~/catkin_ws/src`  To go to the workshop file that we made and access the src file to install the robot arm package on it.

---

To install the package, we write this command: `$ git clone https://github.com/smart-methods/arduino_robot_arm.git`.

![01](https://user-images.githubusercontent.com/71232960/126025279-cab30fdb-6b31-436b-81f4-486387cfb409.png)
 
---

After what we installed, we go to the src file, then we choose arduino_robot_arm file, then we go to the robot_arm_pkg file, then to lunch file, we choose the check_motors.launch file, Inside the file we change `type="state_publisher"` to `type="robot_state_publisher"`.

![02](https://user-images.githubusercontent.com/71232960/126025288-9cadb670-3380-4cab-9aba-80ef750958ec.png)

---

In the end, we will download all the requirements but since we use ROS online system we don't need to do it, we just run the arm with this command: $ roslaunch robot_arm_pkg check_motors.launch , And we'll see the arm work successfully and without any errors.

![04](https://user-images.githubusercontent.com/71232960/126025297-87b400fa-cca8-4754-b3f6-e8c6b42374d1.png)
![03](https://user-images.githubusercontent.com/71232960/126025298-a28c2edf-d0b3-4510-8683-c7fd75e82ce2.png)
