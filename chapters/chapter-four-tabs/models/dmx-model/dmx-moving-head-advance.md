# DMX Moving Head Advance

Model Setup:

* Define most of the parameters the way you would for the existing moving head 3D model
* Use the "Orient to Zero" parameters to get the pan/tilt positions in layout to make the head look like it does when its commanded to 0 which is usually the bootup position.
* We want to define a Common starting position with the head point Up and facing Forward. All commands will be relative to that starting position I call the "Home" position. So we have a Zero position and a Home position.
* You define the Zero position by viewing the layout and you define the Home position by creating a blank sequence and dropping a Moving Head Effect on the head. Click the center of the position grid so that it will latch a Pan=0 Tilt=0 command into the heads settings. If the head is not pointing Up and Forward then you need to adjust the degrees in the Orient Forward and Orient Up parameters for the pan/tilt motors. Just change the settings and come back and click on the effect to see it change. If you use an old school effect to position the head you should see how it points to the Zero position when commanded to Zero whereas the Moving Head Effect should apply the Home position offset.

Parameters:

* Fixture: You need to set the fixture position for each head MH1 through MH8. This teaches xLights where each head is positioned so that when you tell it to do a Fan it know how to space out the heads. You can assign more than one head to a position if desired.
* PanMotor:\
  Channel (Coarse): Required.....define the main pan channel\
  Channel (Fine): For 16 bit heads. The Fine channel is optional and can be set to 0 to disable.\
  Min Limit (deg): Limit how many degrees the head will pan to the left starting from facing forward\
  Max Limit (deg): Limit how many degrees the head will pan to the right starting from facing forward\
  Range of Motion: How many total degrees does the head pan when commanded from 0 to 255\
  Orient to Zero: Number of degrees to spin the head so it matches the position when commanded to 0\
  Orient Forward: Number of degrees to spin the head from its Zero position so it faces forward\
  Slew Limit (deg/sec): Number of degrees your head can move per second to try to make the screen match reality\
  Reverse: Check this box if your head moves counter-clockwise when commanded from 0 to 255\
  Upside Down: Check this box if you head is mounted inverted
* TiltMotor:\
  Channel (Coarse): Required.....define the main tilt channel\
  Channel (Fine): For 16 bit heads. The Fine channel is optional and can be set to 0 to disable.\
  Min Limit (deg): Limit how many degrees the head will tilt backwards from facing up\
  Max Limit (deg): Limit how many degrees the head will tilt forwards from facing up\
  Range of Motion: How many total degrees does the head tilt when commanded from 0 to 255\
  Orient to Zero: Number of degrees to spin the head so it matches the position when commanded to 0\
  Orient Up: Number of degrees to spin the head from its Zero position so it faces up\
  Slew Limit (deg/sec): Number of degrees your head can move per second to try to make the screen match reality\
  Reverse: Check this box if your head moves counter-clockwise when commanded from 0 to 255\
  Upside Down: Check this box if you head is mounted inverted
* Most other properties are similar to the previous moving heads
* BaseMesh, YokeMesh, HeadMesh: These can be used to change the OBJ objects used to draw the head.
