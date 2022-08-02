# Fan

![Icon](<../../.gitbook/assets/image (385).png>)

![Sequencer Grid](<../../.gitbook/assets/image (697) (1).png>)

{% tabs %}
{% tab title="Position" %}
![](<../../.gitbook/assets/image (98) (1).png>)
{% endtab %}

{% tab title="Blades" %}
![](<../../.gitbook/assets/image (149).png>)
{% endtab %}

{% tab title="Options" %}
![](<../../.gitbook/assets/image (732).png>)
{% endtab %}
{% endtabs %}

The Fan effect creates spiralling blade like objects that move around the model either clockwise or counterclockwise. Used most effectively on models such as a mega tree or a matrix.

One or many colors can be used for the effect. If multiple colors are selected, then the blades of the fan will be made up of the selected colors.

| Option/Settings           | Description                                                                                                  |
| ------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Position: Center X,Y**  | Defines the x and y coordinates of the center (i.e. focus) point of the fan effect.                          |
| **Position: Radius 1**    | Defines the lower radius of the fan.                                                                         |
| **Position: Angle**       | Defines the angle of each arm of the fan.                                                                    |
| **Position: Radius 2**    | Defines the upper radius of the fan.                                                                         |
| **Position: Revs**        | Defines the number of 360 degree rotations per timing mark the effect is in.                                 |
| **Blades: # Blades**      | Defines how many blades the fan effect will use per color selected.                                          |
| **Blades: Width**         | % of area that the width of each blade will take on the effect.                                              |
| **Blades: Angle**         | Angle of each blade from center.                                                                             |
| **Blades: # Elements**    | How many segments each blade is divided into - default is 1.                                                 |
| **Options: Duration**     | Controls the swell i.e. the amount of time that the fan swells out.                                          |
| **Options: Acceleration** | Controls how quickly the fan swells out and then back in.                                                    |
| **Options: Reverse**      | Reverses the direction of the rotation of the fan effect.                                                    |
| **Options: Blend Edges**  | Each edge blends to black. Turning it off converts the fan effect to a full circle at the end of each swell. |

{% hint style="success" %}
Playing with the radius values i.e. making radius 2 less than radius 1 can provide some interesting effects.
{% endhint %}

{% hint style="success" %}
You can create four Fan effects that each take up about one quadrant of your model (matrix/house) and have them all doing different thing with their arms blending at the edges. The four positions would be x25:y25, x25:y75, x75:y75, x75:y25.
{% endhint %}
