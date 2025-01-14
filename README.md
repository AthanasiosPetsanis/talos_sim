<img title="D.I.R." alt="Alt text" src="/images/dir_horizontal.png">

## A Demonstration of our robot Talos


#### 0. Preview

First of all, clone it to your ros workspace source file then go to your root workspace and type the following commands.
<br>
```git clone -b noetic-devel https://github.com/AltziTS007/talos_sim.git```,
<br>
```rosdep install --from-paths src --ignore-src -r -y```,
<br>
```catkin_make -DCMAKE_BUILD_TYPE=Release -DCMAKE_C_COMPILER=/usr/bin/gcc-8```.
<br>
<br>
And don't forget to sauce.
<br>
```source devel/setup.bash```

#### 1. Launch our world and Talos

To start the simulation go to your terminal and hit ```roslaunch talos_description spawn_robocup.launch``` and hit play to gazebo in the left corner.

#### 2. Launch gmapping

Next, we hit gmapping for mapping ```roslaunch talos_navigation gmapping.launch```.

Move the robot with ```rosrun teleop_twist_keyboard teleop_twist_keyboard.py```.

#### 3. Save the map

Now we save the map by hitting ```rosrun map_server map_saver```.


### 4. Conclusion

The simulation is in an early stage a lot of things need to be optimized from navigation, manipulation, state-machine, and of course vision. 


:warning: *Every bug you encounter, address it to the Issues section above.* :warning:

Thank you!


### Sources from GitHub:

- https://github.com/iralabdisco/ira_laser_tools
- https://github.com/ros-perception/slam_gmapping
- https://github.com/ros-planning/navigation
- https://github.com/pal-robotics/realsense_gazebo_plugin
- https://github.com/issaiass/realsense2_description
- https://github.com/FlexBE/flexbe_app
- https://github.com/robocup-at-work/atwork-commander
