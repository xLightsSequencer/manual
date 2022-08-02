# NULL Controller

## NULL Controller

NULL controller type is used to generate channel blocks with no physical hardware or controller. This type of controller is used in setups, where the sequence output will not be used by xLights as a show player, but output data to be used for playback on a standalone controller.

![](<../../../.gitbook/assets/image (45).png>)

There could be large matrices to be implemented via P10 or P5 panels running off a BeagleBone Black controller. A null output can reserve a huge number of channels, but not actually output anything if the Output to Lights function is on. A model can still be sequenced as normal and viewed on all the windows just as any other output.

### Channels

Number of channels of the null controller. It defaults to 512 channels but can be changed to a larger number.

### Adding Controller

![](<../../../.gitbook/assets/image (364).png>)

Click on Add Null and specify the number of channels to be reserved.&#x20;
