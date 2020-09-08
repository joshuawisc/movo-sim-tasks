# CoppeliaSim scenes for Movo simulation

Contains various scenes that simulate a Kinova Movo and various other interactable objects.

## Requirements
1. ROS
2. [Movo Control ROS Package]()

## Instructions

I had to recompile a CoppeliaSim plugin to include some movo messages. You could try to do the same thing but it would probably be easier to temporarily replace your plugin with mine. Just backup your current libsimExtROSInterface.so file and place mine in your CoppeliaSim folder. You can switch it back out after testing.  
The simulation works with the Xbox control system in the Movo control package.

### Running
1. Run roscore
2. Navigate to Movo control ROS workspace and source devel/setup.bash
3. Run - `roslaunch movo_mimicry movo_sim.launch`
4. Open another terminal and source devel/setup.bash
5. From the same terminal, open CoppeliaSim (run ./coppeliaSim.sh in the CoppeliaSim folder)
6. In CoppeliaSim, open one of the scenes in the tasks folder
7. Click play on the simulation

### The simulation should be running and the robot should be controllable at this point

## Tasks (Scenes)
1. movoScene - General scene to play around in
2. movoStack - Stack blocks on opposite side of table
3. movoMultipleTransfer - Transfer the blocks into the empty area on the desk
4. movoMovingBlocks - Transfer the blocks off the belt
5. movoLargeBlock - Grab the large block with both arms and move it across the table
6. movoDoublePour - Pour the marbles from one glass to another
7. movoMarker - Grab the marker and draw on the desk
8. movoPointTouch - Point at a cube with the left arm and grab a cube with the same color with the right arm
9. movoDoor - Grab handle and open and close door
10. movoDrawer - Grab handle and open and close drawer
11. movoFork - Stab object at and angle to pick them and make the fork vertical to drop the object
12. movoSpoon - Grab the spoon and scoop the marbles from the table
