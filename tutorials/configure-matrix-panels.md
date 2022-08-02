# Configure Matrix Panels

## **Configure P10 Matrix Panels**

In this example, the setup consists of 8 P10 panels (4H x 2 W) driven via a Beagle Black Bone (BBB) with an octoscroller running the Falcon Player (referred to as the FPBBB). This process should be the same for Raspberry Pi's running FPP with a Pi Hat or Colorlight Card.

First Add a New Ethernet Controller to the Controller Tab. It is recommended to use a DDP Protocol for FPP based P10/P5 panels. An E131 Protocol can also be used but for this guide DDP was selected.

![](<../.gitbook/assets/image (119).png>)

![](<../.gitbook/assets/image (3).png>)

Set the Name to FPPBB. Set the IP Address of the device IP(192.168.5.200 in this example). The Id is a unique controller ID for xLights to use, this Id must be different for each out. The default Id of 1 is okay for this example. The number of channels is the total number of channels for the P10 matrix. To calculate this number channels, multiple the number of channels per LED(3 in most cases) by the number of LEDs per panel(512 for P10's) and then multiple that result by the number of Panels(eight in this example). The final values is the total channel for the Matrix.

$$
Channels Per LED  * LED Per Panel * NumberOfPanel  = Channel Count
$$

For this example, the total number of channels is: 3 x 512 x 8 = 12288 channels.

![](<../.gitbook/assets/image (361).png>)

Set the Description Field To 'P10Matrix' and set the Vendor to 'FPP' and the Controller Type to 'PiHat'. The Description . Enable the 'Auto Upload Configuration' setting.

Click 'Save' when complete.

![](<../.gitbook/assets/image (296).png>)

Next, Define a model ‘P10Matrix’ for in the Layout Tab

![Layout Tab](<../.gitbook/assets/image (634).png>)

First Select the 'Matrix' model icon in the Model Toolbar.

![Matrix Model ](<../.gitbook/assets/image (496).png>)

Click the Left Mouse Button Down then Drag the Pointer to the Right, and Release.

![](<../.gitbook/assets/image (115).png>)

Next, define the model settings. Set the model name to ‘P10Matrix’ (or any name of your choice) set it as a horizontal matrix.

![](<../.gitbook/assets/image (282) (1).png>)

Set ‘# Strings’ = 64 (corresponds to number of rows), ‘Nodes/String’ as 64 (corresponds to the columns) and ‘Strands /String’ = 1. 'Starting Location' = Top Left.

{% hint style="info" %}
A single 32 \* 16 P10 panel has 16 rows (height) and 32 columns (width). Right click on the image in your Layout and select Node Layout to view the node definition.
{% endhint %}

To set the Start Channel Click the Ellipsis(three periods) button in the Start Channel Box.

![](<../.gitbook/assets/image (622).png>)

Set the start Channel by Clicking the 'Controller' Option and selecting the Controller Name set earlier, from the drop-down list. Keep the 'Start Channel' set to 1.

![](<../.gitbook/assets/image (37).png>)

The start channel should be set to '!P10Matrix:1' and xLights will automatically calculate the end channel.

![](<../.gitbook/assets/image (40).png>)

Click the 'Save' Button when done.

![](<../.gitbook/assets/image (347).png>)

### Upload Config to FPP

Switch back to the Controller Tab. Highlight the 'FPPBB' controller and click 'Upload Output'. This will automatically set the Panel Start channel In FPP for you.

![](<../.gitbook/assets/image (58).png>)

### **BBB FPP definition**

Open The Beaglebone controller web page by entering the IP address in your web browser of choose or by right-clicking on the DDP output and selecting 'Open Controller'.

![](<../.gitbook/assets/image (608).png>)

Set the FPP controller to bridge mode for testing for now. When running your show you can use bridge mode or switch to FPP Remote Mode, both will work with the DDP setup. No channel inputs need to be setup the DDP protocol handle that for you.

Click the 'Input/Output Setup' Menu Banner and Select the 'Channel Outputs' Option

![](<../.gitbook/assets/image (263).png>)

On the LED Panel page, Check the Enable LED Panel Output Option. The panel layout is 2 x 4. The Start channel should automatically been updated by the Upload To Controller Option used earlier. Make sure this matches the model definition in xLights. 'Single Panel Size' sets the Panel Size and Scan Rate. For most indoor P10 panels this is '32x16 1/8 Scan'. The channel count is automatically is calculated. This should also match the model in xLights. The 'Model Start Corner' should be the same as the 'Starting Location' in xLights. 'Default Panel Color Order' should match the panel vendors recommendation. Different vendors use different Color Orders. You may have to do try all the options to find the correct one. 'Brightness' is the Panel brightness, 10 is 100%, 1 is 10%. All the other options keep to the defaults.

![LED Panel Output Page](<../.gitbook/assets/image (88) (2).png>)

The vertical arrows correspond to the Up/Down physical setting of the arrows on the panel backside. The LED Panel Layout orientation is as if viewed from the **front** of the panels. 'O-1', 'O-2', 'O-3', etc are the outputs ports on the Octoscroller. 'P-1', 'P-2', 'P-3', etc. is the panel order for each output. The first panel connected to the Octoscroller output is 'P-1', the second panel is 'P-2' and so forth.

![Octoscroller](<../.gitbook/assets/image (79) (1).png>)
