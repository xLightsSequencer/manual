# Models

## **Models**

A model in xLights defines the entire required characteristic about a single physical element of your display. Typically it will represent a common item such as an arch, a matrix, a straight line, flood light as well as more esoteric and custom made items such as singing trees, candy canes, a snowman etc.

It defines the type of lights(RGB, Single Channel, etc), the number of channels, and other characteristics required to render the sequence data. When a model is defined, it is retained in the xLights configuration "xlights\_rgbeffects.xml" file in the show directory. It can be reused for all subsequent sequences.

{% hint style="info" %}
A model is made up of one or more strands, and each strand is made up of one or more nodes.
{% endhint %}

### Adding Models

At the top of the layout screen is a row of Model icons. If you hover the cursor on each icon, the model name will be displayed. The model icons represent an Arch, Candy Cane, Circle, Custom model, Icicles Matrix, Single Line, Spinner, Star, Tree, Window Frame, Wreath and Import Custom. The last icon labelled ‘Import’ Custom enables you to import and create a custom model that has been exported from another sequence.

![](<../../../.gitbook/assets/image (213) (1).png>)

To define a new Model, click on the Model icon that you wish to create once. The model icon will have a dark blue square around it. Then with your mouse left button click on the layout canvas , and keep your mouse button still held down. The model shape will appear on the canvas in yellow. If it does not , then left click on the canvas and drag slightly. At the same time , a model is created and displayed in the Model panel that is normally to the left of the Layout screen.

Depending on the type of model, it will either be bounded by four, three points or two points.

In this image, the Candy canes have three points. The bottom left is green and marks the beginning of the model, the bottom right is blue and marks the end of the model and the top center is blue and is used to rotate the model.

