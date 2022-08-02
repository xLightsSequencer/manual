# Setting Start Channels

## Automatic Start Channels

If Auto Layout Models is enabled in the Controller Tab, xLights will automatically calculate the Model Start and End Channels based on the controller settings.

![](<../../../../.gitbook/assets/image (38).png>)

First Set the Controller the model will be connecting to.

![](<../../../../.gitbook/assets/image (36).png>)

Then Set the Controller Port

![](<../../../../.gitbook/assets/image (709).png>)

If assigning multiple models to one controller port you must set the model chaining to determine the order of the models on the controller output.

![](<../../../../.gitbook/assets/image (147).png>)

## Manually **Changing Start Chanel**

First Change the Controller Dropdown to "Use Start Channels" in the model settings.

![](<../../../../.gitbook/assets/image (73).png>)

Click within the Start Channel cell and then click on the highlighted box to open up The Start Chanel Window. &#x20;

![](<../../../../.gitbook/assets/image (552).png>)

![](<../../../../.gitbook/assets/image (704).png>)

The 'Offset From' determines how the start address is calculated. If the offset is set to "None" the start channel is then used to define the absolute channel number.&#x20;

However it is possible to use other definition setups:

If you select the ‘Universe Number’ option, the start channel for the model is calculated based on the “start channel” that is offset from this ‘Universe Number’.&#x20;

If you have one controller setup on your controller tab with universes 10 through 14, all with 510 channels, for the model set as Start Channel “1”, From Universe “11”, its real absolute start channel in the FSEQ would be channel 511  (first channel of the Universe 11).

The “ANY” value indicates that the Universe is not specific to an IP address and therefore xLights searches for the universe number. (This is the recomended setting to use)

You can specify a specific IP address if you wish - in the unusual event that you have the same universes on different controllers on different IP addresses.  &#x20;

The start channel value can also be specified relative to other channels using the End of Model or Start of Model options. You can specify an offset from an output number or select the start channel to start from the end of another model or align with the start of another model (in the last two scenarios, the model name  is to be selected from a drop down box).

This options works well if your models are reasonably static as the channel numbers are automatically calculated. If however, you delete models then it can break the chain . xLights will alert you to this , but the popup dialogs could be tricky to navigate through.

The ‘Controller’ option, uses the controller name to determine the start channel for the model. It is calculated based on the “start channel” that is offset from the Controller Start Channel in the Controller Tab. This option works well for P5 or P10 Panels running of a FPP controller.

