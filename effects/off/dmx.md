# DMX

![Icon](<../../.gitbook/assets/image (92) (1).png>)

![Sequencer Grid](<../../.gitbook/assets/image (331).png>)

![](<../../.gitbook/assets/image (85).png>)

The DMX effect is used to output a value between 0-255 to the model. Channel 1 in the DMX effect corresponds to the first channel of the model and up to 18 channels can be controlled.

Use a Single Line model for RGB nodes. As an example, 5 RGB nodes which will create 15 channels of data.

| **Option/Settings** | Description                                                                                                                                                                                                                                                           |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Channels  1-10**  | Select the tab to control Channels 1 -10                                                                                                                                                                                                                              |
| **Channels 11-20**  | Select the tab to control Channels 11-20                                                                                                                                                                                                                              |
| **Channels 21-30**  | Select the tab to control Channels 21-30                                                                                                                                                                                                                              |
| **Channels 31-40**  | Select the tab to control Channels 31-40                                                                                                                                                                                                                              |
| **DMX Value**       | Select the DMX value (from 0 to 255) for the Channel that has been selected.  The channels will be offset from wherever is defined in the model definition.  So if the model for a DMX device starts at channel 450 then the channel 3 slot will control channel 452. |
|                     | Click on the Value Curves icon to open a list of additional nonlinear effects.  Use the Ramp effect to vary the output anywhere from 0 to 255.                                                                                                                        |
| **Remap Channels**  | Remap channels will "move" the DMX from one channel to another. This is used when importing sequences and the source DMX fixture uses different DMX channels.                                                                                                         |
| **Save As State**   | Save the current DMX Values as a State Definition.                                                                                                                                                                                                                    |

{% hint style="success" %}
For Pan/Tilt head control movement, select the Use Ramps attribute and set it to a timing mark of say 10 seconds long. It will move the head for 10 seconds between the ramp values.
{% endhint %}
