# Controllers

## Controllers

{% hint style="info" %}
**You can skip this section if you have not have hardware yet, and do not plan to output data to your lights.**
{% endhint %}

The controllers section defines how the channels are mapped to physical hardware and controllers. It is only used when outputting data to the controllers and can easily be changed at any time.

You do not have to define any controllers when you start , but you will need it defined before you can test any effects on physical lights from within xLights.

If you do want to define the controllers details at this stage, select the Controllers tab and add a controllers. The actual controllers settings does not have to be correct as you can change the details later.

To define a E131/DDP/Artnet type controller, Click on the Add Ethernet button:

![](<../../.gitbook/assets/image (135).png>)

Set the Name of the Controller, this can be any value, but make it something specific that is easy to remember for later use.

![](<../../.gitbook/assets/image (383).png>)

Set the Controller Vendor, Model, and Variant. Not all controllers have a variant type, this will be blank for some controllers.

![](../../.gitbook/assets/image.png)

After setting the Controller Type, Enable the Auto Layout Model option.

![](<../../.gitbook/assets/image (6).png>)

Set the controller "IP address", If unknown just use a generic value like "192.168.1.50". Set the "Start Universe" to 1, "Universe Count" to 20, "Channel per Universe" to 510, and press Enter.

![](<../../.gitbook/assets/image (191).png>)

This will create a basic controller with 20 universes. Each universe will have 510 channels. The start and end channel are automatically calculated and displayed in the mapping column.

Click on Save Button to save the controller setting that were added.

![](<../../.gitbook/assets/image (523).png>)
