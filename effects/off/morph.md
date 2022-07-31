# Morph

## Morph

![Icon](<../../.gitbook/assets/image (297).png>)

![Sequencer Grid](<../../.gitbook/assets/image (512).png>)

{% tabs %}
{% tab title="Start" %}
![](<../../.gitbook/assets/image (756).png>)
{% endtab %}

{% tab title="End" %}
![](<../../.gitbook/assets/image (694).png>)
{% endtab %}

{% tab title="Options" %}
![](<../../.gitbook/assets/image (849).png>)
{% endtab %}
{% endtabs %}

The Morph effect creates a Movement across a model of one or many strands of lights with a head and tail. The Morph effect looks best on mega trees, arches and matrix models but is not limited to those models.

In the Color selection there can be from 1 to 8 colors used for the morph. The color selection is from left to right. If one color is selected the whole morph will be that color. If two colors are selected the Head will be set to the first selected color and the Tail with the second selected color.

If three colors are selected the Head will morph from color1 to color2 then will morph to Color 3. If more than 3 colors are selected then the tail will continue to morph from color3 to color4 to color 5 to color 6. Note if you only want the tail to morph then set color1 and color2 to the same color. If a color gradient color is used then the color morphing can be almost infinite.

A morph can start anywhere and end anywhere on a model. The starting and ending locations are specified by the X,Y coordinates on the Start/End tabs.

| Option/Setting                                                        | Description                                                                                                                                                                           |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Start : X1a**                                                       | Defines the first lateral position starting point (0 is bottom).                                                                                                                      |
| **Start : Y1a**                                                       | Defines the first vertical position starting point (0 is left).                                                                                                                       |
| **Start : X1b**                                                       | Defines the second lateral position starting point (100 is top).                                                                                                                      |
| **Start : Y1b**                                                       | Defines the second vertical position starting point (100 is right)                                                                                                                    |
| **Start : Head Length**                                               | Defines how long the head will be and is depicted by the head effect on the grid.                                                                                                     |
| **Start : Link Points**                                               | Enabling this option will cause the X,Y B points to be linked to the X,Y A points.                                                                                                    |
| <p><strong>Morph</strong></p><p><strong>Quickset Options</strong></p> | These options allow the user to quickly choose a commonly used morph type and direction. These are customizable after they are selected.                                              |
| **End : X2a**                                                         | Ending position 2 on the horizontal axis (100 is top).                                                                                                                                |
| **End : Y2a**                                                         | Ending position 2 on the vertical axis.                                                                                                                                               |
| **End : X2a**                                                         | Ending position 2 on the horizontal axis.                                                                                                                                             |
| **End : Y2b**                                                         | Ending position 2 on the vertical axis.                                                                                                                                               |
| **End : Head Length**                                                 | Defines the relative size of the head when the morph reaches the end points.                                                                                                          |
| **End : Link Points**                                                 | Enabling this option will cause the X,Y b points to be linked to the X,Y a points.                                                                                                    |
| **Head Duration**                                                     | Defines how long the head will show during the morph before it changes to the body colors.                                                                                            |
| **Acceleration**                                                      | Defines a non-linear speed for the movement of the morph.                                                                                                                             |
| **Repeat Count**                                                      | This is used when selecting a single morph and you want it to repeat x number of times.                                                                                               |
| **Repeat Skip**                                                       | Sets the number of legs on the model that the morph will skip when the repeat option is enabled.                                                                                      |
| **Stagger**                                                           | This is used in conjunction with the single line morph and repeat. It can be set to positive or negative values for left or right sweeping type morphs. Small values look best (1-4). |
| **Show Head at Start**                                                | When used with the stagger option, the head of each morph will show prior to the morph moving based on the stagger interval.                                                          |
| **Swap Start and End Points**                                         | Button to Quickly swap the start and end points of a morph, which effectively reverses the morph.                                                                                     |

{% hint style="success" %}
Open and use the Effect Assist window. The window will display a grid corresponding to the x,y start and end coordinates. If you then grab a slider for the morph effect and move it, the Effect Assist window shows exactly where the coordinate is being moved to, making it easier to determine what is being done to the effect. Double click to reset the coordinates to defaults.
{% endhint %}

![](<../../.gitbook/assets/image (1123).png>)