![](https://lh3.googleusercontent.com/o06l9Z-jiblMKk6FTb-AW8Mp3ADwhBl5Qp-6BIyd34JwW8Wl51Hr0Bjremvzd75EIOu7hRMngXIHg7uSBV7SmhbgTI6WQCr0TGKj14H6uLQBH1HT4n9bRuvxC8z2xgjoexKHswtK)

If you cannot locate your model after it has been created, click on the model name in the panel and the model image will be highlighted.

Note that the Preview window has the ‘Default’ preview displayed - indicating that the model that is being created will be assigned to and displayed on the default House Preview window.

By clicking and holding in the center of the model - you can drag the model to the required position. You can also use the three points to size the model on the layout.

When the model is aligned horizontally, a red horizontal line will be displayed.

![](https://lh5.googleusercontent.com/lx4kE7JP13W3yjoFHo-W8FBkl-tltwJzqm6yxjza\_YXGWQWw5dzjhlaxv9oKoyaxn1Os76aHWwh0ZFe8L54RsYl0Z1NUgszAfh745\_an9AL52cJjQwBoxs4Kj9mRvD6ewmFLKvyf)

When the model is aligned vertically, a blue vertical line will be displayed.

![](https://lh4.googleusercontent.com/B\_Edk9IVKObPYlDR--o\_6J-d7w0YkcYOlwUquOM9OmBRiEwIPwnpyz5hjTyCk1VEBb83bbBE8wWV6zuygYoluynKD9FiJ1hTugLvC6meDAEwjBVb7ngWbCK8IdLXl4YyulC2oP5u)

In this image, the Single Line model has two points. The bottom left is green and marks the beginning of the model, the bottom right is blue and marks the end of the model. The red superimposed red line indicates horizontal alignment.

![](https://lh4.googleusercontent.com/x7UYtT0ngHm30kDD2FXV0lhYUeb-S5JPUsEsrMR5sjYrtSTXwOw-XaVm9Tnvo2ThMA7LNDYARI6\_xL-IgVpWVUW8CIOuNgcsrWqtgAxK2dXtkK\_HIq97zT-ozB\_bLm0RKR5DJY6W)

If you double click on the Single Line model icon (instead of using a single click) , then you can draw a single line (say as part of the roof line), then click on the layout again and draw another segment from the end of the first segment - this will create another model and so on. Or you can use this technique to draw multiple arches at the same time. Click on the model icon again to deselect it.

{% hint style="success" %}
Both of the above examples have alternate ways of being implemented (using the Poly Line model or using the ‘# of Arches ‘ attribute’ in the model definition of the Arch model.
{% endhint %}

On the left of the layout canvas is a window which displays the name of the model that has just been created and the settings of the model.

![](https://lh6.googleusercontent.com/mB-Z-MBswUa4Dku1XYiopTvuAeJgUs\_7IFFqImgaCg9H\_udwDtLWIP8sGtr-gqITTq7CsNTWrFywT2x7gg-k1IoQ8iLQ5ViV\_fDBn-bJCf7z3\_X4C60K7atd3qkkaU9kAXogLcx7)

These are default values and you can then edit the values to suit your requirements - (change the name, start channel , number of nodes etc).

{% content-ref url="model-attribute/" %}
[model-attribute](model-attribute/)
{% endcontent-ref %}

Click on the Preview attribute and change the Preview window if you so require. Set it to ’Unassigned’ if the model is not to be displayed in the House Preview window.

You can collapse or expand any of the windows of the model characteristics.

{% hint style="info" %}
If you hover on a model name, it will display details of the setup configuration such as the names and channel assignments the model maps to on your controller setup.
{% endhint %}

{% hint style="success" %}
If a Model group name is selected when you create a model , the model will automatically be assigned to the selected Model Group.
{% endhint %}

### Deleting Models

To delete a model, highlight the model on the Layout canvas and press the Delete key or press Ctrl X. You can hold down the cursor and drag to form a rectangle around the model and then delete.

![](<../../../.gitbook/assets/image (155).png>)

You can also Right Click on the Model name in the Model list panel. A ‘Delete’ pop up window will be displayed. Click on it to confirm and delete the model.

### Undo

You can also use the Undo function i.e Ctrl-Z to remove the model that has just been added or undo the last model movement. The Undo function can be repeated.

### Creating Multiple Model Instances

You can select the model image on the canvas, press Ctrl-C to copy and then Ctrl-V to paste. A new model instance will be created. You can also double-click on the Model icon that you wish to create. The model icon will have a grey/light blue square around it. Then with your mouse left button click on the layout canvas. The model shape will appear on the canvas (surrounded by five blue squares). A left click on the canvas again at the required location will create another instance of the model. And so on. To end the process, click on any of the model icons once.

### Rename a Model

A model (name) can be renamed by simply changing the Model name.

{% hint style="info" %}
If the model is already part of a Model group, you should update the Model Group definition. If you don’t then xLights will subsequently provide an option to delete or select the new model name when the application is loaded again.
{% endhint %}

### Modify a Model

Details of a model configuration can be amended by updating the details in the relevant section of the model definition. Save the changes.

### Copy a Model

Once a model has been defined, a quick way to duplicate definitions is to select the model in the Layout window, then use a Ctrl-C to copy it and a Ctrl V to paste it. Save the changes.

### Overlap Checks

If the ‘Overlap checks enabled’ attribute is selected, when you click on the model name in the list, it will turn yellow in the layout display to the right. If there is a channel overlap with any other model, then the other model will turn red.

## Right Click Menu

![](<../../../.gitbook/assets/image (60) (1).png>)

{% hint style="info" %}
The Right Click Menu has some entries that don't apply to individual models and they will not be covered in this section.
{% endhint %}

### Reset

Resets the Current Window View to the default. &#x20;

### Correct Aspect Ratio

This will resize the model so the number of node in the vertical and horizontal direction are equally spaced.

### Node Layout

The node layout window is then displayed. The s1, s2, etc. represent the string numbers, the n1,n2,n3,etc represent the node count.

![Node Layout Dialog](<../../../.gitbook/assets/image (794).png>)

### Lock

Lock a model in place to prevent it from being moved. The Model handles will appear red when a model is locked.

![](<../../../.gitbook/assets/image (320) (1).png>)

### Unlock

Unlock a model so a model can be moved.

### Export as a Custom xLights Model

Create a Custom Model file from a built in Model Type. Use only if you wire your model in a non support format and a built in type will not work.

### Wiring View

Displays a view of how to wire your model based on the Model properties. This can be saved or printed by right clicking on the dialog.

![](<../../../.gitbook/assets/image (336) (1).png>)

{% hint style="warning" %}
By default the Wiring View is set to the **backside** or **reverse view** of the model. To switch to the front side, Select "Front" from the right click menu.
{% endhint %}

### Export xLights Model

Export a Model as a .xmodel file and save to the local disk.

### Replace a Model with a Model

"Swap" a new model with an existing model and kept the model name. Use this if want to change a model and keep the same name. This will prevent Model Groups and sequences from breaking.

