# SubModels

## Node Range SubModels

This setting allows the user to specify parts of a model to be controlled as if it were its own model. For example, you could defined the horizontal and vertical section of a windows frame.

![](<../../.gitbook/assets/image (121).png>)

Click Add to create a new submodel. Then add the nodes that will be included in the submodel. On the right side you will see the model and selected nodes will be highlighted.

![](<../../.gitbook/assets/image (242) (2).png>)

On the right side, the model will be displayed with the selected nodes highlighted. If the user clicks the row header(Top or Bottom), the display will highlight only the nodes in the selected row. If the user clicks the "Node Ranges" column header, all the nodes from all the rows will be highlighted.

The Node Ranges 'Grid' represents the submodels render buffer. A grid five row high with five nodes listed per row will create a 5x5 Render buffer.&#x20;



![](../../.gitbook/assets/5by5.png)

Empty Commas(,) can be used to create empty spaces in the render buffer. The example below will create 5x5 a outline with a 3x3 'hole' in the middle.

![](<../../.gitbook/assets/image (628).png>)

{% hint style="info" %}
Always Press 'Tab' after changing the submodel name or adding nodes to a row. This will guarantee the changes will "stick" and not disappear.
{% endhint %}

{% hint style="info" %}
The 'Vertical Buffer Layout' checkbox with rotate the underlining render buffer 90 degrees.
{% endhint %}

To graphically select the nodes, double click the row header or row cell and select the desired nodes. This option will only populate one row at a time.

![](<../../.gitbook/assets/image (552).png>)

{% hint style="info" %}
Un-check 'Ordered Selection' to enable 'Click and Drag' Mode
{% endhint %}

## Draw Model

To Draw a model, like a Cross, across the whole model click the Draw Model Button.

![](<../../.gitbook/assets/image (536) (1).png>)

Click and drag to select nodes(blue highlight). The selected node will turn grey once selected. Double clicking on a node number also toggles between selected and not selected. 'Select All' will select all the nodes. 'Select None' will deselect all the nodes. The 'Ordered Selection' checkbox enables a single select mode that disables 'Click and Drag'(blue highlight) Mode. 'Ordered Selection' is used to select the individual nodes in a specific order to be used by the underlying buffer.

![](<../../.gitbook/assets/image (374).png>)

The "From Model" button allows the user to select nodes based on the custom model "shape". For Example, you can import a snowflake model file to overlay it on a matrix.

Hold the 'Ctrl'/'Cmd' Key highlight the cells and press Ctrl+C to copy them. Ctrl+V can then be used to paste the cells. This data can also be copied to and from Excel.

![](<../../.gitbook/assets/image (553).png>)

Click Ok to Close the select window.

![](<../../.gitbook/assets/image (110) (1).png>)

## SubBuffer SubModel

![](<../../.gitbook/assets/image (366) (1).png>)

The SubBuffer tab allows the user to select sections of the buffer instead of the nodes. This can be used to divide mega trees/matrices into slices for singing face or individual effects.

![](<../../.gitbook/assets/image (754).png>)

Click The Action Button and Select Generate Slices to automatically generate different size slices.

![](<../../.gitbook/assets/image (275).png>)

![](<../../.gitbook/assets/image (778).png>)

Vertical Slices will create 'count' number of vertical slices that are equal size.

![](<../../.gitbook/assets/image (245).png>)

## Delete

Delete the currently selected submodel(s).

![](<../../.gitbook/assets/image (402).png>)

{% hint style="info" %}
To select multiple submodel to delete, hold the shirt or ctrl/command key.
{% endhint %}

## Copy

Copy the currently selected submodel.

## Action

![](<../../.gitbook/assets/image (237).png>)

### Generate Slices

Select Generate Slices to automatically generate Subbuffer style Submodels.

### Flip All SubModels Vertical

This will flip all the node number rows, top to bottom, bottom to top.

### Flip All SubModels Horizontial

This will flip all the node number row values, left to right, right to left.

### Shift All Nodes in All SubModels

This will Shift all the submodels nodes numbering 1->21, 100->120

### Reverse All Nodes in All SubModels

This will reverse all the submodels nodes numbering. 1->100, 100->1.

## Import

![](<../../.gitbook/assets/image (86).png>)

### Import SubModels from Model

This allows the user to 'copy' submodels from another similar model. Example, if multiple mini-trees, are defined in your layout, only create the sub-models on one tree and then use this option to import the sub-models on all the other trees.

![](<../../.gitbook/assets/image (457).png>)

### Import SubModels from File

This allows the user to 'copy' submodels from a XModel file.

### Import Custom Model Overlay

This option will use a custom model file(.xmodel) to create submodels based on X/Y location of the node locations. The height and width of the custom model file must be smaller than the matrix height and width. This will also import the singing face and model state defines.

![](<../../.gitbook/assets/image (354) (1).png>)

## Export

![](<../../.gitbook/assets/image (445).png>)

### Export SubModels as CSV

This exports all the submodel definitions as a CSV file for viewer with Excel or other spreadsheet software.

### Export SubModel as xModel

This generates a Custom Model xModel file of the currently selected submodel.
