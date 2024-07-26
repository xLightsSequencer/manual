# DMX Model

### **DMX model**

![DMX Model Types](<../../../.gitbook/assets/image (15).png>)

The DMX model has a number of different styles and each has a different model representation.

![](<../../../.gitbook/assets/image (57).png>)

After selecting the DMX Mode, a list of Sub Types will display.

### General

![](<../../../.gitbook/assets/image (19).png>)

Used to define any generic DMX Fixture. Can be used for 3/4 Channel RGBW lights or devices like Fog or smoke machines.

### Floodlight/ Area Flood

![](<../../../.gitbook/assets/image (10).png>)

Used for multichannel Flood lights. The Single Line Model can all be used for DMX Floodlights.

### Moving Head/ Moving Head 3D

![](<../../../.gitbook/assets/image (18).png>)

For DMX Moving Heads. Supports Shutter control, RGBW channels, Color Wheel, etc.

### Servo

Induvial Servo Control, Supports 16 bit servos.

### Skull

For Skulls with servos embedded in them. Skulltronix Skulls are also supported.

![](<../../../.gitbook/assets/image (38).png>)

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

| Property            | Value                                                                                                                                                                                                                                          |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DMX Style           | Moving Head Display Style: Moving Head Top, Moving Head Side, Moving Head Bars, Moving Head Top Bars, Moving Head Side Bars, Moving Head 3D                                                                                                    |
| # of Channels       | Defines how many channels the model uses                                                                                                                                                                                                       |
| Number of Preset    | Set the Number of Preset DMX Presets. These define presets are values that are assigned to a Channel when rendering non DMX effects.                                                                                                           |
| Pan Attributes      | Set the Pan Channel, Orientation, Rotation                                                                                                                                                                                                     |
| Tilt Attributes     | Set the Tilt Channel, Orientation, Rotation                                                                                                                                                                                                    |
| Color Type          | RGBW is 4 individual color channels. Color Wheel uses one channel for the color wheel and one for brightness.                                                                                                                                  |
| Shutter Attributes  | Set the Shutter Channel, Open Threshold,  and On Value. 'Open Threshold' is the DMX value when the shutter will open and the light will be visible. 'On Value' is a fixed value the shutter channel will be once enabled, '0' will disable it. |



{% hint style="info" %}
Due to the Custom Render Styles of DMX model it is recommended to use Per Model Default render style when added effects to a group of DMX Models
{% endhint %}
