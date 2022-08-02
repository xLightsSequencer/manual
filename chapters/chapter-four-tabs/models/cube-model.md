# Cube Model

### Cube Model

![](<../../../.gitbook/assets/image (767).png>)

The Cube model is a 3D model that is used to model objects like Pixel/Peace Stakes, Boxes, or Grids. While the model is 3D, xLights renders the effects in 2D. &#x20;



| Options/Settings                | Description                                                                                                                                                                                                                                                                                                               |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Starting Location               | Determines the starting of the pixel string wiring.                                                                                                                                                                                                                                                                       |
| Direction                       | Direction of the wiring and how it "snakes" though the nodes. Horizontal proceeds left and right based on the front perspective. Vertical will go up and down. Stacked will wire each layer then move to the next layer. See below for examples                                                                           |
| Stand Style                     | <p><strong>Zig Zag</strong> - Wiring winds back and forth.</p><p><strong>No Zig Zag</strong> - Wiring follows the direction and starts back at the beginning of the next line.</p><p><strong>Alternate Pixel</strong> - Wiring 'jumps' over every other node to and winds back thought populating the 'jumped' nodes.</p> |
| Layers All Start in Same Place  | All the wiring for each layer will start in the same location.                                                                                                                                                                                                                                                            |
| Width                           | Width of Cube                                                                                                                                                                                                                                                                                                             |
| Height                          | Height of Cube                                                                                                                                                                                                                                                                                                            |
| Depth                           | Depth of Cube                                                                                                                                                                                                                                                                                                             |
| Strings                         | Number of Physical Strings of Pixels or Lights                                                                                                                                                                                                                                                                            |

### Stand Style

{% tabs %}
{% tab title="Zig Zag" %}
![](<../../../.gitbook/assets/image (771).png>)
{% endtab %}

{% tab title="No Zig Zag" %}
![](<../../../.gitbook/assets/image (760).png>)
{% endtab %}

{% tab title="Alternate Pixel" %}
![](<../../../.gitbook/assets/image (735).png>)
{% endtab %}
{% endtabs %}

### Layers All Start in Same Place

![](<../../../.gitbook/assets/image (770).png>)

All the wiring for each layer will start in the same location. Bottom Left in the example above.

### Example Configurations

#### 3W x 3H x 3D, Front Bottom Left, Horizontal Left/Right, ZigZag

![](../../../.gitbook/assets/2022-08-01\_23h15\_41.png)

#### 3W x 3H x 3D, Front Bottom Left, Vertical Left/Right, ZigZag

&#x20;![](../../../.gitbook/assets/2022-08-01\_23h14\_26.png)

#### 3W x 3H x 3D, Front Bottom Left, Horizontal Front/Back, ZigZag

![](<../../../.gitbook/assets/image (728).png>)

#### 3W x 3H x 3D, Front Bottom Left, Stacked Left/Right, ZigZag

![](<../../../.gitbook/assets/image (765).png>)

