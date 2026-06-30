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

<figure><img src="../../../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

| Property            | Value                                                                                                                                                                                                                                          |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DMX Style           | Moving Head Display Style: Moving Head Top, Moving Head Side, Moving Head Bars, Moving Head Top Bars, Moving Head Side Bars, Moving Head 3D                                                                                                    |
| # of Channels       | Defines how many channels the model uses                                                                                                                                                                                                       |
| Number of Preset    | Set the Number of Preset DMX Presets. These define presets are values that are assigned to a Channel when rendering non DMX effects.                                                                                                           |
| Pan Attributes      | Set the Pan Channel, Orientation, Rotation                                                                                                                                                                                                     |
| Tilt Attributes     | Set the Tilt Channel, Orientation, Rotation                                                                                                                                                                                                    |
| Color Type          | RGBW is 4 individual color channels. Color Wheel uses one channel for the color wheel and one for brightness.                                                                                                                                  |
| Shutter Attributes  | Set the Shutter Channel, Open Threshold,  and On Value. 'Open Threshold' is the DMX value when the shutter will open and the light will be visible. 'On Value' is a fixed value the shutter channel will be once enabled, '0' will disable it. |
| Gobo Attributes     | Set the Gobo Channel and (optional) Gobo Rotation Channel, and define named gobo slots. Each slot pairs a name with the DMX value that selects it, so the Moving Head effect can choose a gobo by name and animate its rotation. See below.    |



### Gobo Support

Moving Head models can be configured with a gobo wheel. In the model properties you set a **Gobo Channel** and, for fixtures with a rotating gobo, an optional **Gobo Rotation Channel**. You then define **named gobo slots**, each pairing a friendly name with the DMX value that selects that gobo on the wheel.

Once the model is configured, the Moving Head effect provides a Gobo tab that lets you pick a gobo by name and set its rotation, so you do not have to remember the raw DMX values for each slot.

<!-- TODO: screenshot -->

{% hint style="info" %}
Due to the Custom Render Styles of DMX model it is recommended to use Per Model Default render style when added effects to a group of DMX Models
{% endhint %}
